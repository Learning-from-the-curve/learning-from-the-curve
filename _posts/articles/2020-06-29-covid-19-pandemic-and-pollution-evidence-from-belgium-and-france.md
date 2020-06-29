---
layout: post
title: "COVID-19 Pandemic and Pollution: Evidence from Belgium and France"
date: 2020-06-29T17:22:10.393Z
summary: The outbreak of COVID-19, which is the most serious public health
  crisis in decades, is bringing complex challenges worldwide. Fighting this
  pandemic requires a better understanding of the so-called ‘risk factors’
  associated with the spread of the virus. Identifying the driving forces
  favoring the diffusion of the virus is a topic of primary importance, not only
  to contain the rapid spread of the current pandemic, but also to prevent the
  occurrence of future pandemics.
author:
  - I. Natali
  - S. Amaral-Garcia
category: articles
---
**Table of Contents**:<a name="tbc"></a>

1. [Introduction](#cap1)
2. [Data sources and methodology](#cap2)
    - [Pollution Data](#cap2.1)
    - [COVID-19 Data](#cap2.2)
        - [Belgium](#cap2.2.1)
		- [France](#cap2.2.2)
3. [Results](#cap3)
	- [Graphical Analysis](#cap3.1)
	- [Econometric Analysis](#cap3.2)
4. [Conclusions](#cap4)
5. [References](#cap5)
6. [Additional Material](#cap6)

### Introduction <a name="cap1"></a>

[*Back to Table of Contents*](#tbc)

The outbreak of COVID-19, which is the most serious public health crisis in decades, is bringing complex challenges worldwide. Fighting this pandemic requires a better understanding of the so-called ‘risk factors’ associated with the spread of the virus. Identifying the driving forces favoring the diffusion of the virus is a topic of primary importance, not only to contain the rapid spread of the current pandemic, but also to prevent the occurrence of future pandemics.

Up to date, there is solid evidence that the elderly are the most vulnerable age group. Patients with some underlying health conditions might be affected more severely. Recently, concerns arose as poorer areas might be more affected by the pandemic than more affluent areas.[^1] There are also cases of people with no risk factors who become critically ill. Given the novelty of the virus, however, more research about ‘risk factors’ related to the COVID-19 virus is needed.

Some researchers have postulated the existence of a relationship between the level of air pollution and the pace at which the virus spreads. In a recent position paper, a group of researchers at SIMA (Italian Society for Environmental Medicine) has shown, mainly through graphical analysis, the existence of a positive association between the number of COVID-19 cases and \\(PM_{10}\\) (Particulate Matter 10) daily limit exceedances in Italian provinces (SIMA, 2020). The hypothesis, here, is that the particulate matter may act as a ‘vector’, facilitating transmission and allowing the virus to spread quickly. Soon after, the presence of the virus was uncovered on 34 samples of \\(PM_{10}\\) in the province of Bergamo (Setti et al., 2020).

Even though some first evidence on the relationship between pollution and COVID-19 is emerging, research is still clearly scant and mostly limited to graphical analysis. In this paper, we contribute to the literature by taking a closer look at the relationship between air quality (as measured by the presence of Particulate Matter, PM10 and PM2.5, in the air) and COVID-19-related harm. We focus on two hardly-hit European countries: Belgium and France. We consider measures of \\(PM_{10}\\) and \\(PM_{2.5}\\) concentrations at the province level for Belgium, and at the regional level for France. Our outcome variables include the number of COVID-19 cases, the number of hospitalizations, the number of individuals in Intensive Care Units (ICU in what follows) and the number of deaths (at the province or regional level). We exploit variation both across regions (or provinces) and across time to study the association between the two pollutants and the virus. Through graphical analysis, we provide suggestive evidence of a positive association between the two. We further corroborate this evidence through simple regression analysis.

Understanding the association between pollution and the COVID-19 pandemic is important from a public health and a regulatory point of view. Indeed, this enables to provide both the scientific community and decision-makers with valuable knowledge and tools to react more promptly in case other epidemics arise in the future and on which regulatory interventions would be useful for their prevention and containment. Moreover, this type of analysis provides regulators with information on which factors should be taken into account when examining possible lockdown easing policies and exit strategies.

The rest of the paper is organized as follows. In Section 2, we describe the data sources and the methodology used to clean and aggregate the available information. Section 3 shows and discusses the results of our analysis for Belgium and France. Section 4 concludes.

### Data sources and methodology <a name="cap2"></a>

#### Pollution Data <a name="cap2.1"></a>

[*Back to Table of Contents*](#tbc)

Pollution data was collected from the European Environment Agency (EEA) website. This database provides information on concentrations of selected pollutants for each sampling point in each member state. EEA receives up-to-date data from most of its member states on an hourly or daily basis, depending on the country. We select two pollutants, \\(PM_{10}\\) and \\(PM_{2.5}\\), which are measured in \\(\mu g/m_{3}\\).

We consider the average daily concentrations across sampling points in the same province or region, in order to obtain an average province/regional measure of the quality of the air. We have data for each province in Belgium (for a total of 11 provinces) and each (old) region in France (excluding overseas).

We focus on \\(PM_{10}\\) and \\(PM_{2.5}\\) for two reasons.[^2] First, the particulate matter contribute predominantly to the development of respiratory and cardiovascular diseases. Its severe effects on human health and mortality are largely due to the small size of these particles, which allows them to penetrate deep into the lungs (WHO, 2013). Second, prior research has found a positive association between these two pollutants and the spread of the COVID-19 pandemic. As mentioned, one hypothesis is that the particulate matter acts as a ‘vector’ that transports the virus and, hence, facilitates its circulation. In this paper, we aimed at verifying the validity of this hypothesis.

#### COVID-19 Data <a name="cap2.2"></a>

[*Back to Table of Contents*](#tbc)

We use different data sources for COVID-19 in Belgium and France, as described below. Each country has been affected by the virus in different moments of time. As a consequence, each country started to count cases, hospitalizations and deaths at different dates. Therefore, we perform our analysis for each country separately.

Moreover, our (simple) econometric analysis exploits the panel structure of our data. Hence, the unit of analysis is province-day for Belgium, and region-day for France. We always consider outcome variables standardized by the province or regional population and lagged by 20 days. That is, each COVID outcome variable is regressed on the level of pollution 20 days before. The rationale is that, according to the currently available medical knowledge, the virus takes between 14 and 20 days before showing the first symptoms. As a consequence, each panel includes pollution data starting from 20 days before the COVID-related harm counts (see below).

Finally, the dependent variables are always expressed in logarithmic terms, while the independent variables (pollution concentrations) are kept in levels.

##### Belgium <a name="cap2.2.1"></a>

Data concerning coronavirus-related harm are collected from Sciensano.be. This database provides information on the number of COVID-19 cases, as of March 1, and on hospitalizations, as of March 15, both at the province level and on a daily basis. Data on deaths are, unfortunately, only available at the regional level. Hence, for Belgium, we consider the following outcome variables: total number of individuals currently hospitalized per 100,000 inhabitants; total number of individuals currently in ICU per 100,000 inhabitants; number of cases per 100,000 inhabitants. Population data are collected from Statbel and refer to population on January 1, 2020.

The panel containing information on the number of cases, includes data from February 10 (20 days before the count, starting on March 1) to April 22. The panel containing information on the number of hospitalizations, instead, includes data from February 24 to April 23.

##### France <a name="cap2.2.2"></a>

Data concerning coronavirus-related harm are collected from ’Sante Publique France’ website. This database gives information on the total number of individuals currently hospitalized, on the number of individuals currently in ICU and on the cumulative number of deaths since March 1, 2020. These data are available starting from March 18 for each department and on a daily basis. In order to obtain regional data, we simply aggregated information on hospitalizations and deaths for departments belonging to the same region. Hence, for France, we consider the following outcome variables: total number of individuals currently hospitalized per 100,000 inhabitants; total number of individuals currently in ICU per 100,000 inhabitants; cumulative number of deaths per 100,000 inhabitants. Population data are collected from the INSEE (Institut National de la Statistique et des études économiques) website and refer to population on January 1, 2020. The French panel includes data from February 28 to April 21.

### Results <a name="cap3"></a>

#### Graphical Analysis <a name="cap3.1"></a>

[*Back to Table of Contents*](#tbc)

Results for our graphical analysis are included in Figures 1 to 4. Each figure shows the relationship between our outcome variables (one for each panel of each figure) and the two pollutants, \\(PM_{10}\\) and \\(PM_{2.5}\\), for each country under investigation. For these plots, we consider one date and exploit cross-province or cross-regional variation in pollution and COVID-related outcomes. For each country, we choose the day before the beginning of lockdown for two main reasons: first, confinement measures forced people to stay at home, thus inevitably reducing exposure to pollution. Second, the decision to implement a lockdown policy can be viewed as a signal that the pandemic has reached the country and the number of cases, hospitalizations and deaths started to be considerably high, thus raising concerns for public health.[^3]

Each point on each plot represents one province or region and refers to the real observations. The red line, instead, represent the fitted values, that is, the predictions for the outcome variable from a linear regression of the latter on the independent variable (pollution, in our case).

This set of graphs uncovers a positive relationship between COVID outcomes and pollution. This seems more evident in the two figures concerning France. For example, in panel (b) and (c) of Figure 4, the dots are (almost) all located very close to the red line of fitted values.

Even though this graphical analysis provides suggestive evidence of a positive association between pollution and the virus adverse outcomes, this is limited to only one day and cannot be considered as rigorous as econometric analysis. For this reason, we subsequently perform regression analysis.

#### Econometric Analysis <a name="cap3.2"></a>

[*Back to Table of Contents*](#tbc)

For the regression analysis of this section, we exploit the panel structure of the data described in Section 2. We run separate regressions for each country and each pollutant. The econometric specification is as follows:

$$ log Y_{r, t} =\beta_{0}+\beta_{1} X_{r, t-20}+\alpha_{r}+u_{r, t}, $$

<div class="text-center">
    <figure class="figure">
        <img src="/assets/images/Articles/COVID-19-Pandemic-and-Pollution-Evidence-from-Belgium-and-France/Figure1.png" class="figure-img img-fluid">
    </figure>
</div>

<div class="text-center">
    <figure class="figure">
        <img src="/assets/images/Articles/COVID-19-Pandemic-and-Pollution-Evidence-from-Belgium-and-France/Figure2.png" class="figure-img img-fluid">
    </figure>
</div>

<div class="text-center">
    <figure class="figure">
        <img src="/assets/images/Articles/COVID-19-Pandemic-and-Pollution-Evidence-from-Belgium-and-France/Figure3.png" class="figure-img img-fluid">
    </figure>
</div>


where \\(Y_{r, t}\\) is the COVID-related outcome of interest in province or region \\(r\\) on day \\(t\\); \\(X_{r, t-20}\\) is the pollutant concentration in province or region \\(r\\) at time \\(t-20\\), while \\(\alpha_{r}\\) are the province or region fixed effects. \\(\beta_{1}\\) is the parameter of interest to be estimated. Finally, \\(u_{r, t}\\) is an idiosyncratic error term.

Results are shown in Tables 1 to 4. Each column of each table reports estimates of \\(\beta_{1}\\)for each outcome variable. In our baseline specification (first row of each table), we simply regress \\(Y_{r, t}\\) on the pollutant concentration. This allows us to exploit both cross-regional and time variation. In the second row of each table, we add the province or region fixed effects. This allows us to control for province or region-specific characteristics that do not vary over time. Given our log-level specification, estimates should be interpreted as the percentage variation in the outcome variable associated with a one unit increase in the independent variable. When fixed effects are included, estimated coefficients should be interpreted as the percentage variation in the outcome variable associated with a one unit increase in the independent variable, within a province or region and across time. The estimated coefficients for Belgium are always positive and statistically significant at 1% level. In France, COVID-related outcomes do not seem to be significantly associated with \\(PM_{2.5}\\) concentration. However, there exists a strong positive correlation between the spread of the virus and \\(PM_{10}\\) concentration. Also, note that estimated coefficients are bigger in magnitude for Belgium than for France. In Belgium, an increase of one \\(\mu g/m^3\\) in \\(PM_{2.5}\\) concentration is associated with a 6.8% increase in the number of cases, a 4.1% increase in the number hospitalizations and a 4.2% increase in the number of individuals in ICU. This results are consistent with prior research, even though estimates are smaller than
those found by previous studies in the US (Xiao Wu et al., 2020).

<div class="text-center">
    <figure class="figure">
        <img src="/assets/images/Articles/COVID-19-Pandemic-and-Pollution-Evidence-from-Belgium-and-France/Figure4.png" class="figure-img img-fluid">
    </figure>
</div>

**Table 1: COVID-19 and Particulate Matter 2.5 in Belgium** <a name="tab1"></a>

<div class="table-responsive-md">
<table class='table table-hover'>
    <caption>Note: Robust standard errors in parenthesis.<br><sup>*</sup><i>p</i> < 0.1, <sup>**</sup><i>p</i> < 0.05, <sup>***</sup><i>p</i> < 0.01</caption>
    <thead>
        <tr>
            <th scope='row'></th>
            <th>(1)<br>Cases<br>(100,000 inh.)</th>
            <th>(2)<br>Hospitalizations<br>(100,000 inh.)</th>
            <th>(3)<br>ICU<br>(100,000 inh.)</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th scope='row'>PM 2.5</th>
            <td>0.0633<sup>***</sup><br>(0.0052)</td>
            <td>0.0407<sup>***</sup><br>(0.0048)</td>
            <td>0.0416<sup>***</sup><br>(0.0049)</td>
        </tr>
        <tr>
            <th scope='row'>PM 2.5<br>(Province fixed effects)</th>
            <td>0.0682<sup>***</sup><br>(0.0036)</td>
            <td>0.0410<sup>***</sup><br>(0.0036)</td>
            <td>0.0427<sup>***</sup><br>(0.0045)</td>
        </tr>
        <tr style="solid black">
            <td colspan="4"></td>
        </tr>
        <tr>
            <th scope="row">N</th>
            <td>803</td>
            <td>660</td>
            <td>660</td>
        </tr>
    </tbody>
</table>
</div>

**Table 2: COVID-19 and Particulate Matter 10 in Belgium** <a name="tab2"></a>

<div class="table-responsive-md">
<table class='table table-hover'>
    <caption>Note: Robust standard errors in parenthesis.<br><sup>*</sup><i>p</i> < 0.1, <sup>**</sup><i>p</i> < 0.05, <sup>***</sup><i>p</i> < 0.01</caption>
    <thead>
        <tr>
            <th scope='row'></th>
            <th>(1)<br>Cases<br>(100,000 inh.)</th>
            <th>(2)<br>Hospitalizations<br>(100,000 inh.)</th>
            <th>(3)<br>ICU<br>(100,000 inh.)</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th scope='row'>PM 10</th>
            <td>0.0337<sup>***</sup><br>(0.0033)</td>
            <td>0.0268<sup>***</sup><br>(0.0032)</td>
            <td>0.0265<sup>***</sup><br>(0.0033)</td>
        </tr>
        <tr>
            <th scope='row'>PM 10<br>(Province fixed effects)</th>
            <td>0.0413<sup>***</sup><br>(0.0020)</td>
            <td>0.0272<sup>***</sup><br>(0.0022)</td>
            <td>0.0280<sup>***</sup><br>(0.0029)</td>
        </tr>
        <tr style="solid black">
            <td colspan="4"></td>
        </tr>
        <tr>
            <th scope="row">N</th>
            <td>803</td>
            <td>660</td>
            <td>660</td>
        </tr>
    </tbody>
</table>
</div>

**Table 3: COVID-19 and Particulate Matter 2.5 in France** <a name="tab3"></a>

<div class="table-responsive-md">
<table class='table table-hover'>
    <caption>Note: Robust standard errors in parenthesis.<br><sup>*</sup><i>p</i> < 0.1, <sup>**</sup><i>p</i> < 0.05, <sup>***</sup><i>p</i> < 0.01</caption>
    <thead>
        <tr>
            <th scope='row'></th>
            <th>(1)<br>Deaths<br>(100,000 inh.)</th>
            <th>(2)<br>Hospitalizations<br>(100,000 inh.)</th>
            <th>(3)<br>ICU<br>(100,000 inh.)</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th scope='row'>PM 2.5</th>
            <td>0.0241<br>(0.0204)</td>
            <td>0.0111<br>(0.0099)</td>
            <td>0.0081<br>(0.0088)</td>
        </tr>
        <tr>
            <th scope='row'>PM 2.5<br>(Region fixed effects)</th>
            <td>0.0255<br>(0.0218)</td>
            <td>0.0107<br>(0.0106)</td>
            <td>0.0083<br>(0.0095)</td>
        </tr>
        <tr style="solid black">
            <td colspan="4"></td>
        </tr>
        <tr>
            <th scope="row">N</th>
            <td>1,188</td>
            <td>1,188</td>
            <td>1,188</td>
        </tr>
    </tbody>
</table>
</div>

**Table 4: COVID-19 and Particulate Matter 10 in France** <a name="tab4"></a>

<div class="table-responsive-md">
<table class='table table-hover'>
    <caption>Note: Robust standard errors in parenthesis.<br><sup>*</sup><i>p</i> < 0.1, <sup>**</sup><i>p</i> < 0.05, <sup>***</sup><i>p</i> < 0.01</caption>
    <thead>
        <tr>
            <th scope='row'></th>
            <th>(1)<br>Deaths<br>(100,000 inh.)</th>
            <th>(2)<br>Hospitalizations<br>(100,000 inh.)</th>
            <th>(3)<br>ICU<br>(100,000 inh.)</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th scope='row'>PM 10</th>
            <td>0.0353<sup>***</sup><br>(0.0071)</td>
            <td>0.0139<sup>***</sup><br>(0.0049)</td>
            <td>0.0100<sup>**</sup><br>(0.0046)</td>
        </tr>
        <tr>
            <th scope='row'>PM 10<br>(Region fixed effects)</th>
            <td>0.0403<sup>***</sup><br>(0.0062)</td>
            <td>0.0155<sup>***</sup><br>(0.0040)</td>
            <td>0.0117<sup>***</sup><br>(0.0039)</td>
        </tr>
        <tr style="solid black">
            <td colspan="4"></td>
        </tr>
        <tr>
            <th scope="row">N</th>
            <td>1,188</td>
            <td>1,188</td>
            <td>1,188</td>
        </tr>
    </tbody>
</table>
</div>

### Conclusion <a name="cap4"></a>

[*Back to Table of Contents*](#tbc)

This paper corroborates existing evidence linking pollution levels to COVID-19 pandemic propagation. Together with prior research, our results suggest that pollution may be an important factor contributing to the diffusion of the virus that policy-makers should take into account.

It is important to note that our study has some limitations. First, our econometric analysis does not identify causal effects. We believe that reverse causality does not represent an important issue here.[^4] However, an omitted-variable problem may persist: even though our specification with province or region fixed effects allows us to control for province or region-specific characteristics that do not vary over time, there may still exist some time-varying local characteristics that are spuriously correlated with pollution and, hence, would bias our estimates.

Second, the use of up-to-date pollution data has pros and cons. On the one hand, these data allow us to exploit recent daily information. On the other hand, although the European Environment Agency (EEA) is a reliable source, this information is not revised. Indeed, the data received by the EEA from each sampling point in each member state are revised and made publicly available with one-year delay. In more detail, in September of each year, the EEA publishes revised data concerning the previous year: hence, pollution data for 2020, for example, will be available in September 2021.

Fighting the current pandemic requires a better understanding of the disease and corresponding propagation mechanisms. More research on this topic is welcome.

### References <a name="cap5"></a>

[*Back to Table of Contents*](#tbc)

[1] Ginsburgh, V., Magerman, G. and Natali, I. (2020), COVID-19 and the Role of Economic Conditions in French Regional Departments. *Working Papers ECARES 2020-17, ULB (Université Libre de Bruxelles*.

[2] Office for National Statistics (2020),
[https://www.ons.gov.uk/peoplepopulationandcommunity/birthsdeathsandmarriages/deaths/bulletins/deathsinvolvingcovid19bylocalareasanddeprivation/deathsoccurringbetween1marchand17april](https://www.ons.gov.uk/peoplepopulationandcommunity/birthsdeathsandmarriages/deaths/bulletins/deathsinvolvingcovid19bylocalareasanddeprivation/deathsoccurringbetween1marchand17april). Last access: June, 2020.

[3] Setti, L., Passarini, F., De Gennaro, G., Barbieri, P., Perrone, M. G., Borelli, M., Palmisani, J., Di Gilio, A., Torboli, V., Fontana, F., Clemente, L., Pallavicini, A., Ruscio, M., Piscitelli, P., Miani, A. (2020), SARS-Cov-2RNA found on particulate matter of Bergamo in Northern Italy: First evidence. *Environmental Research*.

[4] SIMA, Società Italiana di Medicina Ambientale (2020),
[https://www.simaonlus.it/?page_id=694](https://www.simaonlus.it/?page_id=694). Last access: June, 2020.

[5] WHO, World Health Organization (2013), Health effects of particulate matter.
Policy implications for countries in eastern Europe, Caucasus and central Asia.
[https://www.euro.who.int/__data/assets/pdf_file/0006/189051/Health-effects-of-particulate-matter-final-Eng.pdf](https://www.euro.who.int/__data/assets/pdf_file/0006/189051/Health-effects-of-particulate-matter-final-Eng.pdf). Last access: June, 2020.

[6] Xiao Wu, M.S., Nethery, R. C., Sabath, M. B., Braun, D. and Dominici, F. (2020), Exposure to air pollution and COVID-19 mortality in the United States.

### Additional Material <a name="cap6"></a>

[*Back to Table of Contents*](#tbc)

In this appendix, we provide an alternative version of Figure 1 in the main text. We still consider the number of cases, hospitalizations and individuals in ICU and the pollutant PM 2.5, but we now apply a time lag of 15 days between the observation of the pollutant concentrations and the measures of COVID-related harm.

<div class="text-center">
    <figure class="figure">
        <img src="/assets/images/Articles/COVID-19-Pandemic-and-Pollution-Evidence-from-Belgium-and-France/Figure5.png" class="figure-img img-fluid">
    </figure>
</div>

[^1]: For England and Wales, see Office for National Statistics. For France, see Ginsburgh, Magerman and Natali (2020).

[^2]: Note that the indices refer to the diameter of the particles. \\(PM_{10}\\) stands for inhalable particles with a diameter of 10 microns or smaller, while \\(PM_{2.5}\\) indicates particulate matter of diameter of 2.5 microns or smaller.

[^3]: Note that observations on the pollutants’ concentrations refer to the day before the lockdown and, hence, the corresponding observations for COVID-related outcomes refer to 20 days after lockdown. In appendix A, we also provide a version of Figure 1 for a time lag of 15 days.

[^4]: Reverse causality issue should be minimized by the use of lagged values of pollution.
