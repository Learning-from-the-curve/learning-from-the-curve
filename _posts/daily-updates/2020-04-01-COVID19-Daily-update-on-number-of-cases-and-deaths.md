---
layout: post
title: COVID19 - Daily update on number of cases and deaths
date: 2020-04-01 11:54:00 +0100
category: daily-updates
---
[Federico Gallina](https://www.ulb.be/fr/federico-gallina) [(ECARES, ULB)](https://ecares.ulb.be), [Glenn Magerman (ECARES, ULB)](http://www.glennmagerman.com), and the [“Learning from the curve” team](https://github.com/Learning-from-the-curve).

#### 1. Introduction

-------------------------------------

This article presents daily numbers and insights on COVID infections. It analyzes the number of cases and deaths for the most infected countries in the world and the EU,
and then presents more detailed statistics for Belgium. The report is updated every day at 13:30 CET,
after publication of the global [ECDC](https://www.ecdc.europa.eu/en/publications-data/download-todays-data-geographic-distribution-covid-19-cases-worldwide) and Belgian [Epistat](https://epistat.wiv-isp.be/covid/) numbers.

<!--more-->

**Note 1**: We report statistics based on the number of confirmed COVID cases and deaths. These world-wide daily numbers are fantastic. However, they are also not perfect.

- First, the number of infected people is certainly higher than reported. One reason is that not everyone is, nor can be, tested in every country. Specialists estimate the "dark number" (the real number of infected people not captured in the statistics) to be 10 or 100 times larger than recorded.

- Second, there are cross-country differences in the number of cases due to differences in testing policies. Some countries have implemented aggressive testing, random sampling, blood tests, while others only test hospitalized people and/or with severe symptoms. This inadvertly raises confirmed cases for the countries that test more extensively.

- Third, the number of cases does not convey the severity of the disease by case.

- Finally, for deaths, there can be overreporting (comorbidity as cause of death, or other mortalities statistically allocated to COVID mortality) and underreporting (no confirmed COVID diagnosis). We imagine there can be large heterogeneity in this under/overreporting across countries.

We take these numbers and these cautions as given.

**Note 2**: This article is of a  descriptive nature: it does not make any policy statements, nor does it attemp to measure the impact of earlier policy measures. Please see [Learning from the curve](https://github.com/Learning-from-the-curve) for other initiatives in those directions.

**Note 3**: Analysis will be evolving as the project continues. Any feedback, suggestions, critiques, are highly welcomed.

**Data sources:**

- COVID data by country around the world comes from [ECDC](https://www.ecdc.europa.eu/en/publications-data/download-todays-data-geographic-distribution-covid-19-cases-worldwide).

- Country population data comes from [UN](https://population.un.org/wpp/Download/Standard/CSV).

- Detailed COVID data for Belgium from [Epistat](https://epistat.wiv-isp.be/covid/).

#### 2. Global overview

-------------------------------------

As of today, there are 853,200 total cases, 41,887 deaths and 202 countries with reported COVID cases.

##### 2.1 Number of cases

Figure 1 shows the total number of cases by date for the 10 most infected countries in the world. This is a snapshot of the outbreak across countries. While China has been stabilizing since the end of February, many countries are still facing the onset of the pandemic in their country. The country with the most cases is the United States of America, with 189,618 total confirmed cases. Second is Italy with 105,792 confirmed cases, and Spain follows, with 94,417 cases.

{% include plots/daily-update-2020-04-01/2020-04-01-cases_cum-dateRep-plain.html %}
*Figure 1: Total cases by date, global top 10.*

Next, Figure 2 shows the total number of cases per million inhabitants, since the 100th case per million inhabitants for these top 10 countries. The graph differs from the first figure in two ways. First, it accounts for population size. While absolute numbers are a key statistic in the onset of the epidemic, as they relate to the number of people infected from one patient, as the epidemic evolves and reaches a steady state, a particular fraction of the population will be infected. E.g. Belgium can simply never reach the same theoretical maximum number of infected people as the USA.[^1]

[^1]: We could also aggregate all countries in the EU to compare against the USA and China. Additionally, there might be within-country regional differences that affect both absolute and relative numbers (e.g. China is not affected homogeneously in all provinces).

Second, the figure plots the number of cases since the 100th case per million, instead of calendar days. This allows to compare growth rates of the epidemic across countries, accounting for differences in timing of the onset of the epidemic across countries.

As of today, the Vatican City has 0.751% of its population officially infected. This is still far off the estimates of 30-70% of world population ultimately being infected. There can be at least three reasons: (i) real infection rates are orders of magnitude larger than reported ones, (ii) the epidemic is only in its onset, (iii) we are reaching the end of the epidemic, and infection rates are lower than previously projected. Given the growth rates discussed below, we believe (iii) is not plausible at this moment.

{% include plots/daily-update-2020-04-01/2020-04-01-cases_per_mln_cum-after_100th_per_mln.html %}
*Figure 2: Total cases since 100th case, per million inhabitants, global top 10.*

Next, Figure 3 shows the growth rate of the number of cases, since the 100th case for the top 10 infected countries. Growth is expressed as the percentage growth rate of the total number of cases from date *t-1* to *t*.[^2]

[^2]: This growth rate is identical to one calculated as cases per million inhabitants as we divide both numerator and denominator by population per million.

We take the 3-day simple moving average to account for strong fluctuations from e.g. reporting lags. Every country wants to see this growth rate going to zero as soon as possible. China has officially reached that state. Other countries still see growth rates of 10-30% per day.

Two things stand out. First, the slopes, or decreases in growth rates, are not the same across countries. This implies some countries will get to zero growth faster than others. Second, even smoothed by a moving average, these growth rates are not monotonically decreasing. This might be due to temporal outbursts of the virus within countries, or partially due to increased testing policies.

{% include plots/daily-update-2020-04-01/2020-04-01-MA_cases-after_100th.html %}
*Figure 3: Growth rate cases, since 100th case, global top 10.*

##### 2.2 Number of deaths

As noted in the introduction, the number of cases is prone to several sources of non-random measurement error. While measurement error also exists for the number of deaths, this number draws a clearer picture. It also captures the severity of the epidemic. Furthermore, some hypotheses described above using case data might turn out to be less plausible than others.

Figure 4 shows the total number of deaths for the top 10 countries with the deadliest outbreak by date. Since the second half of February, China has been overtaken by Italy and Spain. Since April 1, the USA is the country with the third highest number of deaths due to COVID. As of today, the country with the most deaths is Italy, with 12,430 deaths. Second is Spain, with 8,189 deaths, and the United States of America follows, with 4,079 deaths.

{% include plots/daily-update-2020-04-01/2020-04-01-deaths_cum-dateRep-plain.html %}
*Figure 4: Total deaths by date, global top 10.*

Accounting for population size, Figure 5 shows the total number of deaths per million inhabitants, since the 10th death per million, and this for the top 10 deadliest countries. As before, this graph presents the share of population deceased instead of absolute numbers, and it aligns the evolution of mortality across countries' different epidemic onset times. Here, most countries are on an even worse trajectory than Italy.

{% include plots/daily-update-2020-04-01/2020-04-01-deaths_per_mln_cum-after_10th_per_mln.html %}
*Figure 5: Total deaths since 10th death, per million inhabitants, global top 10.*

Finally, Figure 6 shows the growth rate of the number of deaths, since the 10th case. Again, growth is expressed as the percentage growth rate of the total number of cases from date *t-1* to *t*, and we use the 3-day moving average to smooth reporting lags. Every country wants to see this growth rate going to zero as soon as possible. Again, China has officially reached that state. If we can extrapolate these curves, Iran might reach its end of the epidemic at around day 80, or roughly 40 days from now. Italy follows later, while Spain might do better. Unfortunately, the USA still faces growth rates of the number of deaths between 20 and 30%, with no significant signs of the growth rates decreasing at the moment.

{% include plots/daily-update-2020-04-01/2020-04-01-MA_deaths-after_10th.html %}
*Figure 6: Growth rate deaths, since 10th death, global top 10.*

#### 3. EU28 overview

-------------------------------------

We repeat the same analysis for the EU28 countries, and highlight the top 10 countries within the EU28. As of today, there are 416,158 confirmed cases in the EU28, and 29,320 deaths.

##### 3.1 Number of cases, EU28

Figure 7 shows the total number of cases by date for the 10 most infected countries in the EU28. The EU28 country with the most cases is Italy with 105,792 total confirmed cases. Second is Spain, with 94,417 confirmed cases, and Germany follows, with 67,366 cases.

{% include plots/daily-update-2020-04-01/2020-04-01-cases_cum-dateRep-plain-EU28.html %}
*Figure 7: Total cases by date, EU28 top 10.*

Next, Figure 8 shows the total number of cases per million inhabitants, since the 100th case per million inhabitants for these most infected EU28 countries. Again, some countries are on a steeper path than Italy. As of today, Vatican City has 0.751% of its population officially infected.

{% include plots/daily-update-2020-04-01/2020-04-01-cases_per_mln_cum-after_100th_per_mlnEU28.html %}
*Figure 8: Total cases since 100th case, per million inhabitants, EU28 top 10.*

Next, Figure 9 shows the growth rate of the number of cases, since the 100th case for the top 10 infected countries in the EU. Growth is expressed as the percentage growth rate of the total number of cases from date *t-1* to *t*, and we take the 3-day simple moving average to account for strong fluctuations from e.g. reporting lags. Again, every country wants to see this growth rate going to zero as soon as possible. Growth rates are roughly between 5% and 20% as of today.

{% include plots/daily-update-2020-04-01/2020-04-01-MA_cases-after_100thEU28.html %}
*Figure 9: Growth rate cases, since 100th case, EU28 top 10.*

##### 3.2 Number of deaths, EU28

Finally, we turn to the number of deaths for the top 10 EU28 countries.

Figure 10 shows the total number of deaths for the top 10 EU28 countries with the deadliest outbreak by date. As of today, the country with the most deaths is Italy, with 12,430 deaths. Second is Spain, with 8,189 deaths, and France follows, with 3,523 deaths.

{% include plots/daily-update-2020-04-01/2020-04-01-deaths_cum-dateRep-plain-EU28.html %}
*Figure 10: Total deaths by date, EU28 top 10.*

Accounting for population size, Figure 11 shows the total number of deaths per million inhabitants, since the 10th death per million, and this for the top 10 deadliest EU28 countries. As before, this graph presents the share of population deceased instead of absolute numbers, and it aligns the evolution of mortality across countries' different epidemic onset times. Again, also in the EU, most countries are on an even worse trajectory than Italy.

{% include plots/daily-update-2020-04-01/2020-04-01-deaths_per_mln_cum-after_10th_per_mlnEU28.html %}
*Figure 11: Total deaths since 10th death, per million inhabitants, EU28 top 10.*

Finally, Figure 12 shows the growth rate of the number of deaths, since the 10th case. Again, growth is expressed as the percentage growth rate of the total number of cases from date *t-1* to t, and we use the 3-day moving average to smooth reporting lags. These growth rates suggest that most countries are still in the onset part of the epidemic.

{% include plots/daily-update-2020-04-01/2020-04-01-MA_deaths-after_10thEU28.html %}
*Figure 12: Growth rate deaths, since 10th death, EU28 top 10.*
