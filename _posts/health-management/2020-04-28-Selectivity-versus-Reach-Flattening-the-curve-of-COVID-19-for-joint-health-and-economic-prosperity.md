---
layout: post
title: 'Selectivity versus Reach: Flattening the curve of COVID-19 for joint health and economic prosperity'
date: 2020-04-28 10:01:00 +0100
category: health-management
---
Dr Jacques Bughin, UN consultant, Solvay Business School ULB, Portulans Institute and G20Y, former Director McKinsey Global Institute, and senior partner McKinsey & Company.

We calibrate a SEIR contagion framework, with an extended transmission rate, \\(R_t\\), that accounts for different classes of infections, and for the effects of risk perception and governement actions on Belgium data. We demonstrate that curbing the COVID-19 pandemic with untargetted social distancing is challenging, requiring to sustain a cut of 50% of contacts on top of creating unknown economic risks. With sufficient specificity (>70%) of tests, a model of selective tracing is likely to be more effective.

**Table of Contents**:<a name="tbc"></a>

1. [Introduction](#cap1)
2. [Conceptual model](#cap2)
3. [Experiments](#cap3)
4. [From reach to selective testing, tracing and enforced quarantine](#cap4)
5. [The new social norm of being traced](#cap5)
6. [References](#cap6)

### 1. Introduction <a name="cap1"></a>

[*Back to Table of Contents*](#tbc)

-------------------------------------

By April 14th, the number of recorded infections by the COVID-19 is being close to pass the bar of 2 million individuals worldwide. The death toll is just below 120,000 deaths, according to Worldometer’s compiled statistics (2020). The current virus, which originated in China, has now spread to more than 200 countries worldwide, leaving virtual no one safe.

It has put hospital systems struggling to cope with the flow of heavy infected cases, as feared by Richard Baldwin in a recent post on Vox (2020). Hospital, human, equipment as well as ICU beds capacity have been under excess demand in a matter of just a few weeks following the outbreak in Wuhan. By end of January, Chinese authorities stimulated the import of many health workers into the city, and managed to build up extra bed capacity in a record time to alleviate the pressure. The health system issue has been apparent as well in Europe, in particular Spain, Northern Italy and France. Major consequences of this disequilibrium are a higher fatality rate and a slower pace of recovery rate of contaminated people than average.[^1] Medical resources are alas witnessing high toll of illness and excessive stress levels (see Day, 2020; Fang, 2020; Bughin, 2020a).

[^1]: Ji et al., 2020, *Potential association between COVID-19 mortality and health-care resource availability*, **The Lancet Global Health, 8(4), p.e 480**.

Accordingly, many countries have taken a radical « suppression » approach by imposing major economic standstill in the hope of flattening the epidemic curve of COVID-19 and spread the demand for care more in line with health system abilities. This suppression strategy went crescendo, first forbidding large crowds meetings (theatres, mega-events, etc). It moved quickly to closing schools and asking people to work remotely, then the went to ask the population to stay home. In general, this suppression strategy is a powerful response to a first wave of an unknown pandemic emerging globally, like the COVID-19. There is emerging evidence, that if containement measures are followed by population, pandemic diffusion may slow (Lin et al., 2020). This also buys time to know more about the still unknown features of the COVID-19, and to work on means to battle it via the discovery of powerful antiviral and vaccines.

The challenge is that the suppression strategy also implies an economic shutdown, with likely large ripple effects if kept too long, and without massive macroeconomic reactions (Gourinchas, 2020). Such ripple effects might be a negative spiral of demand and supply reduction, leading a major economic recession, worldwide. Otherwise stated, the  suppression strategy is not sustainable at term, as it creates a growing conflict between health solidarity and economic prosperity. Furthermore, from a behavioral perspective, it will be very difficult to assume that all segments of population will remain ok of significantly reducing their close contacts for long, especially when today, official statistics suggests that less than 1% of the population is being contaminated by the COVID-19. Further, it is known from past behavioral studies that people have an increasingly bad feeling, of the burden of prolonged quarantines (e.g. Person et al., 2004).

At the end of the day, the fundamental question is to find a more effective model in-between the two extremes of « no » and « full contaiment », while still allowing to flatten the curve before the population becomes immune, either naturally, or through medical support. Here, we shed some light on this issue. We look at the question of containment as the typical media business question of reach versus selectivity. Reach is to to get all people contained, but may be this is costly and ineffective, versus slectivity, where we target or personalize responses more much effectively. One simple way to look at this question in epidemiology is though a look at the drivers of the reproduction rate. By calibrating a model of contagion to Belgian data, we shows that the reach strategy is usually very sensitive to the ability to sustain a reduction of contacts in average, of 50%; while the selective strategy, whereby infected people and its close ties accept a complete quarantine, must have sufficiently powerful test, above 70% specificity to be promising.

Those results are obviously only illustrative; but they signal that a model of more segmented reach and selective strategy might be a more powerful strategy than any extreme. The ultimate evolution might be towards a more selective model indeed as a way to make health and economic prosperity rule converge.

### 2. Conceptual model <a name="cap2"></a>

[*Back to Table of Contents*](#tbc)

-------------------------------------

We rely on a classical SEIR model, but builds a more general form of  the reproduction rate, \\(R_t\\), of the total population through time, consistent with He et al., (2013); or Lin et al., (2020). Hence, equation (1) posits a formulation of \\(R_t\\) that makes more explicit, a set of crucial, drivers of the dynamics of the virus diffusion.

$$ R_t = R_0\times [(1-u_t)d+u_t]\times (r_t\times(1-sr_t)\times(1-\frac{D_t}{N_t})\times \exp{(er)}+(1-r_t)\times b\times (1-s_t)\times(1-\frac{D_t}{N_t})\times \exp{(e)}) $$

Where \\(t\\) is a time period, and \\(R_0\\) is the so-called epidemiologic reproduction rate of the COVID-19 as initiated by Kermack and McKendrick, (1927).

The vector of key parameters, (\\(d, r, s, e, b\\)) are representation of five important drivers of how the coronavirus disease, COVID-19, would diffuse:

- \\(R_0\\) is usually used to define the entire risk of the population infected by the virus, in the limit \\(R_0 \to \infty\\). This result however relies on an uniform distribution of contagious events, while most outbreaks are not shaped by the “average” individuals but possibly by a minority of superspreading events. In particular, the probability of containing an outbreak is significantly lower if there is large heterogeneity in secondary infections, as social spread is weakened across the population (Hebert-Dufresne et al., 2020).  To account for the asymetry of contagion, we hence posit: \\(0 < u < 1\\), where \\(1-u\\) the portion of superspreaders, and \\(d > 1\\) is a multiplicator effect. For instance in the case of a Pareto distribution of infection, \\(u=80%\\) and \\(d=16\\), and thus the term \\([(1-u_t)d+u_t]=4\\), reflecting that the network asymetry reduces the power of spread to the population significantly, for a given \\(R_0\\). We do not know the exact distribution linked to the COVID-19, but we have a glimpse from triangulating from other virus distributions of contagion. Measles infection looks like a Pareto distribution; the top 20% typically contributes like 87% for SARS, while the figure is 93% for HIV (Lloyd Smith et al, 2005). For influenza, the distribution looks more like top 20% makes 50% of the secondary infections (Brauer, 2019).

At the level of influenza, the term \\([(1-u_t)d+u_t]=1.56\\). As typically, one estimates \\(\hat{R_0}\\) from observed diffusion data in early days of the outbreaks, that already embeddes the effect from the distribution asymetry of contagion, such estimate \\(\hat{R_0}\\) suffers from a downward bias. For an estimate \\(\hat{R_0}\\), say of 1.3, the true \\(R_0\\), for influenza, will then be \\(1.3\times 1.56\\), or more like 2. Assume still that one can target the portion (\\(1-u\\)), and get half of them adeqautely identified, and fully isolated (or 10% of population) by time \\(t\\) , then \\([(1-u_t)d+u_t]\\) declines from 1.56 to 1.28, or \\(R_t\\) by 18%. This effect is twice bigger than isolating 10% of any average individual; if the asymetry will be like Pareto, the reduction will then be more like 40%.

- Many countries have been in short supply of testing capacity, while also claiming that tests available in the market to date are suffering from low specificity. Thus, the majority of countries, at the exception of some Asian ones, did limited testing so far. Often, they reallocated the available stock of tests, for those emergency cases showing up at hospitals to sort out ture infected cases from others. We take a view then, of two segments of population, one which is tested and recorded, and another one, which is not tested. Accordingly, we may posit: \\(0 < r < 1\\) where \\(r\\) the portion of recorded infected cases to total cases.

The value of \\(r\\), in practice varies with times. At the outbreak of the virus, it might be close to zero. This is especially true in the case of the COVID-19, where the average combination of incubation and contagion periods may be around 20 extra days. \\(r\\) is also likely increasing with time, as pre-symptomatic cases become ill, and countries build up more testing capacity and test specificity increases. We rely on other scholar attempts to have an idea of the actual range of value for \\(r\\). We have estimated \\(r\\) to be in the range of 10% to 20% by March 20th, for most of European countries after 4 weeks in the pandemic implying that a significant amount of cases have been unrecorded (Bughin, 2020b). Li and colleagues (2020), came to the same conclusions for the case of Wuhan, concluding that those non recorded cases may be responsibile for a rather rapid dissemination of novel coronavirus. A powerful case study is the Italian village of Vo, with 3% by early march of its population infected by the coronavirus, or roughly three weeks after the being the host of « patient zero » in  Italy, and after all the population got tested and strict containments were put in order. This level of contagion implies a true number of infections about roughly 8 times what was recorded in the 11 towns most affected by the outbreak in Italy. A large part of under-reporting is that COVID-19 may high high asymptomatic effect; 50% of the individuals infected, did not get any symptom, in the case of Vo.

- The contagion spreads though physical close contacts, due to the mechanisms of entries of the virus into the respiratory system of individuals. We posit; \\(0 < s(r) <1\\) where \\(s(r)\\) is the portion of reduction in contagious social contacts for (un)recorded contaminations. This reduction is of course a weighted average of actions between different sociodemographic segments—for example, someone in its late thirties, who has a front line sales service jobs, one teenager kid at high school, and a good social life, might have roughly 5 times more contacts than a retired single person of 60 years old, according to our computation. In general, also, older persons’ contacts become only social in a closely tight community setting, making them more at risk, but less contagious given narrow networks, while young adults have all sources of, and all types, of close contacts possible, friends, work, school kiss and drives, concerts, parties, love partners, etc. Most studies of contact estimation suggests that  school and work contacts account for roughly 40% of total contacts, 1/3 extra arises  from community circles, and the balance is from own family (see Kelso et al. 2013).

Getting \\(s\\) larger than 0.5 is however challenging. This is because some work from front lines remain necessary in critical sectors, such as healthcare, equipment manufactruring and food and pharmaceutical services for instance. Those sectors typically amount to  25% to 30% of a developed economy. Citizens are usually not fully compliant with social distiancing. In fact, most academic studies suggest that contact rates for non infected individuals, tend to decrease by 30% to 40% during periossd of large influenza, but this is rarely higher, if not strictly imposed (see Caley, et al 2008).

- The term, \\((1-\frac{D_t}{N_t})\times \exp{(e)}\\), where \\(\frac{D_t}{N_t}\\) is the ratio of (death and patients in critical conditions) to population \\(N_t\\), at time \\(t\\). We posit that \\(er>0\\) where \\(er\\) is a proxy for risk aversion towards the virus. It plays out as a multiplier of extra caution taken by the population as far as the severe contagion spreads into the economy. During the 2019 H1N1 outbreak, 25% of Americans were avoided crowded area, as part of the risk perception to catch the disease (Steelfisher, et al, 2010). For a flu-type, a resulting reduction of the attack between 20 to 40% is not implausible as people start ot wear mask, and other protective equipments (Tyson, et al 2020). There might also be evidence that people distort information, and overstate the risk of the disease (Brahmbhatt and Dutta, 2008). This adds to the idea of e being large. For example, during the 2002 SARS, more than 25% of Asian citizens thought they could be contaminated, even if the ex post rate happened to be less than 0.1%.

- We finally posit \\(0 < b < 1\\), where \\(b\\) is the ratio of the level of contagion of non recorded cases to total cases. We note that \\(b\\) is linked to milder cases or asymptomatic cases of the COVID-19. There are only a few studies trying to estimate \\(b\\), and they seem to conclude that \\(b\\) might be in the range of 0.4-0.5 for COVID-19. If the portion of asymptomatic cases may be as large at 50%, \\(b\\) is likely to be in the range of 0.4 to 0.6. As said earlier, this rate of asymptomatic to total cases has been noticed in fullly tested populations like the village of Vo in Northern Italy, or in the cases of random sampling in South Korea.

### 3. Experiments <a name="cap3"></a>

[*Back to Table of Contents*](#tbc)

-------------------------------------

We have played with the five parameters above, after calibrating the SEIR model to Belgium as of April 1, at the time Belgium had recorded just below 14,000 COVID-19 infections, and suffered 828 hospital fatalities. Belgium has been a country that took a decision fast imposed major containment measures, already the day after the 10th recorded deaths in the country. It is however notably suffering from supply chain scarcity, as well as from test availability (just above 6/1,000 of population has been tested by April 1) so that the country early chose to only test people at hospital venues. Belgium does not trace people, yet it may be looking at possible means, at current stage.

We focus on hospital only, not home care, as we wish to look as well on the adéquation between hosptital capacity and hospitalizations. Most home care are put in quarnatine, and will start ot be extensivley tested by now.

#### Sensitivity analysis

If we look at the daily change of recorded cases and fatalities, on that day, Belgium recorded cases might imply that the pandemic could have been spreading, like the flu (\\(R_0=1.3\\)) by April 1, as crude estimate based on daily recorded cases for 20 days before, implies that \\(\hat{R_t}\\) looks like 1.5.  We however know that this \\(\hat{R_t}\\) suffers from mismeasurement errors and possibly asymetry in contagion. For our simulation, we thus have computed \\(R_0\\) for three assumptions of infected cases, e.g. with \\(r=0.7\\); \\(r=0.2\\), and \\(r=0.1\\) by April 1; \\(R_0\\) is computed up to March 18th before the containement measures, and before risk aversion may kick-in. Assuming that \\(d>1\\) is like the influenza, we compute that the adjusted \\(R_0=3.8\\) for \\(r=0.7\\); \\(R_0=2.7\\) for \\(r=0.2\\), and \\(R_0=2.55\\) for \\(r=0.1\\). Not surprisingly, our estimate of \\(R_0\\) decreases with \\(r\\), as \\(r\\) implies a large volume of unnoticed infections at the start. At those levels of \\(R_0\\), COVID-19 might look to be twice more infectious than the typical flu, at \\(R_0=1.3\\). This range of \\(R_0\\) is also consistent with multiple studies on the likely COVID-19 and also hints at the fact that we must induce large risk aversion and/or reduce a large portion of social contacts to hope to curb the disease, with \\(R_t<1\\).

**Table 1** presents the simulation results, based on one final assumption that unrecorded cases have 3.5 times lower probability to end up as a fatality in hospital than recorded cases. This assumption is consistent with the portion of large asymptomatic cases, and the fact that a large channel of fatalities are old persons residing into home cares.

Our simulation is illustrated the following discrete values: \\(s=0.4\\) and \\(s=0.7\\) (As said, \\(s=0.7\\) is difficult to achieve without very strict, and coercitive, rules, especially if the effort must be sustained more than 4 to 6 weeks); \\(b=0.4\\) and \\(b=0.6\\), as well as \\(e=[220; 1,100]\\). We posit as well that \\(u=80\%\\), and \\(u\\) is increased to 90%. The later value of the risk aversion, \\(e=1,100\\), has been computed from different studies, e.g. for the Spanish (He et al., 2013). Regarding \\(r\\), we present the two extremes case of \\(r=0.1\\) (most likely) and \\(r=0.7\\) (current understated cases). We posit as well that \\(u=80\%\\), and \\(u\\) is increased to 90%, as a result of stopping mega events, vacation gathering, etc. We also compute the implied hospital ICU capacity, as the last column, based on a capacity of 2,500 ICU hospital beds. The results in Table 1 demonstrate that:

- The main driver of the outcome of the COVID-19 among the 5 variables discussed is **the level of change in social contacts, \\(s\\)**. Given the high \\(R_0\\) for COVID-19, it is usually good to have social contacts on average reduced by more than 40%, in order to reach a peak in infection

- Given Belgium high ICU bed capacity, above average of EU-27 countries, and the fact that Belgium went quickly into containment actions, ICU capacity is still ok, even at \\(s=0.4\\); but there are also a few cases when ICU capacity becomes tight, **especially when risk aversion is low, and does not induce enough of self-protection of people in face of poor social distancing by third parties (e.g., when \\(e=220\\))**

- Superspreading plays a role, **but especially when risk aversion as well as contact reductions are limited- alas, it also happens when time ICU capacity becomes tight.**

- **Adequate measure, \\(r\\), of true infections is a must, as it drives the dynamics of healthcare resources, in particular in the long-term**; this is because better understanding of total infections makes \\(R_0\\) more accurate and typically not overstated, but it also implies a longer tail of cases. In our simulations, should \\(r\\) be truly 0.7, we know that \\(R_0\\) should then be  higher (\\(R_0\\) at \\(r=0.7\\) reaches 3.8, or roughly 60% higher than \\(R_0\\) for \\(r=0.1\\) to fit the data dynamics of infections). This means, that for the same proportional reduction of contacts, \\(s\\) and same level of self protection, \\(e\\), \\(R_t\\) will be higher in absolute value at same \\(t\\), for \\(r=0.7\\) than for \\(r=0.1\\). This means that the run rate, after May 1, will be higher in thart case. Further, when total infections are much higher than recorded ones (\\(r=0.1\\)), a large part of infections may be due to lighter cases than cases requiring long hospitalisations; but in reverse, when those cases are requiring hospitalizations, they tend to be more serious cases in absolute terms, and with higher mortality.[^1] As mortality further shortens time spent in ICU and peak is happening slightly faster, capacity usage after May is lower in case of \\(r=0.1\\). However, this does not say that this is better managed, this is at the expense of a tigher capacity in late April, and larger mortality.

[^1]: Hopsitalization rates are 3.5 lower for non recorded cases, but there are 7 times more infections than in the case of \\(r=0.7\\). Thus, the system gets more people into the hospital gate.

**Table 1 - Belgium SEIR model for COVID-19, rollout from April 1, 2020 to May 1, estimates.**

<table class='table table-bordered table-dark table-hover'>
    <thead>
        <tr>
            <th scope='col' colspan="8">R=0.1, R<sub>0</sub>=2.4</th>
            <th scope='col' colspan="2">ICU rate by:</th>
        </tr>
        <tr>
            <th scope='col'>e</th>
            <th scope='col'>s</th>
            <th scope='col'>b</th>
            <th scope='col'>u</th>
            <th scope='col'>Total Infection</th>
            <th scope='col'>Total Deaths</th>
            <th scope='col'>Infection peak by (10 days period)</th>
            <th scope='col'>Run rate death (10 days casualties)</th>
            <th scope='col'>May-01</th>
            <th scope='col'>Next 10 days</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th scope='row'>1,100</th>
            <td>0.7</td>
            <td>0.6</td>
            <td>0.9</td>
            <td>103,000</td>
            <td>2,660</td>
            <td>April 11 to 21</td>
            <td>290</td>
            <td>53%</td>
            <td>54%</td>
        </tr>
        <tr>
            <th scope='row'>1,100</th>
            <td>0.7</td>
            <td>0.6</td>
            <td>0.8</td>
            <td>107,250</td>
            <td>2,740</td>
            <td>April 11 to 21</td>
            <td>300</td>
            <td>55%</td>
            <td>56%</td>
        </tr>
        <tr>
            <th scope='row'>1,100</th>
            <td>0.7</td>
            <td>0.4</td>
            <td>0.9</td>
            <td>97,800</td>
            <td>2,565</td>
            <td>April 11 to 21</td>
            <td>280</td>
            <td>52%</td>
            <td>53%</td>
        </tr>
        <tr>
            <th scope='row'>1,100</th>
            <td>0.7</td>
            <td>0.4</td>
            <td>0.8</td>
            <td>100,250</td>
            <td>2,600</td>
            <td>April 11 to 21</td>
            <td>290</td>
            <td>53%</td>
            <td>54%</td>
        </tr>
        <tr>
            <th scope='row'>1,100</th>
            <td>0.4</td>
            <td>0.6</td>
            <td>0.9</td>
            <td>125,000</td>
            <td>3,060</td>
            <td>No peak</td>
            <td>370</td>
            <td>62%</td>
            <td>63%</td>
        </tr>
        <tr>
            <th scope='row'>1,100</th>
            <td>0.4</td>
            <td>0.6</td>
            <td>0.8</td>
            <td>137,000</td>
            <td>3,260</td>
            <td>No peak</td>
            <td>420</td>
            <td>67%</td>
            <td>69%</td>
        </tr>
        <tr>
            <th scope='row'>1,100</th>
            <td>0.4</td>
            <td>0.4</td>
            <td>0.9</td>
            <td>110,500</td>
            <td>2,810</td>
            <td>No peak</td>
            <td>330</td>
            <td>57%</td>
            <td>58%</td>
        </tr>
        <tr>
            <th scope='row'>1,100</th>
            <td>0.4</td>
            <td>0.4</td>
            <td>0.8</td>
            <td>118,000</td>
            <td>2,930</td>
            <td>No peak</td>
            <td>360</td>
            <td>60%</td>
            <td>61%</td>
        </tr>
        <tr>
            <th scope='row'>220</th>
            <td>0.7</td>
            <td>0.6</td>
            <td>0.9</td>
            <td>116,000</td>
            <td>2,890</td>
            <td>April 11 to 21</td>
            <td>340</td>
            <td>59%</td>
            <td>60%</td>
        </tr>
        <tr>
            <th scope='row'>220</th>
            <td>0.7</td>
            <td>0.6</td>
            <td>0.8</td>
            <td>125,000</td>
            <td>3,045</td>
            <td>April 11 to 21</td>
            <td>385</td>
            <td>63%</td>
            <td>65%</td>
        </tr>
        <tr>
            <th scope='row'>220</th>
            <td>0.4</td>
            <td>0.6</td>
            <td>0.9</td>
            <td>173,000</td>
            <td>3,780</td>
            <td>No peak</td>
            <td>685</td>
            <td>87%</td>
            <td>90%</td>
        </tr>
        <tr>
            <th scope='row'>220</th>
            <td>0.4</td>
            <td>0.6</td>
            <td>0.8</td>
            <td>211,000</td>
            <td>4,300</td>
            <td>No peak</td>
            <td>970</td>
            <td>108%</td>
            <td>112%</td>
        </tr>
    </tbody>
</table>

<table class='table table-bordered table-dark table-hover'>
    <thead>
        <tr>
            <th scope='col' colspan="8">R=0.7, R<sub>0</sub>=3.8</th>
            <th scope='col' colspan="2">ICU rate by:</th>
        </tr>
        <tr>
            <th scope='col'>e</th>
            <th scope='col'>s</th>
            <th scope='col'>b</th>
            <th scope='col'>u</th>
            <th scope='col'>Total Infection</th>
            <th scope='col'>Total Deaths</th>
            <th scope='col'>Infection peak by (10 days period)</th>
            <th scope='col'>Run rate death (10 days casualties)</th>
            <th scope='col'>May-01</th>
            <th scope='col'>Next 10 days</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th scope='row'>1,100</th>
            <td>0.7</td>
            <td>0.6</td>
            <td>0.9</td>
            <td>29,000</td>
            <td>1,340</td>
            <td>April 11 to 21</td>
            <td>490</td>
            <td>42%</td>
            <td>44%</td>
        </tr>
        <tr>
            <th scope='row'>1,100</th>
            <td>0.7</td>
            <td>0.6</td>
            <td>0.8</td>
            <td>37,000</td>
            <td>1,435</td>
            <td>April 11 to 21</td>
            <td>600</td>
            <td>50%</td>
            <td>52%</td>
        </tr>
        <tr>
            <th scope='row'>1,100</th>
            <td>0.7</td>
            <td>0.4</td>
            <td>0.9</td>
            <td>26,500</td>
            <td>1,300</td>
            <td>April 11 to 21</td>
            <td>470</td>
            <td>41%</td>
            <td>43%</td>
        </tr>
        <tr>
            <th scope='row'>1,100</th>
            <td>0.7</td>
            <td>0.4</td>
            <td>0.8</td>
            <td>31,500</td>
            <td>1,380</td>
            <td>April 11 to 21</td>
            <td>570</td>
            <td>48%</td>
            <td>50%</td>
        </tr>
        <tr>
            <th scope='row'>1,100</th>
            <td>0.4</td>
            <td>0.6</td>
            <td>0.9</td>
            <td>71,000</td>
            <td>1,815</td>
            <td>No peak</td>
            <td>1,210</td>
            <td>99%</td>
            <td>104%</td>
        </tr>
        <tr>
            <th scope='row'>1,100</th>
            <td>0.4</td>
            <td>0.6</td>
            <td>0.8</td>
            <td>99,000</td>
            <td>2,060</td>
            <td>No peak</td>
            <td>1,680</td>
            <td>141%</td>
            <td>148%</td>
        </tr>
        <tr>
            <th scope='row'>1,100</th>
            <td>0.4</td>
            <td>0.4</td>
            <td>0.9</td>
            <td>60,000</td>
            <td>1,680</td>
            <td>No peak</td>
            <td>1,095</td>
            <td>89%</td>
            <td>93%</td>
        </tr>
        <tr>
            <th scope='row'>1,100</th>
            <td>0.4</td>
            <td>0.4</td>
            <td>0.8</td>
            <td>82,500</td>
            <td>1,890</td>
            <td>No peak</td>
            <td>360</td>
            <td>126%</td>
            <td>127%</td>
        </tr>
        <tr>
            <th scope='row'>220</th>
            <td>0.7</td>
            <td>0.6</td>
            <td>0.9</td>
            <td>32,000</td>
            <td>1,375</td>
            <td>April 11 to 21</td>
            <td>540</td>
            <td>46%</td>
            <td>48%</td>
        </tr>
        <tr>
            <th scope='row'>220</th>
            <td>0.7</td>
            <td>0.6</td>
            <td>0.8</td>
            <td>40,400</td>
            <td>1,480</td>
            <td>April 11 to 21</td>
            <td>685</td>
            <td>50%</td>
            <td>53%</td>
        </tr>
        <tr>
            <th scope='row'>220</th>
            <td>0.4</td>
            <td>0.6</td>
            <td>0.9</td>
            <td>91,500</td>
            <td>1,920</td>
            <td>No peak</td>
            <td>1,520</td>
            <td>127%</td>
            <td>133%</td>
        </tr>
        <tr>
            <th scope='row'>220</th>
            <td>0.4</td>
            <td>0.6</td>
            <td>0.8</td>
            <td>140,000</td>
            <td>2,210</td>
            <td>No peak</td>
            <td>2,220</td>
            <td>195%</td>
            <td>204%</td>
        </tr>
    </tbody>
</table>


*Core assumption 1: non recorded cases (including asymptomatic cases) leads to 4 times lower hospitalisations;*

*Core assumption 2: Distribution of contagion follows influenza (top 20% makes 50% of contagion)*

*Core assumption 3: hospitalisation conversion to ICU and to fatalities calibrated on  April 1 and then constant*

*Core assumption 4: recovered cases are immune in short-term*

*Core assumption 5: contagion is 15 days for very mild cases, not going to hospitals, 8.5 when going to hospital.*

*Based on SEIR model, and calibrated data on period Mars 21 to April 1; only includes hospitalisation cases so as to measure matching with ICU*

#### Maximum likelihood point estimates

On top of the sensitivity analysis, we can provide point estimates of where Belgium may lie. We do this by finding the vector that minimizes the residuals prediction, for April 11, where data are avaialble for Belgium. To ensure convergence, we first hypothesize the most probable cases. Based on the above, the current range of values should be in the range of \\(r=0.1\\) ( multiple press reports had suggested that 100,000 cases could be the true toll of the pandemic by March 23, in Belgium);[^2] \\(s=0.5\\);[^3] \\(b=0.4\\) (as probably a large part of cases are asymptomatic cases); \\(e<1,100\\) as we also know that \\(e\\) may be « capacity constrained », (very limited mask protection available for example in Belgium). We also assume that \\([(1-u_t)d+u_t]=1.6\\), as for H1N1 influenza type. We can posit as well that \\(u\\) is 95%, as Belgium cancelled most events witth more than 100 people, and closed restaurants, etc.

[^2]: This extrapolations are based on the number of cases reoported with flu symptom, while the pandemics of flu was official phasing out by early March, see [https://www.dhnet.be/actu/belgique/100-000-cas-actifs-de-coronavirus-a-redouter-actuellement-en-belgique-5e7c88c8d8ad5816316d2145](https://www.dhnet.be/actu/belgique/100-000-cas-actifs-de-coronavirus-a-redouter-actuellement-en-belgique-5e7c88c8d8ad5816316d2145).

[^3]: It is said that for instance, about 70% of Belgian people are working from home. Nevertheless, travel outside home has been reduced by about 30% in a radius of 5 kms, versus traditional periods without containement, see [https://www.vrt.be/vrtnws/fr/2020/03/26/enquete-de-l_universite-danvers-les-seniors-suivent-mieux-que](https://www.vrt.be/vrtnws/fr/2020/03/26/enquete-de-l_universite-danvers-les-seniors-suivent-mieux-que), and [https://plus.lesoir.be/290734/article/2020-03-28/selon-une-analyse-des-donnees-telecoms-les-belges-adaptent-leur-comportement](https://plus.lesoir.be/290734/article/2020-03-28/selon-une-analyse-des-donnees-telecoms-les-belges-adaptent-leur-comportement).

Using maximum likelihood function optimisation, the vector that minimizes the gap versus observed data by April 11, 2020 suggests that **\\(e=940; s=0.55; b=0.43; u=0.96\\)** for \\(r=0.1\\). This is rather well specified as any 10% deviation from this vector on average increase residuals by more than 150%. The fit deteriorates fast if we increase the value of \\(s\\) and \\(b\\), and decrease \\(e\\). Social distancing to date has resulted in a decline just above 50%; lower than what has been computed for China (>80%; see Lin et al., 2020) as enforcement in Wuhan and China were very strict, for example. At this level, given \\(R_0\\) at 2.6, this is not enough per se to stop the pandemic, as the new \\((R_0=s\times 2.6 = 1.4 > 1)\\). We find that unrecorded cases are less contagious than others, in line with the fact that possibly half of infected people are asymptomatic, and inline with other estiamtes (Lin, et al., 2020). Risk aversion is present, but lower than what observed for the Spanish Flu with a 20% lower effect on limiting contagion (He, et al., 2013). The value of \\(u\\) means that about 40% of superspreading cases have been spotted.

If we optimise for \\(r=0.7\\), the local optimum implies a doubling in \\(e\\) (\\(e=2,200\\)), \\(s\\) increases to 63%, and \\(b\\) declines to 0.25%; \\(u=0.94\\). We should expect the optimisation to lead to such a result, as it implies that the limited number of cases outside hospitals is much less contagious (\\(b=0.25\\) for \\(r=0.7\\) versus \\(0.43\\) for \\(r=0.7\\)) than the ones arriving to hospitals, reinforcing the rationale not to focus on those cases when one lacks test ability. The results for \\(r=0.7\\) are however not that credible. They exhibit a significant deterioration in predictions, with an twenty-fold increase in residuals versus the case of \\(r=0.1\\).[^4]

[^4]: For sake of completeness, we also increased the asymmetry of contagion distribution, \\(d\\) from the current case of top 20=50%, to top 20=65%, which is in line with some influenza metrics. By assuming a higher asymmetry, the predicition deteriorates too, but only two the three fold the original simulation. With this new case, we implictly state that the actual \\(R_0\\) is bigger than thought, but contagion loses power across network of individuals. We  find that \\(b\\) decreases accordingly, from \\(b=0.43\\) to \\(b=0.36\\); \\(s\\) increases from 0.56 to 0.62, and \\(e = 940\\) moves up to 1,160. The value of \\(u\\) remains unchanged. Again, this result simply reflects that one may have to push harder to flatten an pandemic with higher \\(R_0\\).

Continuing thus on our favorite case on \\(r=0.1\\), and keeping the values of the vector constant for April, Belgium might reach 105,000 total (recorded and not recorded) infections by May 1st, with a cumulative toll of 2,700 hospital deaths, and an active ICU utilisation, of 1,400 beds. The peak in daily infections happens before April 17 to April 21, while the number of new cases being hospitalized peaks slighly later, as do number of deaths, just before may 1st, reducing the pressure on ICU.

Still, a deterioration in \\(s\\) and \\(e\\) would lead to a plateau and a rebuild of demand for ICU, especially when \\(s<0.4\\) and \\(e<550\\). We thus confirm that reduction of contagious interaction, \\(s\\), is the main first order target, and increased self protection, \\(e\\). In the absence of specific targetting, and only testing at time of hospital venue, we should aim for a reduction of 50% of interaction both to flatten the curve, and be compatible with health constraints; Risk aversion leads to self protective behavior is a good thing, leading people to more systematically wash hands, wear masks etc. In this respect, we believe that the controversy raised in Belgium regarding the wearing or not mask is unfortunate; the behavior is effective if everyone does it, and on top of, not in substitution of, other distancing and self protective behavior.

### 4. From reach to selective testing, tracing and enforced quarantine <a name="cap4"></a>

[*Back to Table of Contents*](#tbc)

-------------------------------------

One can directly derive from above, that a reduction of contact by 50% is difficult to hold, especially, without some imposed shut down of education and work in the context of the COVID-19. In such a case, we estimate that \\(s=28\%\\), and infections, ICU and death toll will increase versus current case by 20%, 18%, and 15% by May 1st, 2020[^5]. Peak will not arise in this time period.

[^5]: Multiple studies suggests that about 40% of close contacts is linked to school and work. Given that about 70% of those contacts seem to have been eliminated through containement, about half (29%) of \\(s\\) (57%) is due to this channel; or otherwise, said, without it, \\(s\\) will decrease to \\(s=28\%\\), creating a rebuild of the curve.

However, keeping the economy and education close, has large perverse consequence on the economy. Hence, it must imply a few additional amended strategies, for economies to be relaunched, and keeping the disease under control. This includes:

- **Telecommuting should be promoted as a standard** of practice going forward. Nevertheless, this is only possible for certain sectors, and for some functions, possibly, for about 1/3 of the working population to date[^6] (see also Dingel and Neiman, 2020). Even if done, the task distrbution might imply that this will be possible for only a partial time of the work, implying major reorganization of the way one work. Further, the shift will especially play on the lower quartile of the working population, as already telecommuniting is easier and more pronounced for higher quartile of workers (managers, etc.).

[^6]: See reference in [https://bfi.uchicago.edu/working-paper/how-many-jobs-can-be-done-at-home/](https://bfi.uchicago.edu/working-paper/how-many-jobs-can-be-done-at-home/)

- **Public protection must become the new normal**, e.g. in Asia, most restaurants require individuals to wash hands, most malls have hydro6alcohol gel at their entrance to be used by the public etc. Close contact prohibitions make this a difficult strategy for major sportive, cultural, or entertainment events, or major business fares for example. The same issue may apply for most transportations, not only within the mode of transportation, but because excessive mobility may seed new waves of the coronavirus, as currently witnessed by China.[^7]

[^7]: [https://news.yahoo.com/china-reports-record-coronavirus-cases-013153635.html](https://news.yahoo.com/china-reports-record-coronavirus-cases-013153635.html)

- Thus, the most important seems to be the priority of systematic testing, as acknowledged among others by Dewatripont et al. (2020). Testing can be used for two objectives: ensuring people are not infected, so they can be safe to be interacted with, or be put back to work. One clever idea is group testing to maximize costs and roll out, see  Gollier and Olivier Gossner, (2020). Or, in our case here, ensuring that one can spot the infected and their close social ties upfront, so that they can be put in strict quarantine, instead of putting everyone in containment.

Regarding the last point, we again resort to simulation to show the logic,  based on Belgian figures for the COVID-19 pandemic. At the estimated \\(R_0\\) of 2.6, \\(u=96\%\\), and \\(s=28\%\\) as result of no imposed economic actions,  we find that the new amended \\(R_0\\) becomes 1.7, and about 69% of population may be affected in the long term by the COVID-19 with \\(z=69\%\\) is the result of solving for the equation (2):

$$ R_0+\Big(\frac{1}{z}\Big)\times \ln{(1-z)} = 0 $$

where \\(R_0=1.7\\).

In the case of \\(s=57\%\\) (full shutdown), same math leads to 17% of the Belgian population to be infected. We thus infer that the economic shut down prevents 52% of population infected cases, or a reduction of 52/69=75% of the infections. Yet, a) it also hurts at least 31% of people who will not have been infected; b) on top of this, if all infected cases will lead to 3 weeks of work lost, this has to be compared to \\(70\%\times(1-31\%)=49\%\\) of work lost for 8 weeks, or more than two times the true cost of shutdown, which may or may not be justified by the productivity loss of the fatalities.[^8]

[^8]: 0% is 100% shutdown with 30% of economy remaining in function as necessary. Note that, if all infected cases will lead to 3 weeks of work lost, this has to be compared to \\(70\%\times(1-31\%)=49\%\\) of work lost for 8 weeks, or more than two times the true cost of shutdown. On the other hand, and assuming at 2% death rate from our Table 1, and statitics that suggests that 40% of total deaths will be for people with still 20 years of work, this is equivalent to \\(52\%\times 2\%\times 0.4\times 20=0.08\%\\) of a year, or 4 weeks of productivity loss equivalent; thus, at this level, the economic shutdown becomes a valuable return. The labor productivity is only one factor, if this creates a demand pressure and a spiraling depression, then the shutdown is indeed not returning a positive ROI for society.

Now, consider we can target effectively the contaminated individuals, at 70% or 90%, and their social ties obey like today, in Belgium at containment, at 50% rate, or it imporves in proportion of the one at risk, at 50%/69% = 72%. At those levels, worse case (70% specificity and 50% rate of compliance) still imply 59% of cases contamination, while the base case (90% and 72% compliance), leads to less than 5% contamination. Middle case (70% specificity, 72% rate of compliance) would lead to 30% attack rate. We derive from this simulation that a 75% specifity success, with 75% compliance of quarantines for infected and their social ties, may lead to same effect of economic shutdown, but with much lower economic and fairness issues.  

### 5. The new social norm of being traced <a name="cap5"></a>

[*Back to Table of Contents*](#tbc)

-------------------------------------

We are not stating from above we should give up (some measures of) the economic shutdown. We understand that test specificity must be large enough, and jury is still out it can, especially given high asymptomatic cases of COVID-19. We might have to do a mix of both approach in those circumstances, even if today, asymptomatic cases may have low contagious power; and evidence shows that medical and non medical testing combined may make the target of 70% possible (Alibaba claims that its AI-based applications have success at 95%).

We also understand that tracing individuals can be done through mobile and bluetooth/Beacon like technology, but this must be done with extreme caution (Christoph and Gunther, 2020). However, given the large externality of contagion, tracing is likely to be raised as an important social norm to comply with, in order to accept a reconciliation of health and economic prosperity.

In practice, this path of combined testing/tracing and selective economic shutdown has been shown today by countries such as Singapore or South Korea, to be the best to control the COVID-19 pandemics to date (Anderson et al., 2020). In those cases, data were anonymized and a civil society governance model for data crunching was made possible to preserve privacy and GDPR compliance. As such, digital technologies may become a great complementor to our society, both as prevention to find cures and vaccine to COVID-19, as well as to manage social contagion process (see Pissarides and Bughin, 2019).

### 6. References <a name="cap6"></a>

[*Back to Table of Contents*](#tbc)

-------------------------------------

Anderson, Roy M., Hans Heesterbeek, Don Klinkenberg, and T. Déirdre Hollingsworth (2020), *"How will country-based mitigation measures influence the course of the COVID-19 epidemic?,"* **The Lancet 395**.

Baldwin, R. (2020), *"IT is not exponential - an economist view of the epidemiological curve,"* [https://voxeu.org/article/it-s-not-exponential-economist-s-view-epidemiological-curve](https://voxeu.org/article/it-s-not-exponential-economist-s-view-epidemiological-curve)

Brahmbhatt and Dutta, (2008), *"On SARS type of economic effects during infectious disease outbreaks,"* **World Bank, Policy research working paper**.

Brauer, M. (2019), *"Early estimates of epidemic final sizes,"* **Journal of Biological Dynamics**.

Bughin, J. (2020), [Why we must protect our heathcare workfoce during COVID-19.](https://learning-from-the-curve.github.io/health-management/2020/04/25/Why-we-must-protect-the-healthcare-workforce-during-COVID-19.html)

Bughin, J. (2020), [Beyond the recorded figures: How the COVID-19 pandemic might actually be playing out.](https://learning-from-the-curve.github.io/health-management/2020/04/27/Beyond-the-recorded-figures-How-the-COVID-19-pandemic-might-actually-be-playing-out.html)

Caley, et al. (2008), *"Quantifying social distancing arising from pandemic influenza,"* **Journal of the Royal Society Interface**.

Christoph and Gunther (2020), *"Tracing contacts to control covid 19 pandemic,"* 
**Arxiv**.

Dewatripont, M., M. Goldman, E. Muraille and J.-P. Platteau (2020), *“Rapidly identifying workers who are immune to COVID-19 and virus-free is a priority for restarting the economy”,* **VoxEU.org, 23 March**.

Dai, (2020), *"Psychological impact of coronavirus disease outbreak on heatlhcare in China,"* **MedRix**.

Dingel and Neiman, (2020) *"How many jobs can be done at home?,"* **Covid Economics Issue 1, 3**.

Fang, (2020), *"The mental health of medical workers in Wuhan, China dealing with the 2019 novel coronavirus,"* **The Lancet**.

Group testing against Covid-19, Christian Gollier and Olivier Gossner.

Hamilton, S.D., Lo, A.S., Baumgaertner, B.O. and Krone, S.M., (2020), *"The Timing and Nature of Behavioural Responses Affect the Course of an Epidemic",* **Bulletin of Mathematical Biology**.

*"Beyond \\(R_0\\): the importance of contact tracing when predicting epidemics",* Laurent Hebert-Dufresne, Benjamin M. Althouse, Samuel V. Scarpino, and Antoine Allard.

Ji, Y., Ma, Z., Peppelenbosch, M.P. and Pan, Q., 2020, *"Potential association between COVID-19 mortality and health-care resource availability,"* **The Lancet Global Health, 8(4), p.e480.**

Kelso et al., 2013, *"Economic analysis of pandemic influenza mitigation strategies for five pandemic severity categories,"* **BMC Public Health**.

Kermack and McKendrick, (1927), *"A Contribution to the Mathematical Theory of Epidemics,"* **Proceedings of the Royal Society**.

Lee, V.J., Chiew, C.J. and Khong, W.X., (2020), *"Interrupting transmission of COVID-19: lessons from containment efforts in Singapore",* **Journal of Travel Medicine**.

Li, et al. (2020), *"Substantial undocumented infection facilitiates the rapid dissemination of novel coronavirus,"* **Science**.

Lloyd Smith et al, (2005), *“Superspreading and the eﬀect of individual variation on disease emergence,”* **Nature**.

Person B., Sy F., Holton K., et al. (2004), *"Fear and Stigma: The Epidemic within the SARS Outbreak,"* **Emerging Infectious Diseases. 10(2):358-363**.

Pissarides, Ch. and Bughin, J., (2019), *"Dont squander the tech revolution,"*[https://www.project-syndicate.org/commentary/ai-automation-effects-on-wellbeing-by-christopher-pissarides-and-jacques-bughin-2019-07](https://www.project-syndicate.org/commentary/ai-automation-effects-on-wellbeing-by-christopher-pissarides-and-jacques-bughin-2019-07)

Rosenbaum, L., (2020), *"Facing covid-19 in Italy—ethics, logistics, and therapeutics on the epidemic’s front line,"* **New England Journal of Medicine**.

Steelfisher, et al, (2010), *"Public's response to the 2009 H1N1 influenza pandemic,"* **New England Journal of Medicine**.

Worldometer (2020), *"Covid-19 coronavirus pandemic,"* [https://www.worldometers.info/coronavirus/](https://www.worldometers.info/coronavirus/)
