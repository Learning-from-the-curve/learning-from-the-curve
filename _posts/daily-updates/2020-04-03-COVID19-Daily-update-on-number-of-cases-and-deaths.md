---
layout: post
title: COVID19 - Daily update on number of cases and deaths
date: 2020-04-03 11:54:00 +0100
category: daily-updates
---
[Federico Gallina](https://www.ulb.be/fr/federico-gallina) [(ECARES, ULB)](https://ecares.ulb.be), [Glenn Magerman (ECARES, ULB)](http://www.glennmagerman.com), and the [“Learning from the curve” team](https://github.com/Learning-from-the-curve).

### 1. Introduction

-------------------------------------

This article presents daily numbers and insights on COVID infections. It analyzes the number of cases and deaths for the most infected countries in the world and the EU, and then presents more detailed statistics for Belgium. 
By combining several statistics, we aim to better understand where we are in the trajectory of the epidemic, without making any extrapolations (e.g. typical exponential fits). 
As the epidemic evolves, we expect infection rates and mortality rates to decrease and stabilize, and go to zero at the end of (the first wave of) the outbreak.
We also construct a real-time epidemic curve, using China as a benchmark. A real epidemic curve can only be provided at the end of the epidemic, but as daily data comes in, the curve gets updated and converges to the real epidemic curve at the end.

Today's key numbers:

- Global: 1,000,249 total cases, and 51,515 deaths in 203 countries with reported COVID-19 cases.

- EU28: 475,687, and 35,816 deaths.

- Belgium: V total cases, W total hospitalised, X in intensive care, Y deceased, and Z recovered.
<!--more-->

**Note 1**: We report statistics based on the number of confirmed COVID cases and deaths. These world-wide daily numbers are informative and the best available cross-country. However, they are not perfect. 
First, the number of infected people is certainly much higher than reported. One reason is that not everyone is, nor can be, tested in every country. Specialists estimate the "dark number" (the real number of infected people not captured in the statistics) to be 10 or 100 times larger than recorded number. 
Second, there are cross-country differences in the number of cases due to differences in testing policies. Some countries have implemented aggressive testing, random sampling, or blood tests, while others only test hospitalized people and/or with severe symptoms. This naturally raises confirmed cases for the countries that test more extensively. 
Third, the number of cases does not convey the severity of the disease by case. 
Finally, for deaths, there can be over-reporting (comorbidity as cause of death, or other mortalities statistically allocated to COVID mortality), underreporting (no confirmed COVID diagnosis or deaths outside hospitals (e.g. in retirement homes or at home) not counted) and lagged reporting (how long does it take for the numbers to go into the statistics?). There can be a [large amount of heterogeneity in this under/over-reporting](https://www.bbc.com/future/article/20200401-coronavirus-why-death-and-mortality-rates-differ) across countries. 
We take these numbers and these cautions as given.

**Note 2**: This article is of a  descriptive nature: it does not make any policy or normative statements. Please see [Learning from the curve](https://github.com/Learning-from-the-curve) for other initiatives.

**Note 3**: Analysis will be evolving as the project continues. Feedback, suggestions, and/or critiques are highly welcomed.

**Data sources:** 

- COVID data by country around the world from [ECDC](https://www.ecdc.europa.eu/en/publications-data/download-todays-data-geographic-distribution-covid-19-cases-worldwide).

- Country population data from [UN](https://population.un.org/wpp/Download/Standard/CSV). 

- Detailed COVID data for Belgium from [Epistat](https://epistat.wiv-isp.be/covid/). 

- Vector maps for Belgium from [geo.be](geo.be).

### 2. Number of cases

-------------------------------------

#### 2.1 Number of cases

We start with reporting the number of cases for the 10 most infected countries in the world and the EU28.

Figure 1 shows the total number of cases over time.[^1]

[^1]:You can use the dropdown menu to select variants of the same curve. All graphs are interactive, and allow for a sub-selection of countries.

The country with the most cases is United States of America with 245,540 total confirmed cases. Second is Italy, with 115,242 confirmed cases, and Spain follows, with 110,238 cases.

The first tab reports the total number of cases (in log scale), since the 100th confirmed case within that country. Synchronizing dates since the 100th confirmed case allows to compare the speed of the epidemic across countries.

China has been stabilizing since the end of February, signalling that the (first ?) peak has passed. Some countries show a decline in the increase of the number of new daily cases, hopefully pointing to passing a peak, or at least a stabilization of the number of infected people.
However, many countries are still facing exponential growth rates (linear in logs), signalling those countries face the onset of the pandemic. The second tab shows the same total number of cases by date, in levels.

We repeat the graph for the 10 most infected countries in the EU28 in tabs 3 and 4. 
The EU28 country with the most cases is Italy with 115,242 total confirmed cases. Second is Spain, with 110,238 confirmed cases, and Germany follows, with 73,522 cases.

{% include plots/daily-update-2020-04-03/2020-04-03-ln_cum_cases-after_100th.html %}
{% include plots/daily-update-2020-04-03/2020-04-03-cases_cum-dateRep.html %}
*Figure 1: Total cases.*

#### 2.2 Number of cases per million population

Figure 2 shows the total number of cases, per million population, since the 100th case per million people for these top 10 countries. Absolute numbers are a key statistic in the onset of the epidemic, as they relate to the number of people infected from one patient. 
Moreover, in standard S(E)IR models, the number of infected people rises almost identical in countries with vastly different population sizes. However, as the epidemic evolves over time and reaches a steady state, a certain fraction of the population will be infected. 
Therefore, we also report the number of cases correcting for country size. A significant part of the friction the virus encounters, and which in turn affects its growth rate, is country-specific: policy measures, geographic dispersion, population density etc.[^2]

[^2]: E.g. Belgium can never reach the same theoretical maximum number of infected people as the USA. Additionally, there will be within-country regional differences that affect both absolute and relative numbers (e.g. China is not affected homogeneously in all provinces). 

Figure 2 shows these numbers for the 10 most infected countries in the world and for the top 10 EU28 countries.

As of today, the country with the largest confirmed infection rate is Vatican City, with an infection rate of around 0.751%.
This is still far off the [projections](https://www.hsph.harvard.edu/news/hsph-in-the-news/the-latest-on-the-coronavirus/) of 30-70% of adult world population ultimately being infected. 
There are at least four plausible scenarios:

1. real infection rates are orders of magnitude larger than reported ones. Taking Spain as a benchmark, and assuming countries are at the top of the epidemic, this implies real infection rates are around 100-300 times larger than currently reported. One related observation is that many infected people are actually asymptomatic, with a high probability of not being tested.

2. the epidemic is only in its onset, and we expect to reach higher infection rates. Given that most countries have not passed their peak yet, this is a plausible scenario.

3. we are reaching the end of the epidemic, and infection rates are much lower than previously projected. Given the growth rates and our initial estimates for epidemic curves discussed below, we believe this scenario is not highly probable at this moment.

4. the projections of 30-70% global infection rates relate to counterfactual scenarios where no policy action is taken. This is probably the most relevant scenario, and hopefully the costly but necessary measures contribute to a large extent to the lower numbers we see. However, flattening the curve policies also imply that the epidemic is spread more over time, so number can increase for a longer period.

{% include plots/daily-update-2020-04-03/2020-04-03-ln_cases_per_mln_cum-after_100th_per_mln.html %}
*Figure 2: Total cases, per million population.*

#### 2.3 Growth rate of the number of cases

Next, we plot the evolution of growth rates of the number of cases.
Growth rates are expressed in percentage changes from date *t-1* to *t*.[^3]

[^3]: The growth rate on absolute numbers is identical to one calculated as cases per million inhabitants.
We take a 3-day simple moving average to account for strong fluctuations from e.g. reporting lags within countries. 
Each country wants to see this growth rate going to zero as soon as possible. China has officially (close to) reached that state.

Two things are worth noting. 
First, the slopes, or decreases in growth rates, are not the same across countries. This implies some countries will get to zero growth faster than others. 
Second, even smoothed by a moving average, these growth rates are not monotonically decreasing. This might be partially due to temporal new outbursts of the virus within countries, or to increased testing policies.

{% include plots/daily-update-2020-04-03/2020-04-03-MA_cases-after_100th.html %}
*Figure 3: Growth rates, number of cases.*

### 3. Number of deaths

-------------------------------------

#### 3.1 Number of deaths

As noted in the introduction, the number of cases is prone to several sources of non-random measurement error. While measurement error also exists for the number of deaths, this number draws a clearer (but morbid) picture. 

Figure 4 shows the total number of deaths for the top 10 countries with the deadliest outbreak over time.
As of today, the country with the most deaths is Italy, with 13,917 deaths.
Second is Spain, with 10,003 deaths, and United States of America follows, with 6,053 deaths.

The first tab plots the total number of deaths (in log scale) since the 10th death.
Again, we see that China has stabilized, with around 3,500 deaths.
Since the second half of February, China has been overtaken by Italy and Spain.
Since April 1, the USA is the country with the third highest number of deaths due to COVID. 

The second tab shows the same total number of deaths by date, in levels.

We repeat the graph for the 10 highest mortality countries in the EU28 in tabs 3 and 4. 
The EU28 country with the most deaths is Italy with 13,917 deaths. Second is Spain, with 10,003, and France follows, with 4,503 deaths.

{% include plots/daily-update-2020-04-03/2020-04-03-ln_cum_deaths-after_10th.html %}
{% include plots/daily-update-2020-04-03/2020-04-03-deaths_cum-dateRep.html %}
*Figure 4: Total deaths.*

#### 3.2 Number of cases per million population

Figure 5 shows the total number of deaths, per million population, since the 10th death per million people for these top 10 countries.
Here we see most countries being on a similar trajectory as Italy.

{% include plots/daily-update-2020-04-03/2020-04-03-ln_deaths_per_mln_cum-after_10th_per_mln.html %}
*Figure 5: Total deaths, per million population.*

#### 3.3 Growth rate of the number of deaths

We plot the evolution of growth rates of the number of deaths in Figure 6.

{% include plots/daily-update-2020-04-03/2020-04-03-MA_deaths-after_10th.html %}
*Figure 6: Growth rates, number of deaths.*

### 4. Mortality and case-fatality rates

-------------------------------------

We continue with two measures that are highly imperfect, but serve as a benchmark for longer time horizons in tracking the epidemic spread.

The first is the mortality rate, or the number of people dying from COVID as a fraction of total population.
For the 10 countries with the highest current mortality rates in the world (and EU28), this is reported in Figure 7.

Since population is (nearly) fixed, this number will increase monotonically over time and reach a constant value at the end of the epidemic. Various estimates range between 1% and 8%.

This measure deserves a series of remarks.
First, it is hard to evaluate the cause of death due to COVID in the presence of comorbidity or other mortalities statistically allocated to COVID mortality. One way to look at these numbers is a mortality rate due directly or indirectly to COVID, either as a direct cause of death, comorbidity, or e.g. other causes of death but due to the overload of the health system).
Second, there are signs of under-reporting (no confirmed COVID diagnosis or deaths outside hospitals (e.g. in retirement homes or at home) not counted) and lagged reporting (how long does it take for the numbers to go into the statistics?). 
Third, there can be a [large amount of heterogeneity in this under/over-reporting](https://www.bbc.com/future/article/20200401-coronavirus-why-death-and-mortality-rates-differ) across countries. Therefore, the rate within countries is more informative than the cross-country comparison of the levels of these rates.
Finally, these mortality rates are totals over the whole population. By demographics, mortality rates are much higher for older people, and people with pre-existing conditions such as heart or diseases, and diabetes. However, we do not have deaths by demographics in the ECDC data, so we cannot further investigate this here. For Belgium, we exploit more detailed data and match these against life tables.

The second measure is the case-fatality rate (CFR), which reports the number of people dying as a fraction of the infected population. This number is always higher than the mortality rate, as it is a ratio over a strict subset of the population (confirmed infected cases).
This measure also deserves important critiques.
First, in real time, estimates of the CFR can be biased upwards by under-reporting of cases, and downwards by failure to account for the delay from confirmation to death.
Second, the CFR is surely biased upwards since the true number of infected people is much larger than what is reported. Therefore, we focus on the within-country evolution of these rates, rather than comparing across countries, or even the numbers themselves at face value.

{% include plots/daily-update-2020-04-03/2020-04-03-fatality_rate-mortality_rate-after_10th.html %}
*Figure 7: Growth rates, number of deaths.*

### 5. Estimated epidemic curves

-------------------------------------
We conclude with an estimate of real-time epidemic curves for cases and deaths, for both the top 10 world countries and the EU.
It reports the fraction of total cases/deaths over the span of the disease. 
When anyone is talking about "flattening the curve", this is THE curve.

Comparing outbreaks over time or across countries helps to better understand the evolution in the future or in other countries (conditional on other factors).
These curves provide information on the speed (growth rate by day) and severity (number of cases/deaths) of the COVID epidemic, and are important blueprints to benchmark further outbreaks of the disease in the future.

The drawback is that epicurves are only available at the end of the disease. 
At that moment, we will have the full distribution of cases/deaths over time per country (conditional on all the remarks on the measurement of cases and deaths).
Some examples of epicurves for [Mers-Cov](https://www.nature.com/articles/s41598-019-43586-9), [SARS](https://www.who.int/csr/sars/epicurve/epiindex/en/index1.html), [influenza in Canada](https://onlinelibrary.wiley.com/doi/full/10.1111/j.1750-2659.2010.00154.x) and [influenza in Belgium](https://epistat.wiv-isp.be/influenza/). 

Still, we go ahead and construct epicurves for different countries as the disease evolves, as follows. 
First, under the assumption that China has completed the (first) outbreak of the disease, we use China as a benchmark epicurve.
Second, we compare cases and deaths for several countries over time as their outbreak evolves, and we update the curves daily. At the end of the outbreak for a country, the real-time epicurve coincides with the true epicurve. 
As more countries complete the outbreak cycle, they contribute to the benchmark of "the" epicurve for COVID for other countries still completing their cycles. In other words, we keep an eye on this as more countries pass the first peak and this solidifies the structure of the general epicurve.
Third, to compare across countries, the epicurves are centered around a turning point, where the new number of cases or deaths at a given time is maximal. 
Since it is never certain what the maximum is until at the end of the outbreak, we estimate the turning point based on the growth rate of cases/ deaths. In particular, we predict future growth rates using a 4th degree polynomial on current growth rates presented above.
The predicted turning point is then used to calibrate the graph and to compare the curve to the benchmark (China).
Fourth, the y-axis is reported in the fraction of cases/deaths over the length of the outbreak. Together with the turning point, his allows us to compare epicurves across countries. Again, for the real-time epicurves, we calculate the future number of cases based on predicted growth rates to calibrate the y-axis.
Our approach is a naive and brute-force method to construct these real-time epicurves. There are much more refined methods available, such as [Bayesian estimation](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0002185).

Finally, we strongly underline that it is highly probable that additional waves might arrive within a country. As of today, it is not certain that China has finished its full cycle, or that there are seasonal cycles coming up. 
Additionally, these patterns take as given the current policy measures. Too early lifting of measures can and will result in a direct second wave. 
These figures do not serve as any policy measure in any way. They only serve to get an estimate of the epicurves in real time, instead of waiting until the end of the outbreak.

{% include plots/daily-update-2020-04-03/2020-04-03-MA_ln_share_deaths-MA_ln_share_cases-midpoint.html %}
*Figure 8: Real-time epicurves.*
