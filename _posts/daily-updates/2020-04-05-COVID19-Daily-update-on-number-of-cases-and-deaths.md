---
layout: post
title: COVID19 - Daily update on number of cases and deaths
date: 2020-04-05 11:54:00 +0100
category: daily-updates
---
[Federico Gallina](https://www.ulb.be/fr/federico-gallina) [(ECARES, ULB)](https://ecares.ulb.be) and [Glenn Magerman (ECARES, ULB)](http://www.glennmagerman.com).
#### 1. Introduction

-------------------------------------

This article presents daily numbers and insights on COVID infections. It analyzes the number of cases and deaths for the most infected countries in the world and the EU, and then presents more detailed statistics for Belgium.
By combining different statistics, we aim to better understand where we are in the trajectory of the epidemic.
As the epidemic evolves, we expect the number of infections and deaths to decrease and stabilize, and go to zero at the end of (the current wave of) the outbreak.
We also construct a real-time epidemic curve, which gets updated daily. At the end of the epidemic, the real-time epicurve converges to the true epicurve.

Today's key numbers:

- Global: 1,174,652 total cases, and 64,400 deaths in 204 countries with reported COVID-19 cases.

- EU28: 548,805, and 44,900 deaths.

- Belgium: 19,689 total cases, 5,735 total hospitalised, 1,261 in intensive care, 995 on respiration, 1,447 deceased, and 3,751 releaased.

<!--more-->

**Note 1**: We report statistics based on the number of confirmed COVID cases and deaths. These world-wide daily numbers are informative and the best which are available cross-country. However, they are not perfect.
First, by country, the number of infected people is certainly much higher than reported. One reason is that not everyone is, nor can be, tested. 
Second, cross-country differences in infection rates are in part driven by differences in testing policies, which can also vary over time.
Third, the number of cases does not convey the severity of the disease by case.
Fourth, over weekends, reporting lags can be larger.
Finally, there are [several sources of over, under and late reporting](https://www.bbc.com/future/article/20200401-coronavirus-why-death-and-mortality-rates-differ)) of the number of deaths, which again can vary over time and across countries.
We take these observations as given here.

**Note 2**: This article is of a  descriptive nature: it does not make any policy or normative statements. Please see [Learning from the curve](https://github.com/Learning-from-the-curve) for other initiatives.

**Note 3**: Analysis will be evolving as the project continues. Feedback, suggestions, and/or critiques are highly welcomed at [glenn.magerman@ulb.ac.be](glenn.magerman@ulb.ac.be).

**Data sources:**
- COVID data by country around the world from [ECDC](https://www.ecdc.europa.eu/en/publications-data/download-todays-data-geographic-distribution-covid-19-cases-worldwide).
- Country population data from [UN](https://population.un.org/wpp/Download/Standard/CSV). 
- Detailed COVID data for Belgium from [Epistat](https://epistat.wiv-isp.be/covid/). 
- Vector maps for Belgium from [geo.be](geo.be).
- Life tables for Belgium from [Statbel](https://statbel.fgov.be/sites/default/files/files/documents/bevolking/5.4%20Sterfte%2C%20levensverwachting%20en%20doodsoorzaken/5.4.3%20Sterftetafels%20en%20levensverwachting/sterftetafelsAE.xls).

### 2. Number of cases, world and EU28

-------------------------------------

#### 2.1 Number of cases

We start with reporting the number of cases for the 10 most infected countries in the world and the EU28.

Figure 1 shows the total number of cases over time.[^1]

[^1]:You can use the dropdown menu to select variants of the same curve. All graphs are interactive, and allow for a sub-selection of countries.

The country with the most cases is USA with 312,237 total confirmed cases. Second is Spain, with 124,736 confirmed cases, and Italy follows, with 124,632 cases.

The first tab reports the total number of cases (in log scale), since the 100th confirmed case within that country.
In the initial outbreak phase, the epidemic spreads exponentially, not arithmetically, i.e a log scale is the natural way to track the spread.
Synchronizing dates since the 100th confirmed case allows to compare the speed and evolution of the epidemic across countries.

However, [exponential growth curves cannot continue forever](https://medium.com/data-for-science/epidemic-modeling-101-or-why-your-covid19-exponential-fits-are-wrong-97aa50c55f8),
and growth has to decline at some moment due to constraints on the population its is passing through (conceptually, the availability of next victims to infect for various reasons (policies, geography, density...)).
China has been stabilizing since the end of February, signalling that the first peak has passed. However, new domestic cases signal the possible onset of a second wave.
Several countries show a decline in the increase of the number of new daily cases, hopefully pointing to passing a peak, or at least a stabilization of the number of infected people.
However, many countries are still facing exponential growth rates (linear in logs), signalling those countries face the onset of the pandemic.
The second tab shows the same total number of cases by date, in levels.

We repeat the graph for the 10 most infected countries in the EU28 in tabs 3 and 4.
The EU28 country with the most cases is Spain with 124,736 total confirmed cases. Second is Italy, with 124,632 confirmed cases, and Germany follows, with 91,714 cases.
It's worth noting that Sweden's infection rate has decreased significantly since around the 9th day after the 100th confirmed case, while having a [rather lenient policy](https://www.forbes.com/sites/davidnikel/2020/03/30/why-swedens-coronavirus-approach-is-so-different-from-others/#538677cb562b) towards the spread of the virus.  

{% include plots/daily-update-2020-04-05/2020-04-05-ln_cum_cases-after_100th.html %}
{% include plots/daily-update-2020-04-05/2020-04-05-cases_cum-dateRep.html %}
*Figure 1: Total cases.*

#### 2.2 Number of cases per million population

Figure 2 shows the total number of cases, per million population, since the 100th case per million people for these top 10 countries.
Absolute numbers are a key statistic in the onset of the epidemic, as they relate to the number of people infected from one patient.
Moreover, in standard S(E)IR models, the number of infected people rises almost identical in countries with vastly different population sizes.
The first few weeks in the outbreak, higher per-capita numbers mostly imply smaller countries, not different policies or growth rates.
However, as the epidemic evolves over time and reaches a steady state, a certain fraction of the population will be infected.
A significant part of the friction the virus encounters, and which in turn affects its growth rate, is country-specific: policy measures, geographic dispersion, population density etc.

Tab 1 shows these numbers for the 10 most infected countries in the world, tab 2 does this for the top 10 EU28 countries.
As of today, the country/region with the largest confirmed infection rate is San Marino, with an infection rate of around 0.765%.
This is still far off the [projections](https://www.hsph.harvard.edu/news/hsph-in-the-news/the-latest-on-the-coronavirus/) of 30-70% of adult world population ultimately being infected.
There are at least four plausible scenarios:
(i) real infection rates are orders of magnitude larger than reported ones. As of today, XXX has XXX% of its population measurably infected. If we are at the end of the epidemic, this implies real infection rates are around 100-300 times larger than currently reported.
We will never know the true infection rate (due to significant under-testing and a sizeable fraction of asymptomatic infected), and only obtain a guess at the end of the epidemic.
(ii) the epidemic is only in its onset, and we expect to reach higher infection rates. Given that most countries have not passed their first peak yet, this is a plausible scenario.
(iii) we are reaching the end of the epidemic, and infection rates are much lower than projected. Given the growth rates and our initial estimates for epidemic curves discussed below, we believe this scenario is not probable at this moment.
(iv) flattening-the-curve policies lowers the speed with which the epidemic rages. It is not clear yet whether these policies affect the total infection rate at the end of the epidemic.
With these policies in place, the share of infected population can grow at a lower rate but over a longer period.

{% include plots/daily-update-2020-04-05/2020-04-05-ln_cases_per_mln_cum-after_100th_per_mln.html %}
*Figure 2: Total cases, per million population.*

#### 2.3 Growth rate of the number of cases

Next, we plot the evolution of growth rates of the number of cases.
Growth rates are expressed in percentage changes from date *t-1* to *t*.[^2]

[^2]: The growth rate on absolute numbers is identical to one calculated as cases per million inhabitants.
We take a 3-day simple moving average to account for strong fluctuations from e.g. reporting lags within countries.

Each country wants to see this growth rate going to zero as soon as possible.

Two things are worth noting.
First, the slopes, or decreases in growth rates, are not the same across countries.
Second, even smoothed by a 3-day moving average, these growth rates are not monotonically decreasing. This might be partially due to temporal new outbursts of the virus within countries, or to increased testing policies.[^3]

[^3]: Approximating these growth rates with a 4th-order polynomial fit also shows these non-monotonicities.


{% include plots/daily-update-2020-04-05/2020-04-05-MA_cases-after_100th.html %}
*Figure 3: Growth rates, number of cases.*

### 3. Number of deaths, world and EU28

-------------------------------------

#### 3.1 Number of deaths

As noted in the introduction, the number of cases is prone to several important sources of non-random measurement error.
While measurement error also exists for the number of deaths, this number draws a clearer (but morbid) picture.

Figure 4 shows the total number of deaths for the top 10 countries with the deadliest outbreak over time.
As of today, the country with the most deaths is Italy, with 15,362 deaths.
Second is Spain, with 11,744 deaths, and USA follows, with 8,501 deaths.

The first tab plots the total number of deaths (in log scale) since the 10th death.
Again, we see that China has stabilized for now, with around 3,500 deaths.
Since the second half of February, China has been overtaken by Italy and Spain.
Since April 1, the USA is the country with the third highest number of deaths due to COVID.
Most western countries are on a similar trajectory as Italy, with Spain faring worse, and Sweden and Germany being on a better growth path.

The second tab shows the same total number of deaths by date, in levels.

We repeat the graph for the 10 highest mortality countries in the EU28 in tabs 3 and 4.
The EU28 country with the most deaths is Italy with 15,362 deaths. Second is Spain, with 11,744, and France follows, with 7,560 deaths.

{% include plots/daily-update-2020-04-05/2020-04-05-ln_cum_deaths-after_10th.html %}
{% include plots/daily-update-2020-04-05/2020-04-05-deaths_cum-dateRep.html %}
*Figure 4: Total deaths.*

#### 3.2 Number of deaths per million population

Figure 5 shows the total number of deaths, per million population, since the 10th death per million people for these top 10 countries.

{% include plots/daily-update-2020-04-05/2020-04-05-ln_deaths_per_mln_cum-after_10th_per_mln.html %}
*Figure 5: Total deaths, per million population.*

#### 3.3 Growth rate of the number of deaths

We plot the evolution of growth rates of the number of deaths in Figure 6.
The growth rate of Italy is slowing down relatively fast, a hopeful sign.
However, other countries like the United States or the United Kingdom, so not see steady declining growth rates yet.

{% include plots/daily-update-2020-04-05/2020-04-05-MA_deaths-after_10th.html %}
*Figure 6: Growth rates, number of deaths.*

### 4. Derived measures, world and EU28

-------------------------------------

We continue with two measures that are highly imperfect, but serve as a benchmark for longer time horizons in tracking the epidemic spread.

The first is the mortality rate, or the number of people dying from COVID as a fraction of total population.
For the 10 countries with the highest current mortality rates in the world, this is reported in Figure 7, tab 1. For the EU, this is reported in tab 3.

Since population is (nearly) fixed, this number will increase monotonically over time and reach a constant value at the end of the epidemic. Various studies put the mortality rate in a range between 1% and 8%.
There are several sources of measurement error.[^4]

[^4]: See also Note 1 in the introduction.

Therefore, the rate within countries is more informative than the cross-country comparison of the levels of these rates, and we focus on the direction and speed of these measures, rather than their absolute numbers.

The second measure is the case-fatality rate (CFR), which reports the number of people dying as a fraction of the infected population. This number is always higher than the mortality rate, as it is a ratio over a strict subset of the population (confirmed infected cases).
This measure also deserves important critiques.
First, in real time, estimates of the CFR can be biased upwards by under-reporting of cases, and downwards by failure to account for the delay from confirmation to death.
Second, the CFR is surely biased upwards since the true number of infected people is much larger than what is reported. Therefore, we focus on the within-country evolution of these rates, rather than comparing across countries, or even the numbers themselves at face value.
Again, we therefore rather focus on the direction and growth of these numbers within countries, acknowledging there might also be within-country changes over time that drive part of the patterns.

{% include plots/daily-update-2020-04-05/2020-04-05-fatality_rate-mortality_rate-after_10th.html %}
*Figure 7: Growth rates, number of deaths.*

### 5. Estimated epidemic curves, world and EU28

-------------------------------------

We conclude with an estimate of real-time epidemic curves for cases and deaths, for both the top 10 world countries and the EU.
It reports the fraction of total cases/deaths over the span of the disease.
When anyone is talking about "flattening the curve", THIS is the curve.

Comparing outbreaks over time or across countries helps to better understand the evolution in the future or in other countries (conditional on other factors).
These curves provide information on the speed (growth rate by day) and severity (number of cases/deaths) of the COVID epidemic, and are important blueprints to benchmark further outbreaks of the disease in the future.

The drawback is that epicurves are only available at the end of the disease.
At that moment, we will have the full distribution of cases/deaths over time per country (conditional on all the remarks on the measurement of cases and deaths).
Some examples of epicurves for [Mers-Cov](https://www.nature.com/articles/s41598-019-43586-9), [SARS](https://www.who.int/csr/sars/epicurve/epiindex/en/index1.html), [influenza in Canada](https://onlinelibrary.wiley.com/doi/full/10.1111/j.1750-2659.2010.00154.x) and [influenza in Belgium](https://epistat.wiv-isp.be/influenza/).

Still, we go ahead and construct epicurves for different countries as the disease evolves, as follows.[^5]

[^5]: Our approach is a naive and brute-force method to construct these real-time epicurves. There are much more refined methods available, such as [Bayesian estimation](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0002185).

First, under the assumption that China has completed the (first) outbreak of the disease, we use China as a benchmark epicurve.
Second, we compare cases and deaths for several countries over time as their outbreak evolves, and we update the curves daily. At the end of the outbreak for a country, in theory the real-time epicurve coincides with the true epicurve. In practice, we still face measurement issues.
As more countries complete the outbreak cycle, they will contribute to the benchmark of "the" epicurve for COVID for other countries still completing their cycles. In other words, we keep an eye on this as more countries pass the first peak and this solidifies the structure of the general epicurve.
Third, to compare across countries, the epicurves are centered around a turning point, where the new number of cases or deaths at a given time is maximal.
Since it is never certain what the maximum is until at the end of the outbreak, we estimate the turning point based on the growth rate of cases/ deaths. In particular, we predict future growth rates using a 4th degree polynomial on current growth rates presented above.
The predicted turning point is then used to calibrate the graph and to compare the curve to the benchmark (China).
Fourth, the y-axis is reported in the fraction of cases/deaths over the length of the outbreak. Together with the turning point, his allows us to compare epicurves across countries. Again, for the real-time epicurves, we calculate the future number of cases based on predicted growth rates to calibrate the y-axis.

These initial projections suggest that China has experienced a turning point at around 25-30 days. Italy might be on a similar track with a turning point at around 30 days.
Most other countries however, still face increasing rates of infections and deaths.

Finally, we strongly underline that it is highly probable that additional waves will arrive within a country. As of today, it is not certain that China has finished its full cycle, or that there are seasonal cycles coming up.
Additionally, these patterns take as given the current policy measures. Too early lifting of measures can and will result in a direct second wave.
These figures do not serve as any policy measure in any way. They only serve to get an estimate of the epicurves in real time, instead of waiting until the end of the outbreak.


{% include plots/daily-update-2020-04-05/2020-04-05-MA_ln_share_deaths-MA_ln_share_cases-midpoint.html %}
*Figure 8: Real-time epicurves.*

### 6. Updates for Belgium

-------------------------------------

Finally, we provide more detailed and daily updated statistics for Belgium.
As of today, there are 19,689 total cases, 735 total hospitalised, 1,261 in intensive care, 995 on respiration, 1,447 deceased, and 3,751 patients releaased from the hospital.

Figure 9 shows total COVID numbers for confirmed cases, hospitalized patients, hospitalized patients in intensive care, hospitalized patientsunder respiratory support, and deceased patients by date.
There is a maximum capacity of 2,293 ICU beds reserved for COVID patients (red horizontal line).

![](/assets/images/daily-updates/2020-04-05/BE_cases_hosp_dead.svg)
*Figure 9: Cases, hospitalization and deaths.*

Figure 10 shows the number of cases and hospitalized patients by province, as of today.[^6]

[^6]: There is unfortunately no information on the number of deceased patients by province.

![](/assets/images/daily-updates/2020-04-05/BE_hosp_by_province.svg)
*Figure 10: Cases, hospitalization and deaths.*

Next, we show the number of cases by city in Figure 11.[^7]

[^7]: At this stage, there is only info on the number of cases by city, not deaths.

The city with the highest number of infections is Antwerpen with 5,735. Luik follows with 369 and Bergen is third with 326 cases.
In absolute terms, Flanders is much more infected than Wallonia, and these infections are also spread out across cities.

![](/assets/images/daily-updates/2020-04-05/BE_cumcases_bycity.svg)
*Figure 11: Cases, by city.*

Finally, we end with a comparison of the age distribution of COVID deaths, against life expectancy for Belgians in 2018.
Figure 12 shows a cumulative distribution function of the life tables for Belgium (i.e. the probability of dying at a certain age).
For reference, tab XXX shows the distribution of life expectancy in Belgium for both sexes jointly, and male and female separately. Females have in general a higher life expectancy than males.

We then compare these life expectancy tables with the age distribution of COVID deaths.
We discretize the distribution to match the COVID data which is represented in age bins (0-24 years, 25-44, 45-64, 65-74, 75-84, 85+).
While the life tables are fixed, the COVID death tolls by age are updated daily.
Clearly, there is a higher than expected death rate for elderly. We split the comparison also by sex.

We also compare COVID deaths by region (Brussels, Flanders, Wallonia) against the Belgian life tables.

![](/assets/images/daily-updates/2020-04-05/BE_lifetables_bysex.svg)
![](/assets/images/daily-updates/2020-04-05/BE_lifetable_all.svg)
![](/assets/images/daily-updates/2020-04-05/BE_lifetable_male.svg)
![](/assets/images/daily-updates/2020-04-05/BE_lifetable_female.svg)
![](/assets/images/daily-updates/2020-04-05/BE_lifetable_regions.svg)

*Figure 12: Life expectancy and COVID deaths by age.*

We are back with updated numbers tomorrow.

In the mean time, stay safe, and take care of yourself and of others.

Federico and Glenn.
