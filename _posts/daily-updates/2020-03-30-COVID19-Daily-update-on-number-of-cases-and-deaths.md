---
layout: post
title: COVID19 - Daily update on number of cases and deaths
date: 2020-03-30 12:00:00 +0100
category: daily-updates
---
[Prof. Dr. Glenn Magerman (ECARES, ULB)](http://www.glennmagerman.com) and the [“Learning from the curve” team](https://github.com/Learning-from-the-curve).

#### 1. Introduction

-------------------------------------

The outbreak of the coronavirus was first identified in Wuhan, Hubei, China in December 2019, and has been categorized as a pandemic by the WHO on March 11, 2020. See also [here](https://en.wikipedia.org/wiki/2019–20_coronavirus_pandemic) for more information. Since then, the virus has spread rapidly over almost all countries worldwide.

As of today, there are 714964 total cases, 33572 deaths and 195 countries with reported COVID cases.

<!--more-->

This article presents insights in the daily reports on COVID infections worldwide. It analyzes the number of cases and deaths for the most infected countries in the world, the EU, and Belgium respectively. Numbers are always reported in three ways.

- First, we report by calendar date. This provides a snapshot of the current severity of the pandemic across countries.

- Second, we report since the 100th case or death. This allows to compare outbreaks across countries, and generates insights in the different trajectories of those countries.

- Third, we report since the 100th case or death per million inhabitants. This accounts for different sizes of countries and the relative severity by country.

**Note 1:** None of the reported numbers are perfect. For one, not everyone is tested in every country. Specialists estimate the real number of infected people to be 10 or 100 times larger than recorded. Second, some countries have implemented more aggressive testing, while other countries only test those with severe symptoms. This inadvertly raises confirmed cases for the countries that test more extensively. Third, for deaths, there is potential comorbidity, or other factors that might lead to death. It is hard to disentangle the exact cause of death from COVID or comorbidity. In another project, we want to discuss what would be ideal variables to measure the outbreak, and what we can do given the data that is available. Here, we take the numbers, and this observation of data as given.

**Note 2:** Calculations such as the case-fatality rate are extremely noisy if the number of cases is under- or misreported with possibly orders of magnitude difference. We don’t calculate these statistics.

**Note 3:** Analysis will be evolving as the project continues. Any feedback, suggestions, critiques, are highly welcome.

**Sources:**

- COVID case data comes from [ECDC](https://www.ecdc.europa.eu/en/publications-data/download-todays-data-geographic-distribution-covid-19-cases-worldwide).

- Population data comes from [UN](https://population.un.org/wpp/Download/Standard/CSV).

#### 2. Global overview

-------------------------------------

We start by analyzing the top 10 infected countries globally.

##### 2.1 Cases

-------------------------------------

Figure 1 shows the number of confirmed cases for the top 10 countries as of today. While China was the first epicenter, and Europe the second, since March 27, 2020, the USA has overtaken both China and Italy in terms of the number of cases. The number one country is Andorra, with 143025 total confirmed cases. Second is Andorra, with 97689 confirmed cases, and Andorra follows, with 82463 cases.

![Figure 1: Total cases by date, global top 10.]()

When plotting the number of cases startingf from the date of the 100th case in Figure 2, we see how fast the number of confirmed cases increases, correcting for the different times of the outbreak in different countries. Here we see that the spread is faster than China in USA and Spain

![Figure 2: Total cases since 100th case, global top 10.]()

Absolute numbers might be misleading, since the USA has a population of around 300 million inhabitants, versus 10 million in Belgium or 60 million in Italy. We therefore also account for the population size of countries, by plotting the number of cases per million inhabitants in Figure 3. We synchronize countries based on the 100th case per million inhabitants. Here, we see that countries such as Germany, Spain and Switzerland actually have faster infection rates per capita than Italy. In these countries, confirmed infections are currently in the range of 0.15-0.2% of the population.

![Figure 3: Total cases per million since 100th case per million, global top 10.]()

##### 2.2 Deaths

-------------------------------------

Figure 4 shows the number of deads for the top 10 countries with the deadliest outbreak.

The number one country is Andorra, with 10781 total confirmed deaths. Second is Andorra, with 6528 confirmed cases, followed by Andorra, with 3311 deaths. However, USA will shortly overtake China in the number of deaths.

![Figure 4: Total deaths by date, global top 10.]()

In Figure 5, we align the total numbers starting from the 10 death in each country.

![Figure 5: Total deaths since 10th death, global top 10.]()

In Figure 6, we account for country size, and plot the total number of deaths per million, aligned from the 10th death per million.

![Figure 6: Total deaths per million since 10th death per million, global top 10.]()
