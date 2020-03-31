---
layout: post
title: Interactive plot
date: 2020-03-29 15:41:00 +0100
authors:
  - Federico Gallina
category: project-2
---
trial
```python
import pandas as pd
import matplotlib.pyplot as plt
import mpld3
from mpld3 import plugins

covid = pd.read_excel("./input/COVID-19-geographic-disbtribution-worldwide-2020-03-28.xlsx", index_col = [6, 0])
covid = covid[['cases','deaths']]
cumulative_cases = covid.sort_index().groupby(['countriesAndTerritories']).cumsum()
temp_cases = cumulative_cases.swaplevel().reset_index()
rank = temp_cases.loc[temp_cases['dateRep'] == '2020-03-28']
rank = rank.sort_values(by='cases')
top10 = list(rank['countriesAndTerritories'][-10:])
top10_cumulative = cumulative_cases.loc[top10].reset_index(level = 'dateRep')
```
<!--more-->
```python
fig, ax = plt.subplots(figsize = (12, 6))
ax.grid(True, alpha=0.3)
labels_points = []
lines_list = []
for country in top10:
    points = ax.plot(top10_cumulative.loc[country, 'dateRep'], top10_cumulative.loc[country, 'cases'], label=country, marker = 'o')
    lines_list.append(points)
    temp_labels_points = []
    for i in range(len(top10_cumulative.loc[country, 'cases'])):
        label = top10_cumulative.loc[country, 'cases'][i]
        label_date = str(top10_cumulative.loc[country, 'dateRep'][i])
        # .to_html() is unicode; so make leading 'u' go away with str()
        temp_labels_points.append(f'{label_date[:11]}: {label:,}')
    labels_points.append(temp_labels_points)
# define interactive legend

handles, labels = ax.get_legend_handles_labels() # return lines and labels
interactive_legend = plugins.InteractiveLegendPlugin(handles, labels, alpha_unsel=0, alpha_over=3.5, start_visible=True)

tooltip = []
for i in range(len(top10)):
    tooltip.append(plugins.PointHTMLTooltip(lines_list[i][0], labels_points[i], voffset=-30, hoffset=-100))

plugins.connect(fig, interactive_legend, *tooltip)

ax.set_xlabel('Date')
ax.set_ylabel('Number of cases')
ax.set_title('Interactive legend', size=20)
fig.subplots_adjust(right=0.7)

mpld3.display()
```

{% include Interactive_cumulative.html %}
