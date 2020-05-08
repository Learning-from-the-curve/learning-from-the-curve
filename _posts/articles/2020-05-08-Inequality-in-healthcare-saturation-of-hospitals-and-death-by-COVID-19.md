---
layout: post
title: "Inequality in healthcare: saturation of hospitals and death by COVID-19"
date: 2020-05-08 12:00:00 +0100
category: articles
---

**Authors:** Stefano Falcone ([ECARES](https://ecares.ulb.be/?option=com_content&task=view&id=136&Itemid=95); [Université Libre de Bruxelles](https://www.ulb.be/); e-mail: Stefano.Falcone@ulb.be) and Elisa Navarra ([ECARES](https://ecares.ulb.be/?option=com_content&task=view&id=136&Itemid=95); [Université Libre de Bruxelles](https://www.ulb.be/); e-mail: Elisa.Navarra@ulb.be).[^1]

[^1]: We thank Glenn Magerman, Federico Gallina and other members of [*Learning from the curve*](https://learning-from-the-curve.netlify.app/about/)

The spread of COVID-19 pandemic has put healthcare systems around the world under strain. Is there any relationship between the burden on hospital facilities and the number of deaths by COVID-19?

In this study, we exploit regional variation in the Italian healthcare system and the severity of the contagion to provide suggestive evidence that well-equipped intensive care units (ICUs) can save human lives from deaths by COVID-19. We show that this result holds even when controlling for possible confounding factors and that the relationship is not linear: one additional intensive care bed (IC) is more strongly associated with fewer deaths by COVID-19 when ICUs are more extremely saturated.

<!--more-->

To grasp the intuition of this relationship, in Figure (a) we plot the number of beds in ICUs (per 100 infected patients) against the number of total deaths by COVID-19 (per 100 infected patients) as of April 30, 2020. By dividing both the number of deaths and the number of IC beds by the number of total infected, we are conditioning on the severity of the contagion which spread faster in Northern regions. A spurious correlation between number of deaths and number of IC beds would in fact be positive, since Northern regions were more severely hit by COVID-19 and their ICUs already better equipped before the start of the crisis than those in the Centre and South of Italy. The association between ICUs' potential saturation rate and COVID-19's mortality rate is negative and statistically significant at the 1% level (Table 1, column 1): 1 additional IC bed (per 50 infected patients) is associated with 1 saved life (per 100 infected patients). However, this linear correlation masks a strong heterogeneity across Italian regions, with a tighter association in regions where the saturation of ICUs hits more severely.

The association between the strain on ICUs and deaths by COVID-19 is confirmed when looking at the effective burden on ICUs (namely, IC beds per infected in ICU). Weighting the number of IC beds by the number of infected patients in ICUs allows us to rely on a more comparable measure of ICUs' saturation across regions. In fact, the total infected statistics might vary also due to differences in unobservable characteristics of tests and testing procedures. In Figure (b), we plot total deaths (per infected in ICU) against IC beds (per infected in ICU). We use the number of infected in ICUs at its regional peak, so that the selected date may be different across regions. As in Figure (a), the correlation is only significant at the 10% significance level. However, this correlation masks a strong heterogeneity across regions, with IC beds more strongly associated with deaths by COVID-19 when intensive care facilities are more extremely saturated.

While highlighting a significant positive correlation between saturation of IC beds and COVID-19 mortality, Figures (a) and (b) also suggest a geographical clustering of regions in mildly and extremely saturated ones. We define as mild saturation, regions with 6 or more IC beds per 100 infected and extreme saturation those with less than 6 IC beds per 100 infected patients (for Figure (b), these are, respectively, 2 or more IC beds per infected in ICU, and less than 2). Mildly and extremely saturated regions are the same in per-100-infected and per-infected-in-ICU terms, with the exception of Friuli-Venezia Giulia (extreme only in the first measure) and Puglia (extreme only in the second measure). The severity of ICU saturation almost overlaps with the geographical clustering in Northern versus Central and Southern regions: in fact, healthcare facilities are under a heavier strain in the North due to the more dramatic spread of COVID-19 in that part of Italy, despite the pre-existing higher number of IC beds per capita. Given this geographical clustering, we considered appropriate to produce heteroscedasticity-consistent standard error and control for socioeconomic indicators that could confound the associations shown in the Figure. Outcome variables, regressors of interest and selected controls are listed in Table 1, showing mean differences between extreme and mild saturation regions, defined in per-100-infected terms. Only the difference in life expectancy is statistically significant at 5% level, which makes it a good candidate as control.[^2] The inclusion of controls in our regressions confirms that ICUs' saturation is a statistically significant predictor of COVID-19 mortality (Table 1, columns 2 and 6). In addition, the magnitude of the relationship is higher with controls, pointing to a downward confounding due to extremely saturated regions being also characterized by a longer life expectancy. For a given public health expenditure, availability of physicians and life expectancy of the population, one additional bed (per 60 infected) can save 1 extra life (per 100 infected), while 3 additional beds (per infected in ICU) can save 2 human lives (per infected in ICU).

[^2]: The unshown balance test using mild and extreme defined over infected-in-ICU terms yields qualitatively identical results.

To further investigate the heterogeneity of the correlation, in columns (3)-(4) and (7)-(8) of Table 2, we show separately results for mild and extreme saturation regions. In both cases, we find that the correlation between saturation of ICUs and COVID-19 mortality is strongly significant for extremely saturated regions and not significant for less saturated regions. When using per-100-infected variables, the magnitude of the correlation is around 5 times stronger in regions extreme than for the whole sample, while it is 6 times higher for per-infected-in-ICUs variables. In extremely saturated regions, 1 additional IC bed (per 60 infected in ICU) is correlated with 5 saved lives (per 100 infected patients), while 3 additional beds (per infected in ICU) can save 12 lives (per infected in ICU). This confirms that the burden on ICUs is more detrimental in regions where the saturation of ICUs hits more severely.

Although these correlations do not necessarily unveil causal relationships, our results provide preliminary evidence of a non-linear positive link between ICUs saturation and deaths by COVID-19. Our findings hold even when considering the new IC beds built with great effort in the last weeks (result not shown here). If the causal nature of these associations is confirmed and in view of a potential second wave of COVID-19, then investing in ICUs and hospital equipment could contribute to reduce the lethality of the disease. Given the lower number of IC beds per capita in the South than in the North of Italy, due also to new equipment having being built in the last weeks in more severely hit regions, our results suggest that the cost in terms of human lives in the South would be dramatically higher than in the North shall the second wave of COVID-19 hit with equal severity across the national territory. Moreover, our study provides evidence in favor of policies directed to the relocation of patients from extremely to mildly saturated regions.

**Figure**

![](/assets/images/Articles/Inequality-in-healthcare-saturation-of-hospitals-and-death-by-COVID-19/total.png)

<small><i>Note: </i>Deaths is the total number of deaths by COVID-19 as of April 30, 2020. ICU beds is the total number of beds in ICUs in 2018. Variables in per-100-infected terms are divided by the total number of infected times 100.</small>

<small><i>Data source: </i> Protezione Civile (Deaths and infected by COVID-19); Ministry of Health (ICU beds).</small>

**Table 1: Balance Test**

<table class='table table-hover'>
    <thead>
        <tr>
            <th scope='col'></th>
            <th scope='col'>Mean <i>Extreme</i></th>
            <th scope='col'>Mean <i>Mild</i></th>
            <th scope='col'>Difference</th>
            <th scope='col'>p-value</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th scope='row'>Deaths per 100 infected</th>
            <td>11.533</td>
            <td>7.872</td>
            <td>3.661</td>
            <td>0.012</td>
        </tr>
        <tr>
            <th scope='row'>Deaths per infected in ICU</th>
            <td>5.323</td>
            <td>2.604</td>
            <td>2.719</td>
            <td>0.009</td>
        </tr>
        <tr>
            <th scope='row'>ICU beds per 100 infected</th>
            <td>2.657</td>
            <td>10.840</td>
            <td>-8.183</td>
            <td>0.000</td>
        </tr>
        <tr>
            <th scope='row'>ICU beds per infected in ICU</th>
            <td>1.100</td>
            <td>3.623</td>
            <td>-2.523</td>
            <td>0.000</td>
        </tr>
        <tr>
            <th scope='row'>Life expectancy</th>
            <td>83.235</td>
            <td>82.530</td>
            <td>0.705</td>
            <td>0.018</td>
        </tr>
        <tr>
            <th scope='row'>Public health exp. per capita</th>
            <td>1,914.156</td>
            <td>1,865.410</td>
            <td>48.746</td>
            <td>0.405</td>
        </tr>
        <tr>
            <th scope='row'>Physicians per 1,000 inh.</th>
            <td>3.950</td>
            <td>4.096</td>
            <td>-0.146</td>
            <td>0.472</td>
        </tr>
        <tr style="solid black">
            <td colspan="5"></td>
        </tr>
        <tr>
            <th scope= 'row'>Observations</th>
            <td colspan='4' style="text-align:center">20</td>
        </tr>
    </tbody>
</table>
<small><i>Note: </i>Mean <i>Extreme</i> reports the mean of listed variables in regions with less than 6 IC beds per 100 infected patients. Mean <i>Mild</i> reports the mean of listed variables regions with 6 or more IC beds per 100 infected patients. Difference calculates the difference between Mean <i>Extreme</i> and Mean <i>Mild</i>. p-value reports the p-value for the t-test on the difference of the means. Deaths is the total number of deaths by COVID-19 as of April 30, 2020. ICU beds is the total number of beds in ICUs in 2018. Variables in per-100-infected terms are divided by the total number of infected times 100. All variables in per-infected-in-ICU are divided by the number of infected patients in ICU at its regional peak. Life expectancy is the regional life expectancy at 0 to 4 years old in 2018. Public health exp. per capita is the regional public health current expenditure in euros divided by regional population in 2016. Physicians per 1,000 inh. is the regional total number of physicians (generalists and specialists) per 1,000 inhabitants in 2017.</small>

<small><i>Data source: </i>Protezione Civile (Deaths and infected by COVID-19); Ministry of Health (ICU beds); Italian National Institute of Statistics (Physicians per 1,000 inh., Life expectancy, Public health exp. per capita).</small>

**Table 2: Table**

<table class='table table-hover'>
    <thead>
        <tr>
            <th scope='col'></th>
            <th colspan='4' style="text-align:center">Deaths per 100 infected<hr></th>
            <th colspan='4' style="text-align:center">Deaths per infected in ICU<hr></th>
        </tr>
        <tr>
            <th scope='row'></th>
            <th>(1)</th>
            <th>(2)</th>
            <th>(3)</th>
            <th>(4)</th>
            <th>(5)</th>
            <th>(6)</th>
            <th>(7)</th>
            <th>(8)</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th scope='row'>Beds (infected)</th>
            <td>-0.512<sup>***</sup><br>(0.107)</td>
            <td>-0.599<sup>***</sup><br>(0.128)</td>
            <td>-0.334<br>(0.238)</td>
            <td>-2.882<sup>**</sup><br>(0.832)</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th scope='row'>Beds (ICU)</th>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td>-0.635<sup>*</sup><br>(0.314)</td>
            <td>-0.712<sup>*</sup><br>(0.388)</td>
            <td>0.195<br>(0.369)</td>
            <td>-4.272<sup>**</sup><br>(1.648)</td>
        </tr>
        <tr>
            <th scope='row'>Life expectancy</th>
            <td></td>
            <td>-0.814<br>(0.872)</td>
            <td>0.190<br>(0.849)</td>
            <td>1.618<br>(1.245)</td>
            <td></td>
            <td>0.193<br>(0.735)</td>
            <td>1.122<br>(1.407)</td>
            <td>0.0584<br>(1.110)</td>
        </tr>
        <tr>
            <th scope='row'>Health exp.</th>
            <td></td>
            <td>-0.00419<br>(0.00471)</td>
            <td>-0.00268<br>(0.00516)</td>
            <td>-0.00132<br>(0.00565)</td>
            <td></td>
            <td>-0.00383<br>(0.00374)</td>
            <td>-0.00274<br>(0.00540)</td>
            <td>-0.00836<br>(0.00509)</td>
        </tr>
        <tr>
            <th scope='row'>Physicians</th>
            <td></td>
            <td>-0.247<br>(1.157)</td>
            <td>-0.401<br>(1.607)</td>
            <td>3.336<br>(1.847)</td>
            <td></td>
            <td>0.497<br>(1.260)</td>
            <td>0.657<br>(1.451)</td>
            <td>1.549<br>(1.725)</td>
        </tr>
        <tr style="solid black">
            <td colspan="9"></td>
        </tr>
        <tr>
            <th scope= 'row'>Observations</th>
            <td>20</td>
            <td>20</td>
            <td>8</td>
            <td>12</td>
            <td>20</td>
            <td>20</td>
            <td>8</td>
            <td>12</td>
        </tr>
        <tr>
            <th scope= 'row'>Mean Dep. Var.</th>
            <td>10.07</td>
            <td>10.07</td>
            <td>7.872</td>
            <td>11.53</td>
            <td>4.234</td>
            <td>4.234</td>
            <td>2.870</td>
            <td>5.142</td>
        </tr>
        <tr>
            <th scope= 'row'>Sample</th>
            <td>All</td>
            <td>All</td>
            <td>Mild</td>
            <td>Extreme</td>
            <td>All</td>
            <td>All</td>
            <td>Mild</td>
            <td>Extreme</td>
        </tr>
    </tbody>
</table>
<small>Standard errors in parentheses. <sup>*</sup><i>p</i> < 0.10, <sup>**</sup><i>p</i> < 0.05, <sup>***</sup><i>p</i> < 0.01.</small>

<small><i>Note: </i>In regressions (1) to (4), Deaths per 100 infected is the total number of deaths by COVID-19 (per 100 infected patients) as of April 30, 2020. In regressions (5) to (8), Deaths per infected in ICU is the total number of deaths divided by the number of infected patients in ICUs at its regional peak. Beds (infected) is the total number of beds in ICUs in 2018 per 100 infected patients. Beds (ICU) is the total number of beds in ICUs in 2018 per infected patient in ICU. Life expectancy is regional life expectancy at 0 to 4 years old in 2018. Health exp. is the regional public health current expenditure in euro divided by regional population in 2016. Physicians is the regional total number of physicians (generalists and specialists) per 1,000 inhabitants in 2017. Mean Dep. Var. reports the average number of deaths per 100 infected and the average number of deaths per infected in ICUs for the regression samples. Regressions (1) and (5) do not include controls. Regressions (1), (2), (5), (6) are run over the entire sample. Regressions (3) and (7) are run over the Mild subsample defined, respectively, as regions with 6 or more IC beds per 100 infected, and regions with 2 or more IC beds per infected in ICU. Regressions (4) and (8) are run over the Extreme subsample defined, respectively, as regions with less than 6 IC beds per 100 infected, and regions with less than 2 IC beds per infected in ICU. Robust standard errors in parenthesis.</small>

<small><i>Data source: </i>Protezione Civile (Deaths and infected by COVID-19); Ministry of Health (ICU beds); Italian National Institute of Statistics (Physicians per 1,000 inh., Life expectancy, Public health exp. per capita).</small>
