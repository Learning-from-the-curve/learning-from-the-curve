---
layout: post
title: COVID19 - Daily update on number of cases and deaths
date: 2020-03-28 15:45:00 +0100
authors: Glenn Magerman
category: daily-updates
---
[Prof. Dr. Glenn Magerman (ECARES, ULB)](http://www.glennmagerman.com) and the [“Learning from the curve” team](https://github.com/Learning-from-the-curve).

#### 1. Number of reported cases, globally

-------------------------------------

While the pandemic started in the province of Hubei, China, the virus has spread over almost all countries. Since two weeks, Europe has been the epicenter of the pandemic, with several countries seeing a rapid incresase in both confirmed cases and deaths. However, since this week, there is the increased risk that the USA will become the next epicenter.

<!--more-->

We start by evaluating the 10 most hit countries as of today. Figure 1 shows the number of confirmed cases for the top 10 countries on March 27, 2020. While China had the most confirmed cases until yesterday, the USA overtook both Italy and China. Spain and Germany are following.

![](/assets/images/daily-updates/2020-03-28/cumcases_byday_global_top10.svg){: .mx-auto .d-block }

Figure 1: Cumulative number of cases by date, global top 10.

The difference in growth rates becomes clearer when we plot the number of cases starting from the date the 100th case if confirmed in Figure 2. Both aggressive testing and increase number of infections create more confirmed cases. Again, USA, Italy and Spain show very rapid increases.

![](/assets/images/daily-updates/2020-03-28/cumcases_post100_global_top10.svg){: .mx-auto .d-block }

Figure 2: Cumulative number of cases since the 100th case, global top 10.

Absolute numbers might be misleading here, since the USA has a population of around 300 million inhabitants, versus 10 million in Belgium or 60 million in Italy. We therefore also account for the population size of countries, by plotting the number of cases per million inhabitants in Figure 3. We synchronize countries based on the 100th case per million inhabitants. Here, we see that countries such as Germany, Spain and Switzerland actually have faster infection rates per capita than Italy.

Note: it’s not completely certain whether the absolute number or relative number matters to estimate the speed of the pandemic. One often used measure, R<sub>0</sub>, captures the average number an infected person infects. It does not say anything however, about the speed with which that happens. Depending on country particularities, the virus will also face capacity constraints on who it can attack, in the form of social distancing, geographic dispersion and population density in particular areas.

![](/assets/images/daily-updates/2020-03-28/cumcases_perMln_post100_global_top10.svg){: .mx-auto .d-block }

Figure 3: Cumulative number of cases per million, global top 10.

#### 2. Number of deaths, globally

-------------------------------------

However, the reported number of cases as a measure has several drawbacks. First, the amount of testing (and reporting) is highly heterogeneous across countries. In no country, every potential patient is tested. Due to a lack of testing materials, many countries restrict testing only to severely ill patients. Second, the quality of testing is very heterogeneous. For instance, to get a good swab, testers have to get the swab stick up to 10cm in the mouth or nose cavity to catch the virus. Many tests therefore can give high false negatives, and double testing is performed. Third, some instances doubt the reporting quality of different countries. For instance in China, there might be incentives to keep 0 domestic infections over the last days. The Chinese national government has now ordered local bureaus to report honestly. Fourth, as shown by a very recent study, patients are in fact most infectuous a few days before showing symptoms (if any). Therefore there is a large time window in which can be tested. Taken together, experts believe the number of confirmed cases to be a factor of 10 to 100 higher in reality. Moreover, some countries rapidly increase testing, generating more confirmed cases.

Therefore, we also consider the number of confirmed COVID deaths for the top 10 in Figure 4. There is a clear difference with the number of reported cases: Italy is the morbid leader, and Spain has also surpassed China. Other countries are rising rapidly, such as France, Iran and the USA. However, the slope for Iran is lower than these of the other high-reporting countries. It’s not clear why.

![](/assets/images/daily-updates/2020-03-28/cumdeaths_byday_global_top10.svg){: .mx-auto .d-block }

Figure 4: Cumulative number of deaths, global top 10.

We repeat the analysis for the number of deaths since the 10th death in Figure 5. Here we see that, compared to Italy, the number of deaths is even increasing much more rapidly for Spain. At this rate, Spain will mourn 8,000 deaths at around day 22, compared to day 30 for Italy.

![](/assets/images/daily-updates/2020-03-28/cumdeaths_post10_global_top10.svg){: .mx-auto .d-block }

Figure 5: Cumulative number of deaths since 10th death, global top 10.

We also calculate the growth rates per million inhabitants in Figure 6.

![](/assets/images/daily-updates/2020-03-28/cumdeaths_perMln_post10_global_top10.svg){: .mx-auto .d-block }

Figure 6: Cumulative number of deaths per million, global top 10.

#### 3. Number of cases, EU28

-------------------------------------

We next describe the evolution of the number of reported cases in the EU28. We document the top 10 in Figure 7. Again, we see the sharp growth of Italy. However, it has been an early country in the outbreak, and we see similar growth rates in other EU countries: e.g. Germany, Spain and France.

![](/assets/images/daily-updates/2020-03-28/cumcases_post100_EU28_top10.svg){: .mx-auto .d-block }

Figure 7: Cumulative number of cases since 100th, EU28 top 10.

Correcting for country size in Figure 8, we see a comparable growth rate to Italy for Belgium and the Netherlands, and even more rapid rates for Germany, Austria and Spain.

![](/assets/images/daily-updates/2020-03-28/cumcases_perMln_post100_EU28_top10.svg){: .mx-auto .d-block }

Figure 8: Cumulative number of cases per million, EU28 top 10.

#### 4. Number of deaths, EU28

-------------------------------------

Finally, we turn to the number of deaths for the top 10 EU28 countries. In Figure 9, we show the growth rates for deaths from the 10th death in that country. Here, we see worrisome growth for Spain, but also France has the same rate as Italy.

![](/assets/images/daily-updates/2020-03-28/cumdeaths_post10_EU28_top10.svg){: .mx-auto .d-block }

Figure 9: Cumulative number of deaths, EU28 top 10.

Comparing trends, and depicting the number of deaths per million inhabitants in Figure 10, we see that in relative terms, more people get infected faster than Italy in Spain and Belgium.

![](/assets/images/daily-updates/2020-03-28/cumdeaths_perMln_post10_EU28_top10.svg){: .mx-auto .d-block }

Figure 10: Cumulative number of deaths per million, EU28 top 10.
