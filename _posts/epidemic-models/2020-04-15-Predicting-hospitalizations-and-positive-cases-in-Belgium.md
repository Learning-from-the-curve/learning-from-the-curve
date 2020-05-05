---
layout: post
title: Predicting hospitalizations and positive cases in Belgium
date: 2020-04-15 11:00:00 +0100
category: epidemic-models
---
[Vincenzo Verardi](https://directory.unamur.be/staff/vverardi) (UNAMUR-CRED, FNRS, ULB).

**Table of Contents**:<a name="tbc"></a>

- [Predicting hospitalizations and positive cases in Belgium <a name="cap1"></a>](#predicting-hospitalizations-and-positive-cases-in-belgium)

### Predicting hospitalizations and positive cases in Belgium <a name="cap1"></a>

[*Back to Table of Contents*](#tbc)

-------------------------------------

As explained in a previous post [COVID-SIR](https://learning-from-the-curve.netlify.app/epidemic-models/2020/04/13/COVID-SIR.html#cap1), epidemiologists have very performant models to understand the evolution of an epidemic. Probably the best known is the so-called

$$ SIR: \bf{Susceptible} \rightarrow \bf{Infected} \rightarrow \bf{Removed} $$

that allows to easily model the evolution of an epidemic relying on the reproduction number \\(R\_0\\) and the infectious period of a pathogen. A great epidemic calculator is freely available at [http://gabgoh.github.io/COVID/index.html](http://gabgoh.github.io/COVID/index.html). This is a wonderful tool to simulate how the Covid-19 epidemic might spread according to the characteristics of a population. The reproduction number \\(R\_0\\) is the average number of infections produced by a single case in a population where everyone is susceptible to be contaminated. This has been estimated to be around 2.2 for the Covid-19 pandemic. Thomas Pueyo has illustrated how this value could cause dramatic outcomes in his article [Coronavirus: The Hammer and the Dance](https://medium.com/@tomaspueyo/coronavirus-the-hammer-and-the-dance-be9337092b56) if nothing is done.<!--more-->
The effective reproduction number \\(R\_e\\) (i.e. the product of \\(R\_0\\) and of the fraction of the population that is susceptible of being contaminated) can be reduced thanks to social distancing. By increasing social distances, the share of the population susceptible of being contaminated decreases and so does \\(R\_e\\). As soon as \\(R\_e\\) becomes smaller than one, the epidemic will start fading away or at least slowing down. To summarize, thanks to the increase in social distancing, the spread of epidemic can be slowed, and an overwhelming of the health sector can hopefully be avoided. After an exponential growth in the number of cases in the beginning of the epidemic, an inflection point of the curve could be reached much earlier than if nothing was done. A very simple and naïve model to estimate the total number of contaminated individuals could then be used to have a broad idea of how the epidemic is evolving. This would be to look for the sigmoidal (\\(S\\)-looking) function relating the number of observed cases to time, that better approximates the observed cases. Probably the simplest candidate is the *logistic function* that can be written as:

$$ Cases(t) = \frac{m}{1 + \exp{(-s(t-t_{\inf}))}} $$

where \\(m\\) is the asymptote (maximum), \\(t\_{inf}\\) is the inflection point (the moment of maximal growth rate in the number of cases) and \\(s\\) is the scale (related to the steepness of the curve). Ideally one would like to predict how many individuals will be affected in any period and understand if, at the end of the epidemic, the number of cases will have been enough to reach the so-called herding or collective immunity.

For the very specific case of Covid-19, only part of the infected individuals is identified through testing (at least for now) and many individuals that have milder symptoms go unnoticed. With the increasing number of tests performed over time, it is hence questionable to do a time-series analysis using the number of positive cases as these will most likely increase due to an increase in testing (even if the epidemic slows down). Furthermore, any international comparison would make no sense as the number of tests performed changes dramatically from country to country and so does the identified number of positive cases.

What we suggest to do is to rely on the number of hospitalized patients, which is probably more informative. Even if the number will (fortunately) not coincide with the total number of positive cases, the shape of the prediction function should be similar. It could then be possible to estimate the total number of cases (from the predicted number of hospitalizations) doing a simple proportion (relying on the percentage of hospitalized patients amongst the infected ones as estimated in the literature). The Maximum Likelihood estimation (broadly speaking the most likely model given the data available) for the logistic regression is easy to fit. In the graph below we present the observed number of hospitalizations (dots), the best fitting logistic curve in blue (representing the expected cases) and its derivative (representing the expected change in the number of hospitalizations) in orange.

**Click on the legend to add or remove lines**

{% include plots/Epidemic-Models-2020-04-15/Belgium.html%}\\
The logistic fit is unfortunately not fully appropriate for these data especially in case of existence of public interventions that shape the evolution of the epidemic. Such an intervention was implemented in Belgium the 19th of March 2020 when a lockdown was ordered. This created an artificial maximum in the number of infections and the decline from that point on has been slower than the raise in infections. This skewness in the distribution of infections was expected as can be easily seen in the \\(SIR\\) graph presented in a previous post and reproduced here below (for a smaller time range).

**Click on the legend to add or remove lines**

{% include plots/Epidemic-Models-2020-04-15/Lockdown.html%}\\
This asymmetry can be modelled (inter alia) using a skewed logistic model where:

$$ Cases(t) = \frac{m}{(1 + \exp{(-s(t-t_{\inf}))}^{\alpha}} $$

Where \\(\\alpha\\) is the skewness parameter.

**Click on the legend to add or remove lines**

{% include plots/Epidemic-Models-2020-04-15/Belgium_SL.html%}\\
The fit is better than that of the standard logistic and the predicted number of hospitalizations in Belgium is slightly higher. Indeed the skew-logit model predicts (ceteris paribus) that 15000 individuals will have been hospitalized while the standard logit estimates about 12500. It is generally accepted that 10% to 20% of the infected individuals need hospitalization. One could therefore extrapolate the total number of infected patients easily. In the graph below we present the total number of estimated cases (assuming that 10% of total infected individuals are hospitalized).

**Click on the legend to add or remove lines**

{% include plots/Epidemic-Models-2020-04-15/Belgium_POS.html%}\\
Thanks to the public intervention (and if the lockdown is maintained till the end of the epidemic), the number of final cases is estimated to be around 150000 which translates into around 6000 deaths. Naturally, the lockdown cannot be maintained forever, and this estimation is certainly a lower bound. Possible exit strategies should be studied to find the optimal deconfinement. The age structure of the population should play a central role in the analysis given the specificities of this specific virus, particularly lethal for the elderly. We will discuss this point in a future post devoted to exit strategies. In that occasion we will present a more complete epidemic model that includes age classes, symptomatic and asymptomatic cases, location specific interactions and many more features.
