---
layout: post
title: 'We might be winning the battle of the COVID-19 epidemic in China: a dynamic R(t) perspective'
date: 2020-04-22T10:00:00.021Z
category: health-management
summary: COVID-19 went recognized at the end of December 2019, when a Wuhan hospital admitted four individuals from the Seafood Market. Given the exponential contagion during  the outbreak as it was also discovered at the start of the epidemic at Hunan for the COVID-19, there has been an absolute case that warrants to act fast (that is, before the take off of the exponential), as well as at scale, (so that the contagion becomes non self-reproducing). The good news is that the world has been facing many epidemics, and has learned a set of critical actions to curb the diffusion of many diseases, such as Ebola, SARS and others.
author:
  - J. Bughin
---

Dr Jacques Bughin, UN consultant, Solvay Business School ULB, Portulans Institute and G20Y, former Director McKinsey Global Institute, and senior partner McKinsey & Company.

**Table of Contents**:<a name="tbc"></a>

1. [Introduction](#cap1)
2. [What could drive a major pandemic for COVID-19?](#cap2)
3. [The dynamics of \\(R_t\\) for the COVID-19 case: we may be winning the curse in China](#cap3)
4. [Downgrading to a sever flu, instead of 20 million fatalities?](#cap4)

### 1. Introduction <a name="cap1"></a>

[*Back to Table of Contents*](#tbc)

-------------------------------------

#### **March 7**

In a series of post articles (available [here](https://www.learningfromthecurve.net/health-management/)), I recently made the point that, under a no containment scenario, COVID-19 may bring a) millions of fatalities worldwide, b) as well as significant damage to economies, as result of a negative worldwide spiral of reduction in demand and supply.

COVID-19 went recognized at the end of December 2019, when a Wuhan hospital admitted four individuals from the Seafood Market. Given the exponential contagion during  the outbreak as it was also discovered at the start of the epidemic at Hunan for the COVID-19, there has been an absolute case that warrants to act fast (that is, before the take off of the exponential), as well as at scale, (so that the contagion becomes non self-reproducing). The good news is that the world has been facing many epidemics, and has learned a set of critical actions to curb the diffusion of many diseases, such as Ebola, SARS and others.

The type of explosion of cases one witnessed at the start of the COVID-19 outbreak made indeed lots of insiders to fear for the worst. In less than one month, from January 20 to February 17, **the recorded cases increased exponentially, from 270 to close to 50,000 in the Hubei province of China, or a factor of 200; with a continous doubling of cases every 7 days like in the early weeks of the outbreak, this could have led to hundreds of thousands infected cases by early April.**

But there is some good news. Even if China took a few weeks to launch strong actions, Chinese authorities then quickly imposed by mid January large scale quarantines, as well multiple city shutdowns. Other, more recent actions have involved new series of ways to more accurately diagnose mild cases, as well as the establishment of a mobile based QR code coloring of Chinese citizens to secure more effective sorting of susceptibles, contaminated and sane cases.[^1]

[^1]: See [https://finance.yahoo.com/news/china-seeks-help-national-tech-110156832.html](https://finance.yahoo.com/news/china-seeks-help-national-tech-110156832.html).

Those actions, in line with our prescriptions needed to maximize the chance to reduce the spread of disease, seem to work. Experts are consequentially more and more optimistic that the pandemic may become controllable and run out of course in China, in the next two months, instead of exploding.[^2]

[^2]: See Lucey, Daniel; Sparrow (2020), *"China Deserves Some Credit for Its Handling of the Wuhan Pneumonia"*, **Foreign Policy**.

Based on current numbers and the actions taken by China, and in other European countries with outbreaks such as Italy and France, **we may be leaning towards a scenario towards a severe flu worldwide. The key is thus to continue high vigilance, deliver fast and scalable actions of social distancing, shutdowns if necessary, across the globe when the epidemy is entering a new country. And make sure citizens adapt their social behavior as a significant contributor to curb the disease spread.**

### 2. What could drive a major pandemic for COVID-19? <a name="cap2"></a>

[*Back to Table of Contents*](#tbc)

-------------------------------------

A pandemic's size, speed, and risk depend on the  level and spread of population clusters’ reproduction rate, incubation and contagious period, and fatality rate (see my [previous article](https://www.learningfromthecurve.net/health-management/2020/04/16/Three-key-COVID-19-indicators-to-curb-a-potential-of-20-million-human-fatality.html)). On the positive side for COVID-19, the virus seems to exhibit a strong, but not exceptional high level of the reproduction rate, called \\(R_0\\), (\\(R_0\\) is in the range of 2 for the whole of China, estimated from data january to February, and about 2.7 for same period in the Hubei region). But on the negative side, the virus has a material fatality rate (we estimate between 0.5% to 2%) versus a typical flu, as well as exhibits a possibly less concentrated distribution of social contagion than other viral diseases.

#### **Changing \\(R_t\\):the underlying maths and case study**

As the exponential nature of the outbreak is driven by the mean and spread of reproduction rate, \\(R_0\\), it is critical to see how we can limit it. The reproduction rate \\(R_0\\) is easily interpretable as the product of contact frequency, \\(c\\), and the probability of being contaminated for each contact, \\(p\\):[^3]

[^3]: See Larson, 2007, *Simple Models of Influenza Progression Within a Heterogeneous Population*, **Operations Research**.

$$ R_0 = p\times c $$

$$ R_{t} = \Big(p + \frac{dp}{dt}\Big) \times c + \Big(c + \frac{dc}{dt}\Big) \times p $$

Where \\(d(.)\\) is the time differential change.

\\(p\\) is clearly a variable one can influence, and rather quickly. This implies that \\(R_t\\) may evolve over time, as a result of imposition of quarantines, or still because the population changes behavior in terms of social distancing, with \\(\\frac{dp}{dt}<0\\).

In general, the number of contacts, \\(c\\), may be roughly constant behaviorally, at least for very low (perceived) risk disease, and for people not aware of the possible pandemic. However, the larger the perceived risk of the pandemic, the more likely citizens may adapt behavior and reduce contact, making \\(\\frac{dc}{dt}<0\\), and \\(R_t\\) decline with time. For example, during the 2002 SARS, more than 25% of Asian citizens thought they could be contaminated, even if the ex post rate happened to be less than 0.1%; as a result a large set of persons were reducing travel; 10 to 50 percent decline in tax revenues, and up to 80 percent decline in luxury hotel stays.[^4] Likewise during the 2019 H1N1 outbreak, 25% of Americans were avoiding crowded areas.[^5]

[^4]: See Brahmbhatt and Dutta, 2008, *On SARS type of economic effects during infectious disease outbreaks*, **World Bank**, Policy research working paper.

[^5]: See Steelfisher, et al, 2010, *Public's response to the 2009 H1N1 influenza pandemic*, **New England Journal of Medecine**.

Recent research on pandemics suggests that, even with uncertainty, it would be rational for any self interested individual to decrease the number of contacts, \\(\\frac{dc}{dt}<0\\). For a flu-type, frequency might change downward, with a resulting reduction of 20% to 40%. In general, the types of reduction depends on many behavioral factors as well ad the wisdom of crowd. Likewise, the resulting decline on \\(p\\), depends on how people wishes to self-protect, and in geenral \\(\\frac{dp}{dt}<0\\), and the effect may be more or less the same magnitude as \\(\\frac{dc}{dt}\\).[^6]

We have yet to know how behaviors have changed in China, as a result of the spread and perception of risk of the spread, of COVID-19. But there is enough anecdotal evidence that behaviors have indeed changed for citizens, towards lower contact rates, while authorities in any case forced them towards that consequence. If one looks at other outbreaks, and looked at effective reproduction rates, we find a following typical cycle of exponential at the start, then a slowing growth to the peak, and then, a last phase, when epidemic phases out (Table 1).

[^6]: See, Tyson, et al. 2020, *The Timing and Nature of Behavioural Responses Affect the Course of an Epidemic*, **Bulletin of Mathematical Biology**; or still Eksin, et al. 2019, *Systematic biases in disease forecasting – The role of behavior change*, **Epidemics, 27**.

**Table 1: Dynamics of reproduction rates**

<table class='table table-bordered table-dark table-hover'>
    <thead>
        <tr>
            <th scope='col'>Outbreak</th>
            <th scope='col'>Reproduction rate R<sub>0</sub> (first three weeks)</th>
            <th scope='col'>Delta change first three weeks to mid period</th>
            <th scope='col'>Mid period of outbreak (3 months)</th>
            <th scope='col'>Delta change mid to late period</th>
            <th scope='col'>Late period</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th scope='row'>SARS Asia</th>
            <td>2.2 to 3.6</td>
            <td>-40%</td>
            <td>1.6 to 1.8</td>
            <td>-58%</td>
            <td>0.7</td>
        </tr>
        <tr>
            <th scope='row'>SARS elsewhere</th>
            <td>1.6</td>
            <td>-41%</td>
            <td>0.95</td>
            <td></td>
            <td>not computed</td>
        </tr>
        <tr>
            <th scope='row'>H1N1 2009</th>
            <td>2.5 to 3</td>
            <td>-51%</td>
            <td>1.4</td>
            <td>-63%</td>
            <td>0.5 to 0.6</td>
        </tr>
        <tr>
            <th scope='row'>Mexican Flu</th>
            <td>2.1</td>
            <td>-15%</td>
            <td>>1.8</td>
            <td>-50%</td>
            <td>>0.9</td>
        </tr>
    </tbody>
</table>

*Source: Lit Search, author's own computation*

The dynamics around the phases are not exactly the same. SARS and H1N1 were handled quickly with large quarantines. The case of the Mexican flu is also a known case of active policy reduction, but it took time to be handled. The flu first took its spread in multiple villages in the country, but without very large awareness of the inhabitants—leading to a significant attack rate in the range of 40% to 50% of the population. The city of Mexico got the flu epidemy noticed, and in the first weeks of the flu moving into the country capital, social distancing was imposed together with closure enforced on schools, public spaces and hospitals reducing \\(c\\) significantly, and leading to a significant decline on the reproduction rate, \\(R_t\\) through times.

### 3. The dynamics of \\(R_r\\) for the COVID-19 case: we may be winning the curse in China <a name="cap3"></a>

[*Back to Table of Contents*](#tbc)

-------------------------------------

We still have to know the exact drivers of \\(R_t\\) for the Covid 19-in China, but we can estimate its effect, through the shape of how the outbreak has behaved. Using the numbers of recorded contagions, and estimating a « two weeks by two weeks » cut off estimate, we reach the following result that we might have reached a situation of control in China (see Table 2).[^7] In response to the outbreak of COVID-19, a series of prompt public health measures have been undertaken.[^8] On January 1st, the Huanan Seafood Wholesale Market was closed in the hope of eliminating zoonotic source of the virus. On 11 January, reverse transcription-polymerase chain reaction (RT-PCR) reagents were developed to trace the infection. Ten days later, the Emergency Response System was activated and intensive surveillance and isolation of suspect cases started aggressively. School and work were suspended. Close ties to infected received medical observation and quarantine for 14 days. Travel from and to Wuhan City as well as other medium-sized cities in Hubei Province went to be restricted.

[^7]: China outside the Hubei region got to start the measure directly after the notice of the Wuhan epicenter, thus got more quickly into influencing social contacts to quickly reduce \\(R_t\\).

[^8]: See Wang, et al. 2020, *Phase-adjusted estimation of the number of Coronavirus Disease 2019 cases in Wuhan, China*, **Cell Discovery**.

Based on typical contact profiles (at home, with friends, at work, school), the frequency of contact may roughly be 40% based on public space connections (travel, school, at work), and 60% based on community and family interactions. Assume that complete distancing was effective in 80% in public space in the Hubei region, and that social distancing from community was half-effective, given asymptomatic cases at 50% of total cases. This means that \\(\\frac{dc}{dt}=-60%\\) for China. As \\(R_t\\) decreased roughly by 85% from Jan 23 to  Feb 29, we would infer that \\(\\frac{dp}{dt}<0\\), equal to -25%. This number may be in line with change in protective behaviors seen in other outbreaks.[^9]

[^9]: See Eksin, et al. 2019, *Systematic biases in disease forecasting – The role of behavior change*, **Epidemics**.

**Table 2: Dynamics \\(R\\) of reproduction rates**

<table class='table table-bordered table-dark table-hover'>
    <thead>
        <tr>
            <th scope='col'>Date</th>
            <th scope='col'>Hubei region</th>
            <th scope='col'>Delta change</th>
            <th scope='col'>Rest of China</th>
            <th scope='col'>Delta change</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th scope='row'>Jan 15</th>
            <td>5.5 to 6.0</td>
            <td>-18%</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th scope='row'>Jan 30</th>
            <td>4.0 to 5.5</td>
            <td>-38%</td>
            <td>2.8</td>
            <td>-61%</td>
        </tr>
        <tr>
            <th scope='row'>Feb 15</th>
            <td>2.5 to 3.5</td>
            <td>-70%</td>
            <td>1.1</td>
            <td>-55%</td>
        </tr>
        <tr>
            <th scope='row'>Feb 29</th>
            <td> < 1 </td>
            <td></td>
            <td> < 1 </td>
            <td></td>
        </tr>
    </tbody>
</table>

*Source: Wikipedia, John Hopkins University, own computation*

*Note: Ranges depend on hypotheses on reported cases, and on changes in contagion period*

### 4. Downgrading to a sever flu, instead of 20 million fatalities? <a name="cap4"></a>

[*Back to Table of Contents*](#tbc)

-------------------------------------

It is important that those figures in Table 2 got confirmed by more thorough analyses than just moving average, with no data filtering, as well as on only recorded contaminated figures. Further, wave 2 or wave 3 may also arise, as it was the case for the Spanish flu. But the key insights too, are that, even if one assumes from now on, that \\(R_t\\) is getting indeed just below 1, **the total outbreak will be more like 3% to 5% of the total population in the Hubei region. For China outside of the Hunan region, the figures will be then less than 1% of total population.**

Otherwise stated, and scaling those figures to worldwide population, we will be between 0.4 million to 4 million fatalities (China outside of Hubei, and Hubei) regions, or a reduction of at least 80% of the fatalities, as it got noticed, after the actions to control H1N1 in 2019 (we estimate, roughly minus 85% reduction versus potential of the pandemic). We will have succeeded in controlling the outbreak.

-------------------------------------

*© Jacques Bughin. Written March 07. Comments more than welcome. All errors are mine. References listed as they are found in the text*
