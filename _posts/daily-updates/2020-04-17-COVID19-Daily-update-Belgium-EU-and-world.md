---

layout: post

title: COVID-19 - Daily update Belgium, EU and world

date: 2020-04-17 12:00:00 +0100

category: daily-updates

---

[Federico Gallina](https://www.ulb.be/fr/federico-gallina) [(ECARES, ULB)](https://ecares.ulb.be) and [Glenn Magerman (ECARES, ULB)](http://www.glennmagerman.com), with the [Learning from the curve](https://github.com/Learning-from-the-curve) team.

This article presents daily insights on COVID-19 for Belgium, the EU28 and the most infected countries in the world. We report cases, hospitalizations and deaths for Belgium. We also compare life expectancy with COVID deaths by age groups, and calibrate a real-time epidemic curve. We then report patterns on cases and deaths for other countries, lockdown policies and their epicurves. By combining these different statistics, we aim to better understand where we are in the trajectory of the epidemic.

This article is updated daily after 13:30.

Today's key numbers:

- Global: 2,114,269 total cases, and 145,144 deaths in 206 countries with reported COVID-19 cases.
- EU28: 869,611, and 89,680 deaths.
- Belgium: 35,546 total cases, 5,161 total hospitalised, 1,140 in intensive care, 5,163 deceased, and 7,961 recovered.

<!--more-->

**Important**: Statistics on the number of COVID cases and deaths are useful and are the best that are available cross-country, but they are not perfect. Some warnings and thoughts on the interpretation of these numbers:

**Note 1**: The number of infections is certainly much higher than reported in every country. Not everyone is, will be, nor can be, tested. This can be due to a combination of several factors. First, technical constraints make it impossible to test the whole population. This can for example be due to limited resources on test material, and how to reach everyone in the population. Second, policy choices determine who gets tested and who not. For instance, in Belgium, the latest policies include testing all people in retirement homes, which did not happen until the last few days. Third, there is evidence of a large share of asymptomatic patients, which would never ask to be tested nor will show up in hospitals or other statistics. We would therefore suggest to use (stratified) random sampling across the population to deal with these three factors simultaneously, and to get a better grip on the share of people infected in the population. Methods that currently over-sample particular subgroups of the population (e.g. health workers, people in retirement homes, workers in crucial sectors) are important to map the spread of the virus in these subgroups, but have to be properly reweighted to give information on the infectiousness of the population. In attendance of such sampling strategies and data, the number of hospitalizations is arguably a better measure to evaluate the severity of the disease. Further detailed information on demographics and pre-existing conditions of tested people would be important to make targeted policy decisions. There are [several sources of over, under and late reporting](https://www.bbc.com/future/article/20200401-coronavirus-why-death-and-mortality-rates-differ) which vary over time and across countries. See also [Bloomberg](https://www.bloomberg.com/opinion/articles/2020-03-28/confirmed-coronavirus-cases-is-an-almost-meaningless-metric) for a discussion on testing policies.

**Note 2**: Differences in testing policies drive part of the variation in infection rates across countries, as some countries implement more aggressive testing than others. Moreover, these testing policies can also change within countries over time. Therefore, both across- and within-country numbers do not only reflect the evolution of the virus per se, but also policies. Different policies across countries can result in different levels of the number or share of cases in the population. This is a large part of the current debate in the media, such as Belgium reporting more deaths due to COVID, or the USA reporting higher numbers because there is more testing. Still, these numbers can be informative. For example, if we keep fixed testing and reporting policies within countries over time, the evolution of cases, hospitalizations, deaths etc. within that country tells us a lot about the evolution of the virus in that country. Relative changes across countries can then be informative of differences in spreads, policies, recoveries etc. However, policies on testing and reporting also change over time within countries. These have to be carefully considered when analyzing within-country evolutions.

**Note 3**: Both absolute and relative numbers (as a share of the population) are informative. In the onset of the epidemic, the absolute number of cases matters the most. Models of epidemiological spreads (such as the S(E)IR models) predict a very similar number of cases in the onset, whether this is a small country like Belgium, or a large one like the USA. Over the evolution of the epidemic however, a particular share of the population will be infected or deceased. These relative numbers matter more for the longer time horizon of the epidemic, and account for e.g. differences in country size. Across-country differences in the share of population infected/deceased are still partly due to reporting (see Note 1), but also reflect differences in policies, population density and geographic dispersion. As a side note, the adequate level of population as in country/region/state/province etc. depends on several factors that in turn depend on the particular question at hand. For instance, most of the outbreak in China is concentrated in the province of Hubei. Should we count China as a whole, or only Hubei as the relevant population? Should we compare Italy to the USA? Maybe not when comparing infection shares, but when we want to analyze policy decisions, there are most often made at the federal level.

**Note 4**: This report shows descriptive statistics on the evolution of the COVID disease. We do not present policy recommendations, counterfactual analysis or structural predictions here. Our behaviour impacts the curve, not the other way around...

**Note 5**: We share all codes for this report (Python and Stata versions) and other projects on [GitHub](https://github.com/Learning-from-the-curve/daily-updates) for other researchers or contributors to use, and for the general public. See our other projects at [Learning from the curve](https://github.com/Learning-from-the-curve), an initiative of several researchers at [ECARES](http://ecares.ulb.be/), [Solvay](https://www.solvay.edu/en/), [ULB](www.ulb.be). Any comments, suggestions or contributions are highly welcomed at [glenn.magerman@ulb.ac.be](glenn.magerman@ulb.ac.be)

**Data sources:**

- Detailed COVID data for Belgium from [Epistat](https://epistat.wiv-isp.be/covid/).

- Shape files for Belgium from [geo.be](geo.be).

- Geojson data used for interactive maps can be found [here](https://github.com/Datafable/rolling-blackout-belgium/blob/master/data/geospatial/municipalities-belgium.geojson).

- Life tables and population for Belgium from [Statbel](https://statbel.fgov.be).

- COVID data by country around the world from [ECDC](https://www.ecdc.europa.eu/en/publications-data/download-todays-data-geographic-distribution-covid-19-cases-worldwide).

- Country population data from [UN](https://population.un.org/wpp/Download/Standard/CSV).

- Policy measures from [Oxford COVID-19 Government Response Tracker](https://www.bsg.ox.ac.uk/research/research-projects/oxford-covid-19-government-response-tracker).

**Table of Contents**:<a name="tbc"></a>

1. [Daily updates for Belgium](#cap1)

2. [Daily updates, world and EU28](#cap2)

### 1. Daily update for Belgium <a name="cap1"></a>

[*Back to Table of Contents*](#tbc)

-------------------------------------

#### 1.1 Cases, hospitalizations and mortality

We start with the analysis for Belgium. Figure 1 shows total COVID numbers for cases, hospitalizations and deceased patients by date. There are possible reporting lags, as different sources have to record and transmit their data to Epistat. We present the latest available numbers, the same as showcased on the Sciensano dashboard.[^1]

[^1]: A case is recorded as the date of symptoms onset, sampling, diagnosis, or reporting.

There are currently 35,546 confirmed infections, 5,161 hospitalized patients, 1,140 patients in intensive care, with 846 patients on respiratory aid, and 5,163 people have died from the infection. On the up side, 7,961 patients have been released from the hospital. There is a current maximum capacity of 2,293 ICU beds reserved for COVID patients, and 49.72% of capacity of ICU beds is taken.

There has been a moderate decline in the number of hospitalized patients up to around April 10, but as of today, this number might be increasing again. Any upward trend in the number of hospitalized people might signal the onset of a second wave of the epidemic in Belgium.

{% include plots/daily-update-2020-04-17/2020-04-17-Belgium-cumulative.html %}

<p style="text-align: center; font-style: italic;">Figure 1: Number of cases, hospitalizations and deaths in Belgium.</p>

Figure 2 shows the number of cases and hospitalized patients by province, for the latest available date.[^2] Most provinces are equally hit in terms of absolute numbers, with the exception of Brabant Wallon, Luxembourg and Namur, which are also the provinces with the lowest population count. In relative terms, Limburg is the hardest hit province with the highest number of cases per capita.

[^2]: Numbers by province can also be lagged; we present the latest available data. There is currently no information on the number of deceased patients by province.

{% include plots/daily-update-2020-04-17/2020-04-17-Belgium-province.html %}

<p style="text-align: center; font-style: italic;">Figure 2: Number of cases and hospitalizations by province.</p>

Next, Figure 3 shows the number of cases by municipality.[^3] The city with the highest number of infections is currently Antwerpen with 1,259. Liège follows with 811 and Brussel is third with 524 cases. In absolute terms, Flanders is much more infected than Wallonia, and these infections are also spread out across most cities. We also show the number of cases as a percentage of the population for each municipality (hover over the municipality to see the values).

When controlling for population by municipality, the pattern changes significantly. There are geographic clusters of the spread of the disease, with hard hit regions around Hasselt/Sint-Truiden, Mons and Liège.[^4]

[^3]: Currently, there is no information hospitalized or deceased patients by municipality.

[^4]: The geographic data used to build the map are from 2014. For the Belgian municipalities that merged in 2019 we include the former municipalities (pre-2019) separately, and we impute the cases for the merged municipality in 2019 to each pre-2019 municipality. Some of the polygons in the map are empty due to missing data for that municipality or a problem with the geographic data in the geojson file. For example, Elsene (Ixelles) is not on the map, but we know that it has 256 cumulative cases, that is 0.29% of its population is infected.

{% include plots/daily-update-2020-04-17/2020-04-17-Belgium-map.html %}

<p style="text-align: center; font-style: italic;">Figure 3: Number of cases by municipality.</p>

#### 1.2 COVID mortality by age groups and regions

In Figure 4, we compare the life expectancy for Belgium (blue) against COVID deaths (red) across age groups.

The blue curve plots the probability of being dead by a certain age, for all causes of death.[^5] The red curve shows mortality rates from COVID, across age groups. In particular, each curve shows the fraction of deaths up to a certain age. E.g. in general (blue curve), individuals have a probability of being dead by 70 years of age of around 15%. At 90 years, this probability increases to over 90%.

[^5]: In 2018, there was an influenza epidemic that generated significant over-mortality in the elderly. We average the densities over the years 2015-2017 to wash out year-specific peaks in mortality. There are some deaths reported without information on age, we drop these for the COVID CDF calculations. Since COVID mortality is given by age bins, we also bin the life tables. For each age bin (0-24 years, 25-44, 45-64, 65-74, 75-84, 85+), we take the midpoint.

Turning to COVID mortality, we see that the distribution for both sexes is skewed towards the elderly, with a turning point at around 70 years. More elderly people die from COVID than predicted by the life expectancy tables, relative to other age groups. Conversely, younger people have a higher probability of dying from another cause than one allocated to COVID. If COVID would not discriminate across age, both curves would coincide. Importantly, this curve might change over the course of the disease.
For instance if elderly people die faster, but also younger people die over the epidemic, the distribution might shift its gravitational point to younger ages later in the epidemic. Importantly, this data does not account for pre-existing conditions, some of which might be a plausible risk factor for COVID (diabetes, vascular diseases etc.): age and pre-existing conditions correlate strongly, and without more information, we cannot disentangle both causes of mortality. Still, there can be over-mortality in the population due to COVID even if COVID is not the direct cause of death, for example pre-existing conditions, an overload of the health case system that generates otherwise preventable deaths etc.

We also compare COVID deaths by age group across regions (Brussels, Flanders, Wallonia). There might be regional differences (e.g. from health care capacity or quality). For instance, there seems to be a slighly lower mortality rate for elderly in Wallonia, but there might be differences in reporting times across regions. E.g. deaths from nursery homes seem to be lagging more for Wallonia than Flanders or Brussels.

{% include plots/daily-update-2020-04-17/2020-04-17-Belgium-life-expectancy.html %}

<p style="text-align: center; font-style: italic;">Figure 4: Life expectancy versus distribution of COVD deaths by age groups and region.</p>

#### 1.3 Epicurve for Belgium

We conclude the analysis for Belgium with a real-time epidemic curve for cases and deaths in Figure 5.

The epicurve reports the fraction of total cases or deaths over the span of the disease. When people talk about "flattening the curve", THIS is the curve. Some examples of epicurves for [Mers-CoV](https://www.nature.com/articles/s41598-019-43586-9), [SARS](https://www.who.int/csr/sars/epicurve/epiindex/en/index1.html), [influenza in Canada](https://onlinelibrary.wiley.com/doi/full/10.1111/j.1750-2659.2010.00154.x) and [influenza in Belgium](https://epistat.wiv-isp.be/influenza/).

Epicurves are only available at the end of an outbreak. Then the length, peak and total number of cases or deaths are known. Still, we want to estimate where we are in the trajectory while the disease evolves.

We therefore estimate these numbers as follows. First, we target one or more countries that have potentially completed the first wave of the disease. We use these countries as a benchmark epicurve. As of today, we use China as a benchmark. As more countries complete the outbreak cycle, these will also contribute to the benchmark of the "true" epicurve for COVID.

Second, we map the trajectory for Belgium against that of China. This graph does not use any predictive models, but simply fits the plausible trajectory of Belgium. The mapping is as follows. First, we calculate the date with the largest number of cases in the data. That date is the peak, or "turning point". This shifts the currently observed data for Belgium relative to the trajectory of China on the *x*-axis. For China, we are past the first peak, while for Belgium, the peak is still not 100% certain, and a new daily record will shift the estimated turning point to that date. We plot the graphs from the date of passing the 0.01% case or 0.001% death in the data.
Then, we rescale each curve to be a fraction of cases or deaths out of the total numbers up until today. This rescales the curve on the *y*-axis. The resulting graph then overlays the current predicted trajectory for Belgium against the benchmark trajectory. If both curves coincide, this implies the outbreak has followed a very similar trajectory in both countries, correcting for cross-country differences such as population size, testing policies, total number of cases/deaths.

The results are informative: if Belgium has reached its first peak, the number of days from the onset to the peak of the outbreak is around 40 days, longer than China (around 25-30 days). Second, it might be that Belgium lingers longer around the peak than China. This might signal a slower trajectory of the disease in Belgium compared to China, and hence also a slower recovery. Third, we might see the potential onset of a second wave for China. However, we underline again that these trajectories are shaped by policies and human adherence to these policies: our behaviour impacts the curve, not the other way around...

We compare cases and deaths over time as the outbreak evolves, and we re-estimate, fit and update these curves daily.

{% include plots/daily-update-2020-04-17/2020-04-17-MA_ln_share_cases-midpoint-Belgium.html %}

<p style="text-align: center; font-style: italic;">Figure 5: Epicurves: an estimated evolution of the epidemic waves.</p>

### 2. Daily updates, world and EU28 <a name="cap2"></a>

[*Back to Table of Contents*](#tbc)

-------------------------------------

#### 2.1 Number of cases and deaths

We continue with the number of cases and deaths for the 10 most infected countries in the world and the EU28.[^6]

[^6]: Some of these graphs are similar to the popular graphs in the [Financial Times](https://www.ft.com/coronavirus-latest).

Figure 6 shows the total number of cases over time. The country with the most cases is United States of America with 671,331 total confirmed cases. Second is Spain with 182,816 cases, and Italy follows, with 168,941 cases. The Figure reports the total number of cases (in log scale), since the 100th confirmed case within that country. In the initial outbreak phase, the epidemic [spreads exponentially](https://medium.com/data-for-science/epidemic-modeling-101-or-why-your-covid19-exponential-fits-are-wrong-97aa50c55f8), but tapers off as the epidemic evolves, due to constraints on the spread of the virus (e.g. policies, geography, density).
Synchronizing dates since the 100th confirmed case allows to compare the speed and evolution of the epidemic across countries. China has been stabilizing since the end of February, signalling that its first peak has passed. The longer this curve stays flat, the more hopeful China can be.
However, the arrival of new domestic cases signal the possible onset of a second wave. The curve for several countries tapers off, but other countries are still in the onset, facing close to exponential growth rates.

Some additional notes. First, there is a large jump in deaths for the USA on April 16, with over 3500 reported deaths in one day. This could signal the onset of a worse trajectory for the USA, than the previous path it was following. Second, while Sweden has been viewed as a good example of a more laissez-faire policy with lower case and death rates than other EU countries, there has been a jump to a higher rate over the last few days. We will closely monitor the discrete jumps of these countries over the next days. Finally, there is a jump for deaths in China on April 17, due to lagged reported deaths that are now included in the numbers.

When looking at the EU28, the country with the most cases is Spain with 182,816 total confirmed cases. Second is Italy, with 168,941 confirmed cases, and Germany follows, with 133,830 cases. It's worth noting that Sweden's infection rate has decreased significantly since around the 9th day after the 100th confirmed case, while having a [more lenient policy](https://www.forbes.com/sites/davidnikel/2020/03/30/why-swedens-coronavirus-approach-is-so-different-from-others/#538677cb562b).  

The Figure also reports the total number of deaths since the 10th death. As noted in the introduction, both the number of cases and deaths are prone to several sources of non-random measurement error. However, we expect the measurement error to be smaller for the reported number of deaths. As of today, the country with the most deaths is United States of America, with 33,284 deaths. Second is Italy, with 22,172 deaths, and Spain follows, with 19,130 deaths. These top 3 countries account for 0.51% of all deaths worldwide. Again, we see that China has stabilized for now, with around 3,500 deaths. We repeat the graph for the 10 highest mortality countries in the EU28. The EU28 country with the most deaths is Italy, with 22,172 deaths. Second is Spain, with 19,130 deaths, and France follows, with 17,920 deaths.

{% include plots/daily-update-2020-04-17/2020-04-17-ln_cum_cases-ln_cum_deaths-after_10th.html %}

<p style="text-align: center; font-style: italic;">Figure 6: Evolution of cases and deaths for the world and EU28 countries (top 10).</p>

Absolute numbers are a key statistic in the onset of the epidemic, as they relate to the number of people infected from one patient. Moreover, in standard S(E)IR models, in the onset of an outbreak, the predicted number of infected people rises almost identical in countries with vastly different population sizes. As the epidemic tapers off however, these numbers will converge to a fraction of the population being infected or deceased.[^7] In Figure 7, we plot the number of cases and deaths for these countries, as a percentage of the population. For cases, we report since the 0,01% case, for mortality, since the 0,001% death. 

[^7]: The first few weeks in the outbreak, higher per-capita numbers mostly imply smaller countries, not different policies or growth rates.

As of today, the EU28 has an average infection rate of 0.170%, and a mortality rate of 0.017%, calculated as the total number of cases/deaths over the EU28 population. This is still far off the [projections](https://www.hsph.harvard.edu/news/hsph-in-the-news/the-latest-on-the-coronavirus/) of 30-70% of adult world population ultimately being infected.  There are at least four hypotheses: (i) real infection rates are orders of magnitude larger than reported ones. If we are at the end of the epidemic, this implies real infection rates are around 100-300 times larger than currently reported. (ii) the epidemic is only in its onset, and we expect to reach higher infection rates.
(iii) we are reaching the end of the epidemic, and infection rates are much lower than projected. Given the growth rates and our estimates for epidemic curves, we believe this scenario is not probable at this moment. (iv) flattening-the-curve policies lower the speed with which the epidemic rages. It is not clear yet whether these policies affect the total infection rate at the end of the epidemic. With such policies in place, the share of infected population can grow at a lower rate but over a longer period.

{% include plots/daily-update-2020-04-17/2020-04-17-cum_cases_population-cum_deaths_population-after_0.001.html %}

<p style="text-align: center; font-style: italic;">Figure 7: Evolution of cases and deaths for the world and EU28 countries, as a fraction of the population (top 10).</p>

Countries around the world have taken several measures to slow down the speed of the epidemic in their country. The strength and timing of these policies however, varies significantly across countries.
Figure 8 shows an index of the strength of measures taken, and at what moment in the outbreak, expressed as the total number of deaths at that moment. The index is [The Oxford COVID-19 Government Response Tracker](https://www.bsg.ox.ac.uk/research/research-projects/oxford-covid-19-government-response-tracker),[^8] ranges between 0 (no policy) to 100 (maximum measures) and combines 13 indicators of government responses, including school closures, travel bans, and fiscal or monetary measures. There is a clear difference between both the speed with which countries implemented particular policies, as well as the severity of the measures taken as of today. For example, while Belgium has raised its measures rapidly and drastically, the UK has been slower and more lenient. 

[^8]: Hale, Thomas, Sam Webster, Anna Petherick, Toby Phillips, and Beatriz Kira (2020). Oxford COVID-19 Government Response Tracker, Blavatnik School of Government. Data use policy: Creative Commons Attribution CC BY standard.

{% include plots/daily-update-2020-04-17/2020-04-17-policy.html %}

<p style="text-align: center; font-style: italic;">Figure 8: Evolution of policy measures for world countries (top 10 by deaths).</p>

#### 2.2 Growth rates

Next, in Figure 9 we plot the evolution of growth rates of the number of cases and deaths, since the 100th case and the 10th death. Growth rates are expressed in percentage changes from date *t-1* to *t*. We take a 3-day simple moving average to account for strong fluctuations from e.g. reporting lags within countries.

Each country wants to see its growth rate going to zero as soon as possible. China has seen close to zero growth rates for a series of days now. Two things are worth noting. First, the slopes, or decreases in growth rates, are not the same across countries. Second, even smoothed by a 3-day moving average, these growth rates are not monotonically decreasing.

This might be partially due to temporal new outbursts of the virus within countries, or to increased testing policies.[^9]

[^9]: Approximating these growth rates with a 4th-order polynomial fit (not shown) also shows these non-monotonicities.

{% include plots/daily-update-2020-04-17/2020-04-17-MA_cases-MA_deaths-after_100th.html %}

<p style="text-align: center; font-style: italic;">Figure 9: Evolution of growth rates of cases and deaths for the world and the EU28 (top 10).</p>

#### 2.3 Epicurves, world and EU28

We conclude with an estimate of real-time epidemic curves for cases and deaths, for both the top 10 world countries and the EU in Figure 10. These initial projections suggest that China has experienced a turning point at around 25-30 days. Most other countries however, seem to experience a slower reach to the peak, roughly around 40 days, under the assumption that the calculated peaks in the daily updated data are currently reached.

For those countries that have reached a peak, the decline seems to be slower than that of China.

{% include plots/daily-update-2020-04-17/2020-04-17-MA_ln_share_cases-MA_ln_share_deaths-midpoint.html %}

<p style="text-align: center; font-style: italic;">Figure 10: Real-time epicurves.</p>

-------------------------------------

We are back with updated numbers tomorrow.

In the mean time, stay safe, and take care of yourself and of others.

Federico and Glenn.

-------------------------------------
