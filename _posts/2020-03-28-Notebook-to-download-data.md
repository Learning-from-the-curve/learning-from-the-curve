---
layout: post
title: Notebook to download data
date: 2020-03-28 15:41:00 +0100
category: project-2
---
This notebook imports data for COVID related analysis from a number of online sources.

First of all, we need to import a few useful libraries.

<!--more-->

```python
import pandas as pd
import os
from pandasdmx import Request
import eurostat
from concurrent.futures import ThreadPoolExecutor
import time
```

Make sure to have all packages. If not, type "pip install --namepackage--" in the console or in the terminal. We can now start to get the data.

Define function to get the downloaded data in empty lists.

```python
start_time = time.time()

def data(url, container):
    ind = 0
    for i in url:
        if ind <= len(url):
            container.append([url[ind][0],pd.read_csv(url[ind][1], index_col = 0, parse_dates = [0])])
        ind += 1
```

Here is an extract of the data

#### Data From [World Population Prospects](https://population.un.org/wpp/Download/Standard/CSV/) and [Johns Hopkins](https://github.com/CSSEGISandData/COVID-19/tree/master/csse_covid_19_data/csse_covid_19_time_series)

John Hopkins provides daily data on **confirmed cases**, **deaths** and **recovered** for many countries in the world. Data can be freely accessed through GitHub. We can also get data from the UN.

```python
url_WPP = [['WPP_tot_pop', 'https://population.un.org/wpp/Download/Files/1_Indicators%20(Standard)/CSV_FILES/WPP2019_TotalPopulationBySex.csv'],
          ['WPP_pop_age_sec', 'https://population.un.org/wpp/Download/Files/1_Indicators%20(Standard)/CSV_FILES/WPP2019_PopulationByAgeSex_Medium.csv'],
          ['WPP_fertility', 'https://population.un.org/wpp/Download/Files/1_Indicators%20(Standard)/CSV_FILES/WPP2019_Fertility_by_Age.csv']]

url_JH = [['JH_confirmed', 'https://raw.githubusercontent.com/CSSEGISandData/COVID-19/master/csse_covid_19_data/csse_covid_19_time_series/time_series_covid19_confirmed_global.csv'],
            ['JH_death', 'https://raw.githubusercontent.com/CSSEGISandData/COVID-19/master/csse_covid_19_data/csse_covid_19_time_series/time_series_covid19_deaths_global.csv'],
            ['JH_recovered', 'https://raw.githubusercontent.com/CSSEGISandData/COVID-19/master/csse_covid_19_data/csse_covid_19_time_series/time_series_covid19_recovered_global.csv']]

```

#### Data From [Eurostat](https://ec.europa.eu/eurostat/web/population-demography-migration-projections/data/database)

The library Eurostat allows to get demographics data in one line of code. We download data about population as well as national accounts. Data need to be cleaned for later usage.

```python
def EU_stat(url, container):
    ind = 0
    for i in url:
        if ind <= len(url):
            container.append([url[ind][0], eurostat.get_data_df(url[ind][1])])
        ind += 1
```

Define the variables according to their codes on eurostat.

```python
data_eurostat = [['EU_pop', 'demo_r_gind3'], ['EU_gdp', 'nama_10_gdp'], ['EU_cons', 'nama_10_fcs'], ['EU_trade', 'nama_10_exi'], ['EU_short_rate', 'irt_st_a'],
                ['EU_long_rate', 'irt_lt_gby10_a'], ['EU_unemp', 'une_rt_a'], ['EU_inv', 'nama_10_an6']]
```

Create empty containers and run the functions

```python
JH = []
WPP = []
EU = []

with ThreadPoolExecutor(max_workers = 3) as e:
    e.submit(data(url_JH, JH))
    e.submit(data(url_WPP, WPP))
    e.submit(EU_stat(data_eurostat, EU))
```

#### Save all data

Run the lines below **only** if you need to save data locally. The default path of the function is your current working directory. If another path is specified, the function will create the folders in that path if they do not already exist.

```python
def store_data(path = os.getcwd(), JH_data = True, WPP_data = True, EU_data = True):
    os.makedirs(path, exist_ok = True)
    if JH_data:
        ind = 0
        for i in JH:
            JH[ind][1].to_csv(path + JH[ind][0] + '.csv', index = False)
            ind += 1
    if WPP_data:
        ind = 0
        for i in WPP:
            WPP[ind][1].to_csv(path + WPP[ind][0] + '.csv', index = False)
            ind += 1
    if EU_data:
        ind = 0
        for i in EU:
            EU[ind][1].to_csv(path + EU[ind][0] + '.csv', index = False)
            ind += 1
```

Save the data in a folder called *files* inside your current working directory.

```python
store_data(os.getcwd() + "/files/")
end_time = time.time()
print(f"Total time: {end_time - start_time}")
```

    Total time: 255.59749102592468
