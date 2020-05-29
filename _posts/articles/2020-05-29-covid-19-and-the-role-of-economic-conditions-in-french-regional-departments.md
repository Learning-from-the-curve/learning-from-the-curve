---
layout: post
title: "Covid-19 and the Role of Economic Conditions in French Regional Departments"
date: 2020-05-29T09:00:00.021Z
category: articles
summary: "The recent outbreak of Covid-19 has infected the world at an incredible speed. While
there are many similarities across countries in terms of the characteristics of the epidemic
spread, there are also large differences across regions. In this paper, we examine regional
variation in the outbreak across continental France. We use information on the number of
deaths and discharged patients from Covid-19 and socio-economic variables at the department
level. Controlling for other factors, we corroborate existing evidence that, unfortunately,
inequality kills: departments with more inequality face a higher incidence rate of
the disease, expressed as the number of deaths and discharged (gravely ill) patients. Using
covariance analysis combining both deaths and releases, we find no statistically differential
relationship across factors that contribute to deaths or recoveries."
author:
  - V. Ginsburgh
  - G. Magerman
  - I. Natali
---

**Table of Contents**:<a name="tbc"></a>

1. [Introduction](#cap1)
2. [The econometric model and data](#cap2)
3. [Results](#cap3)
4. [Analysis of Covariance](#cap4)
5. [Conclusions](#cap5)
6. [References](#cap6)
7. [Tables](#cap7)
8. [Figures](#cap8)

-------------------------------------

### Introduction <a name="cap1"></a>

[*Back to Table of Contents*](#tbc)

The outbreak of the Covid-19 pandemic has found both the scientific
community and the general public unprepared. Its rapid spread and the
skyrocketing number of individuals dying for the virus have caused deep
concerns, profound uncertainty and anxiety around the globe. The
pandemic not only affects individual health and health care systems, but
also economic and sociologic ecosystems. Flattening the curve affects
our behavior, but our behavior also affects the curve. In this paper, we
aim at understanding how existing socio-economic disparities might
contribute to differences in the spread of the virus.

Our concern is to study whether regional variations in socio-economic
conditions (poverty level, education level, density of doctors), as well
as geographic circumstances (the East and North-east borders with
Germany, Luxembourg and Belgium) have an influence on the pattern of the
pandemic in continental France.[^1] Figures [1](#fig1) and [2](#fig2) show the 94 French
continental departments, and the intensity of the outbreak in these
regions. [Figure 1](#fig1) depicts the total number of Covid deaths by department
on April 20, 2020. [Figure 2](#fig2) shows the total number of discharged Covid
patients on the same day. Clearly, the North (Belgian and Luxembourg
borderline) and North-East regions have been hit harder, relative to the
South-West areas, as can be explained by the initial hotbeds of Alsace
and Bas-Rhin (Low Rhine) regions. France recently decided to pursue
confinement in the Eastern regions as well as in Paris and its
surrounding departments, but unlock in the Western and central parts of
the country. On May 5, 2020, the President of the Bas-Rhin department in
Alsace claimed that it would be ‘pure madness’ to unlock his department.
The French Prime-Minister unveils, at the same time, that France ‘is cut
into two pieces’ (Huffpost, 2020). Hervé le Bras (2020), researcher at
the Institut national d’études démographiques, analyzed the dynamics of
the pandemic, comparing how the virus developed in two regions: the
Haut-Rhin department, where the number of cases of Covid is large and
somewhat out of control, and Bouches-du-Rhône in the South, where the
epidemic took off much later.

In this paper, we use information on socio-economic variables and Covid
data to understand how socio-economic variation might contribute to
these differences. We implement a simple estimation setup, with lagged
socio-economic indicators (year 2017), and current Covid data (April
2020). We do not look at the dynamics, nor at demographic variation at
the regional level. We run regressions of both deaths and discharged (D
& D in what follows) separately, as well as together (using an analysis
of covariance framework) on a certain number of departmental geographic
and socio-economic characteristics, such as total population, Gini
coefficients to measure inequality, level of education, and doctors’
density.

Unfortunately, it was not possible to know with certainty the exact
moment at which the epidemic started in each department. Though some
figures on cases are available, this information is rather scant before
March 18, 2020. In addition, it may have been difficult for public
authorities themselves to identify the so-called ‘patient 0.’ This
poses, of course, reliability issues for data proceeding March 18.
However, we downloaded data on the cumulative number of deaths and
patients discharged from hospitals on April 20 when both authorities and
the general public were well aware of the pandemic and the collection of
data had become more rigorous and well organized. The problem here is
that the number of days between ‘patient 0’ and April 20, is not the
same in all departments. It is even suggested that a few cases of Covid
appeared in France in December 2019, or even earlier on November 16,
2019, long before blazing, in the department of Haut-Rhin (Peillon,
2020).[^2]

The paper is organized as follows. In Section 2, we describe the
econometric model and the variables that are used. Section 3 is devoted
to econometric results, and Section 4 concludes.

### The econometric model and data <a name="cap2"></a>

[*Back to Table of Contents*](#tbc)

We believe that, in this specific context, reverse causality is not an
issue, though our results do not identify causal effects since an
omitted-variable problem may still exist. The econometric model we use
is simple. We regress the number of Covid deaths and discharged from
hospitals on departmental variables:

$$y_{ik}= R_i\alpha_k + X_i\beta_k + \epsilon_{ik}, i =1,..., 94; k= 1,2,$$

where \\(i\\) is one of the 94 departments, \\(y_{ik}\\) is either the
number of deaths (\\(k=1\\)) or of discharged inhabitants (\\(k=2\\)) in
department \\(i\\), \\(R_i\\) is a vector of two dummy variables which
represent geographical characteristics (Northern and Eastern France, and
Ile de France, that is Paris and its surroundings), \\(X_i\\) is a vector
of departmental socio-economic characteristics, \\(\alpha_k\\) and
\\(\beta_k\\) are vectors of parameters and \\(\epsilon_{ik}\\) is the error
term. Variables \\(y_{ik}\\) and population, which is one of the variables
in vector \\(X_i\\), are expressed in logarithms.

The dependent variables were downloaded on April 20 from the website
Santé Publique France. The choice we had was to take the more recent
data at the time we started our analysis, though they were slightly
declining afterwards. We chose the high point of the pandemic.

The vector of two dummy variables \\(R_i\\) includes the following
borders: (a) Northern and Eastern departments that have a border with
Southern Belgium, Luxembourg and Germany,[^3] as well as (b) Ile de
France, a group of departments, with Paris (75) as center.[^4]

Data for the variables in vector \\(X_i\\) are all downloaded from the
INSEE (Institut National de Statistique et des Etudes Economiques)
website and include: number of inhabitants in logs, Gini coefficient,
basic education,[^5] number of doctors per 100,000 inhabitants.

We ran five regression for D & D, by introducing variables one after the
other, in the order described above. The first two contain the dummies
*North-East* and *Ile de France*; next comes
population,[^6] inequality within regions measured by the Gini
coefficient, education and density of doctors.

### Results <a name="cap3"></a>

[*Back to Table of Contents*](#tbc)

#### Baseline Regressions

Results appear in Tables [1](#tab1) (for deaths) and [2](#tab2) (for discharged) and are
very similar across the two tables. Clearly, the North-Eastern border
and Ile de France (column 1) have the largest number of D & D people.
This may be partly due to the fact that departments in the North-East
and, especially, in Ile de France, which includes Paris and the
surrounding departments, are among the most populated ones. This becomes
obvious in column (2), where we add the variable population, which
causes a drop in the magnitude of the coefficients for both dummies (and
a larger drop for the dummy *Ile de France*). Despite this, coefficients
picked up by the two dummies remain significantly different from 0 at
the 0.01 probability level. Population only can thus not fully capture
the extension of the virus in these two regions.

Next, we add the Gini coefficient. In both regressions the variable
picks up positive effects that are all significantly different from 0,
at the 0.01 or 0.05 probability level. This means that a larger level of
inequality is associated with a larger number of deaths and severely ill
individuals. This is an important result and seems to be in line with
previous findings in the UK. According to an article published on *The
Guardian*, poorer areas in England and Wales are significantly more
affected by the pandemic, with twice a death toll as more affluent
neighborhoods. This may be due to a few reasons: for instance,
individuals in a disadvantaged economic status are more likely to have
pre-existing conditions, they are more likely to live in worse quality
housing, they are more likely to have jobs that cannot be done through
smart-working (by staying at home). These are, evidently, factors that
contribute to expose more the most vulnerable populations to the virus.

The effect of poor education, as described earlier, is probably
overshadowed by the effect of inequality, that is, large differentials
in incomes within each department. People without higher education are
likely to remain poor. The coefficients picked up by the variable are
not significantly different from 0.

Finally, we get to those who have been of great help in the corona
pandemic. One expects that more physicians per inhabitant would help
containing the outbreak, by allowing people to enter a hospital quickly
enough and by providing them with the necessary treatment. Indeed, here,
the density of doctors (both generalists and specialists) is negatively
associated to both the number of deaths and the number of individuals
severely affected by the virus, as proxied by the number of discharged.
The coefficients are, however, not statistically different from zero,
which may be due to the presence of some other (confounding) factors
that we are not taking into account.

#### Analysis of Covariance <a name="cap4"></a>

[*Back to Table of Contents*](#tbc)

The estimated parameters displayed in Tables [1](#tab1) and [2](#tab2) do not seem to be
very different, though [Table 1](#tab1) deals with death, while [Table 2](#tab2) deals
with those who were discharged from hospitals. To check whether they are
significantly different, we opted using an analysis of covariance, which
implicitly assumes that the distribution of errors is the same in both
subsamples (D & D). The model is now:

$$y_{i0}= R_0 \alpha_0 + X_0\beta_0  +  \delta R_0\alpha +  \delta X_0\beta + \epsilon_{i0}, i =1,..., 186.$$

In this formulation, \\(y_{i0}\\) is a vector constructed by piling up
each department’s deaths followed by each department’s discharged and is
regressed on a matrix \\(R_0\\) formed by piling up two matrices \\(R_i\\).
Matrix \\(X_0\\) is constructed in the same way by repeating twice
\\(X_i\\). Finally, \\(\delta\\) is a dummy variable equal to 1 for
observations related to \\(y_{i1}\\), that is, deaths, and 0 for
discharged. The coefficients on the interaction terms \\(\delta R_{0}\\)
and \\(\delta X_{0}\\) will tell us whether the effect of the covariates
is different for deaths and discharged.[^7] The results that we now
analyze can be found in [Table 3](#tab3).

As can be checked, the coefficients picked up by the variables
North-East, Ile de France, Population, Gini, Education and Doctors’
density, as well as the value of the intercept, are exactly the same as
those in [Table 2](#tab2). This is due to the fact that our dummy, \\(\delta\\), is
equal to zero for discharged and, hence, these coefficients pick the
effect of the covariates on the number of discharged individuals. Those
coefficients that were significantly different from 0 remain so, and
those that were not, remain so as well. Standard errors are also
approximately the same.

The estimates for \\(\alpha\\) and \\(\beta\\), instead, will tell us the
difference in the effect of each independent variable across the two
groups (deaths and discharged). To make this clearer, consider the
following example: in Equation (5), results show that the effect of
North-Eastern regions is equal to 0.955 for the group of discharged (as
in [Table 2](#tab2)), to which 0.242, picked up by the interaction
\\(\delta R_0\\), should be added for those who died. The sum is equal to
1.197 and it is identical to the coefficient associated to North-East in
column 5 of [Table 1](#tab1). This shows that the coefficient associated to each
interaction term will yield the difference in the effect of each
covariate across the two groups: if this coefficient is not
statistically different from zero, we conclude that this difference is
not significant.

The estimates of \\(\alpha\\) (associated to the interactions
North-East\*Dummy and Ile de France\*Dummy) are positive and
significantly different from 0 at the 0.01 or 0.05 level, which implies
that they increase the role of the two regions for those who have died,
in all regressions.

The effect of Population is common across the two groups (D & D) since
the coefficient for Dummy\*Population is not significantly different
from 0. Analogous reasoning applies to the Gini since the Dummy\*Gini
coefficients are not different from zero. Finally, Education and
Doctors’ density do not contribute to the fits. It is also interesting
to note that the coefficient for Dummy\*Intercept is negative (but small
and not significantly different from 0 in Equations (2) and (3)) which
indicates that the number of deaths is (fortunately) smaller that the
number of discharged, on average.

It is also worth noting that all fits of equations (3) to (5) are good
since the adjusted \\(R^2\\) are larger than 0.65 and increase to 0.73 in
the analysis of covariance in [Table 3](#tab3).

### Conclusions <a name="cap5"></a>

[*Back to Table of Contents*](#tbc)

There is a clear pattern of heavy infections (deaths and discharged
patients) along the French border with Belgium, Luxembourg and Germany,
and in the departments that surround Paris. It is not clear whether the
effect of the border is due to the countries that border France (and
people passing from one country to the other), or to a cause that we did
not find. This is different for Ile de France with over 12 million
inhabitants, who, before confinement, were traveling, usually using
metros or trains in and out of Paris, where they work (or vice-versa).
Note that more recently, that is, after inputting the numbers of D & D,
the virus moved to more central and western regions,[^8] though with
less virulence than in the North-East and Ile de France. We will need,
however, to wait a couple of weeks, to check whether this will remain
milder.

The fact that population is related to D & D is obvious, but far from
being the only factor, as we showed above.

Finally, it should be clear that more inequality means that the
population is not homogeneous, and that richer people live in one part
of a town or a village, are probably more careful, and may have gardens
to be able to breath, while poor people have little choice, live in
another part of the town and are more likely to walk on the street and
in parks. This is what a British report also points out (Improvement
Service, 2020, p. 3):

> "People living in socio-economic disadvantage are more likely to be
> working in the low paying jobs which are keeping the country going in
> supermarkets, as cleaners, delivery drivers and home care workers, and
> a significant proportion of these low paid workers will be women. The
> four ‘C’s’ of cleaning, care, cashiering and catering, commonly seen
> as women’s work are now massively important, and those working in
> these areas are being exposed daily to the risk of contracting
> Covid-19."

They are also more likely to have lost (at least for some time) their
job, which is a very grim perspective.

As we said, the estimated coefficients picked up by education, which are
not significantly different 0, are probably in the shadow of unequal
incomes measured by the Gini coefficient. The fraction of poor people
who usually have a low level of education are less likely to escape the
pandemic.

Most crises are likely to increase inequality, given increases in the
rate of unemployment and lower wages that follow, as well as
difficulties to get loans from banks to pay their mortgage, even if they
are only temporary. And Covid-19 will probably not be different. This
means that the pandemic hits harder areas in socio-economic disadvantage
today and will probably exacerbate disparities in the near future
(Furceri et al., 2020). This highlights the importance of policy
interventions aimed at helping individuals living in poor conditions, in
order to (i) attenuate the impact of the pandemic today and (ii)
attenuate the (potential) negative consequences of the pandemic in the
near future.  

### References <a name="cap6"></a>

[*Back to Table of Contents*](#tbc)

Furceri, D., Loungani, P. L., Ostry, J. D. and Pizzuto, P. (2020). COVID-19 will raise inequality if past pandemics are a guide. *VOX CEPR Policy Portal* [web: last accessed May 20, 2020].

Le Bras, Hervé (2020). On entrevoit trois stades de l’épidémie de Covid-19 en France. *Le Monde*, April 30, 2020.

Huffpost (2020). Déconfiner les départements rouges? De la ‘pure folie’ pour le président du Bas-Rhin, *Le HuffPost*, May 8, 2020.

Improvement Service (2020), Poverty, inequality and Covid-19 [web: last accessed May 20, 2020].

Peillon, Luc (2020). L’origine de l’épidémie de Covid en France peut-elle remonter à l’automne 2019? *Libération*, 21 mai 2020.

Pidd, H., Barr, C. and Mohdin, A. (2020). Calls for health funding to be prioritised as poor bear brunt of COVID-19. *The Guardian*, May 1, 2020.

### Tables <a name="cap7"></a>

[*Back to Table of Contents*](#tbc)

**Table 1: Regression Results. Number of Deaths.** <a name="tab1"></a>

<div class="table-responsive-md">
<table class='table table-hover'>
    <caption>Note: Two of the 94 departments had no deaths on the 20th of April.<br>Robust standard errors in parenthesis. <sup>*</sup><i>p</i> < 0:1, <sup>**</sup><i>p</i> < 0:05, <sup>***</sup><i>p</i> < 0:01</caption>
    <thead>
        <tr>
            <th scope='row'></th>
            <th>(1)</th>
            <th>(2)</th>
            <th>(3)</th>
            <th>(4)</th>
            <th>(5)</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th scope='row'>North-East</th>
            <td>1.78493<sup>***</sup><br>(.4041796)</td>
            <td>1.362145<sup>***</sup><br>(.2496312)</td>
            <td>1.320606<sup>***</sup><br>(.2371874)</td>
            <td>1.199691<sup>***</sup><br>(.2474712)</td>
            <td>1.196585<sup>***</sup><br>(.2473837)</td>
        </tr>
        <tr>
            <th scope="row">Ile de France</th>
            <td>2.658232<sup>***</sup><br>(.2022909)</td>
            <td>1.434573<sup>***</sup><br>(.1942773)</td>
            <td>1.212202<sup>***</sup><br>(.1892048)</td>
            <td>1.402966<sup>***</sup><br>(.2181983)</td>
            <td>1.301863<sup>***</sup><br>(.3032876)</td>
        </tr>
        <tr>
            <th scope="row">Population</th>
            <td></td>
            <td>1.063447<sup>***</sup><br>(.1446876)</td>
            <td>.9891452<sup>***</sup><br>(.1619487)</td>
            <td>1.158865<sup>***</sup><br>(.225545)</td>
            <td>1.150728<sup>***</sup><br>(.230567)</td>
        </tr>
        <tr>
            <th scope="row">Gini</th>
            <td></td>
            <td></td>
            <td>.0538155<sup>**</sup><br>(.0268751)</td>
            <td>.0981521<sup>***</sup><br>(.0295869)</td>
            <td>.1110501<sup>***</sup><br>(.0363411)</td>
        </tr>
        <tr>
            <th scope="row">Education</th>
            <td></td>
            <td></td>
            <td></td>
            <td>.0470603<br>(.0304477)</td>
            <td>.0407087<br>(.0304477)</td>
        </tr>
        <tr>
            <th scope="row">Doctors’ Density</th>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td>-.000752<br>(.0011276)</td>
        </tr>
        <tr>
            <th scope="row">Intercept</th>
            <td>3.670147<sup>***</sup><br>(.1283489)</td>
            <td>-10.23082<sup>***</sup><br>(1.931404)</td>
            <td>-10.65228<sup>***</sup><br>(1.852999)</td>
            <td>-16.09139<sup>***</sup><br>(4.318988)</td>
            <td>-15.81489<sup>***</sup><br>(4.498292)</td>
        </tr>
        <tr style="solid black">
            <td colspan="6"></td>
        </tr>
        <tr>
            <th scope="row"><span class="math inline"><em>R</em><sup>2</sup></span></th>
            <td>.3922114</td>
            <td>.6461379</td>
            <td>.652798</td>
            <td>.665427</td>
            <td>.6662798</td>
        </tr>
        <tr>
            <th scope="row">Adjusted <span class="math inline"><em>R</em><sup>2</sup></span></th>
            <td>.3785533</td>
            <td>.6340744</td>
            <td>.6368347</td>
            <td>.6459751</td>
            <td>.6427231</td>
        </tr>
        <tr>
            <th scope="row">N</th>
            <td>92</td>
            <td>92</td>
            <td>92</td>
            <td>92</td>
            <td>92</td>
        </tr>
    </tbody>
</table>
</div>

**Table 2: Regression Results. Number of Discharged.** <a name="tab2"></a>

<div class="table-responsive-md">
<table class='table table-hover'>
    <caption>Robust standard errors in parenthesis. <sup>*</sup><i>p</i> < 0:1, <sup>**</sup><i>p</i> < 0:05, <sup>***</sup><i>p</i> < 0:01</caption>
    <thead>
        <tr>
            <th scope='row'></th>
            <th>(1)</th>
            <th>(2)</th>
            <th>(3)</th>
            <th>(4)</th>
            <th>(5)</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th scope='row'>North-East</th>
            <td>1.498502<sup>***</sup><br>(.3883368)</td>
            <td>1.013639<sup>***</sup><br>(.2502798)</td>
            <td>.9433316<sup>***</sup><br>(.2346669)</td>
            <td>.9574594<sup>***</sup><br>(.2418449)</td>
            <td>.954981<sup>***</sup><br>(.2415764)</td>
        </tr>
        <tr>
            <th scope="row">Ile de France</th>
            <td>2.423485<sup>***</sup><br>(.1784774)</td>
            <td>1.100784<sup>***</sup><br>(.159507)</td>
            <td>.7230497<sup>***</sup><br>(.1747128)</td>
            <td>.6993664<sup>***</sup><br>(.2000135)</td>
            <td>.6430911<sup>**</sup><br>(.264656)</td>
        </tr>
        <tr>
            <th scope="row">Population</th>
            <td></td>
            <td>1.112531<sup>***</sup><br>(.1123722)</td>
            <td>.993284<sup>***</sup><br>(.1211013)</td>
            <td>.9752686<sup>***</sup><br>(.1553269)</td>
            <td>.9719336<sup>***</sup><br>(.1580135)</td>
        </tr>
        <tr>
            <th scope="row">Gini</th>
            <td></td>
            <td></td>
            <td>.0902798<sup>***</sup><br>(.0292446)</td>
            <td>.0848994<sup>**</sup><br>(.0330915)</td>
            <td>.0923457<sup>**</sup><br>(.0361311)</td>
        </tr>
        <tr>
            <th scope="row">Education</th>
            <td></td>
            <td></td>
            <td></td>
            <td>-.0055659<br>(.0224333)</td>
            <td>-.0089142<br>(.025325)</td>
        </tr>
        <tr>
            <th scope="row">Doctors’ Density</th>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td>-.0004245<br>(.001146)</td>
        </tr>
        <tr>
            <th scope="row">Intercept</th>
            <td>4.907909<sup>***</sup><br>(.1208542)</td>
            <td>-9.592106<sup>***</sup><br>(1.489271)</td>
            <td>-10.37125<sup>***</sup><br>(1.389197)</td>
            <td>-9.751786<sup>***</sup><br>(3.047651)</td>
            <td>-9.626842<sup>***</sup><br>(3.148192)</td>
        </tr>
        <tr style="solid black">
            <td colspan="6"></td>
        </tr>
        <tr>
            <th scope="row"><span class="math inline"><em>R</em><sup>2</sup></span></th>
            <td>.3571441</td>
            <td>.7118813</td>
            <td>.733274</td>
            <td>.7334894</td>
            <td>.7338071</td>
        </tr>
        <tr>
            <th scope="row">Adjusted <span class="math inline"><em>R</em><sup>2</sup></span></th>
            <td>.3430154</td>
            <td>.7022774</td>
            <td>.7212863</td>
            <td>.7183468</td>
            <td>.715449</td>
        </tr>
        <tr>
            <th scope="row">N</th>
            <td>94</td>
            <td>94</td>
            <td>94</td>
            <td>94</td>
            <td>94</td>
        </tr>
    </tbody>
</table>
</div>

**Table 3: Results of the Analysis of Covariance.** <a name="tab3"></a>

<div class="table-responsive-md">
<table class='table table-hover'>
    <caption>Note: Two of the 94 departments had no deaths on the 20th of April. This results into 2*94-2 observations.<br>Robust standard errors in parenthesis. <sup>*</sup><i>p</i> < 0:1, <sup>**</sup><i>p</i> < 0:05, <sup>***</sup><i>p</i> < 0:01</caption>
    <thead>
        <tr>
            <th scope='row'></th>
            <th>(1)</th>
            <th>(2)</th>
            <th>(3)</th>
            <th>(4)</th>
            <th>(5)</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th scope='row'>North-East</th>
            <td>1.498502<sup>***</sup><br>(.3894372)</td>
            <td>1.013639<sup>***</sup><br>(.2510045)</td>
            <td>.9433315<sup>***</sup><br>(.2353612)</td>
            <td>.9574594<sup>***</sup><br>(.2425761)</td>
            <td>.954981<sup>***</sup><br>(.2423228)</td>
        </tr>
        <tr>
            <th scope='row'>North-East*Dummy</th>
            <td>.2864277<sup>***</sup><br>(.0957056)</td>
            <td>.3485058<sup>***</sup><br>(.0861668)</td>
            <td>.3772743<sup>***</sup><br>(.0952936)</td>
            <td>.2422315<sup>**</sup><br>(.0939364)</td>
            <td>.2416038<sup>**</sup><br>(.0957339)</td>
        </tr>
        <tr>
            <th scope="row">Ile de France</th>
            <td>2.423485<sup>***</sup><br>(.1789831)</td>
            <td>1.100784<sup>***</sup><br>(.1599689)</td>
            <td>.7230497<sup>***</sup><br>(.1752297)</td>
            <td>.6993664<sup>***</sup><br>(.2006182)</td>
            <td>.6430911<sup>**</sup><br>(.2654737)</td>
        </tr>
        <tr>
            <th scope="row">Ile de France*Dummy</th>
            <td>.2347463<sup>**</sup><br>(.0927611)</td>
            <td>.3337892<sup>***</sup><br>(.1135917)</td>
            <td>.4891525<sup>***</sup><br>(.1457478)</td>
            <td>.7035998<sup>***</sup><br>(.1643193)</td>
            <td>.658772<sup>***</sup><br>(.2096761)</td>
        </tr>
        <tr>
            <th scope="row">Population</th>
            <td></td>
            <td>1.112531<sup>***</sup><br>(.1126976)</td>
            <td>.993284<sup>***</sup><br>(.1214596)</td>
            <td>.9752686<sup>***</sup><br>(.1557965)</td>
            <td>.9719336<sup>***</sup><br>(.1585017)</td>
        </tr>
        <tr>
            <th scope="row">Population*Dummy</th>
            <td></td>
            <td>-.0490841<br>(.1035451)</td>
            <td>-.0041388<br>(.1141379)</td>
            <td>.1835962<br>(.1461286)</td>
            <td>.178794<br>(.1472504)</td>
        </tr>
        <tr>
            <th scope="row">Gini</th>
            <td></td>
            <td></td>
            <td>.0902798<sup>***</sup><br>(.0293312)</td>
            <td>.0848994<sup>**</sup><br>(.0331916)</td>
            <td>.0923457<sup>**</sup><br>(.0362427)</td>
        </tr>
        <tr>
            <th scope="row">Gini*Dummy</th>
            <td></td>
            <td></td>
            <td>-.0364643<br>(.0223767)</td>
            <td>.0132527<br>(.0248453)</td>
            <td>.0187044<br>(.0257238)</td>
        </tr>
        <tr>
            <th scope="row">Education</th>
            <td></td>
            <td></td>
            <td></td>
            <td>-.0055659<br>(.0225011)</td>
            <td>-.0089142<br>(.0254033)</td>
        </tr>
        <tr>
            <th scope="row">Education*Dummy</th>
            <td></td>
            <td></td>
            <td></td>
            <td>.0526262<sup>***</sup><br>(.0189861)</td>
            <td>.049623<sup>**</sup><br>(.0210125)</td>
        </tr>
        <tr>
            <th scope="row">Doctors’ Density</th>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td>-.0004245<br>(.0011496)</td>
        </tr>
        <tr>
            <th scope="row">Doctors’ Density*Dummy</th>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td>-.0003275<br>(.0008917)</td>
        </tr>
        <tr>
            <th scope="row">Intercept</th>
            <td>4.907909<sup>***</sup><br>(.1211966)</td>
            <td>-9.592106<sup>***</sup><br>(1.493583)</td>
            <td>-10.37125<sup>***</sup><br>(1.393307)</td>
            <td>-9.751787<sup>***</sup><br>(3.056866)</td>
            <td>-9.626843<sup>***</sup><br>(3.157919)</td>
        </tr>
        <tr>
            <th scope="row">Intercept*Dummy</th>
            <td>-1.237761<sup>***</sup><br>(.0738208)</td>
            <td>-.6387168<br>(1.390247)</td>
            <td>-.2810338<br>(1.372104)</td>
            <td>-6.339603<sup>**</sup><br>(2.82479)</td>
            <td>-6.188046<sup>**</sup><br>(2.888944)</td>
        </tr>
        <tr style="solid black">
            <td colspan="6"></td>
        </tr>
        <tr>
            <th scope="row"><span class="math inline"><em>R</em><sup>2</sup></span></th>
            <td>.4825624</td>
            <td>.7321625</td>
            <td>.7433982</td>
            <td>.749052</td>
            <td>.7495514</td>
        </tr>
        <tr>
            <th scope="row">Adjusted <span class="math inline"><em>R</em><sup>2</sup></span></th>
            <td>.4681891</td>
            <td>.7216296</td>
            <td>.7302765</td>
            <td>.7331875</td>
            <td>.7306222</td>
        </tr>
        <tr>
            <th scope="row">N</th>
            <td>186</td>
            <td>186</td>
            <td>186</td>
            <td>186</td>
            <td>186</td>
        </tr>
    </tbody>
</table>
</div>

[^1]: We do not include Corsica, la Réunion, islands in the Atlantic Ocean, and French Guyana.

[^2]: As will be seen, the pandemic was, and still is very serious in the Eastern France.

[^3]: The following French departments are part of this border: Nord (department number 59), Ardennes (68), Meuse (55), Meurthe-et-Moselle (54) Bas-Rhin (67), Haut-Rhin (68) and Moselle (57). We excluded a certain number or Eastern departments, that border Switzerland (essentially mountains, though Geneva is quite close to France) as well as the Italian and the Spanish borders, for the same reason (the Alps and the Pyrenees), though Italy and Spain were hardly hit by the virus.

[^4]: The other departments are Essone (91), Hauts-de-Seine (92), Val-de-Marne (94), Oise (60), Seine-Saint-Denis (93), Val d’Oise (95), and Yvelines (78).

[^5]: Education levels are census data available for 1999, 2010 and 2015. Data after 2015 are extrapolated. INSEE provides the number of individuals older than 16 who do no longer attend school (‘population non-scolarisée’) in each education group. Basic Education, here, is defined as the share of those with no diploma or with a Diplôme National du Brevet (DNB), which is granted after completion of the first cycle of education, or with a Brevet d’etude professionnelle (BEP) or Certificat d’apritude professionelle (CAP), which are obtained after completing the first two years of a professional high school.

[^6]: We also tried population density and GDP in place of population (all combinations), but population performs best.

[^7]: Note that the number of observations should be equal to \\(2\times 94\\), since there are 94 departments, but two observations on the variable \\(y_{i1}\\) are missing (see above).

[^8]: Auvergne, Côte-d’Armor, Franche-Comté, Loiret, Pays de Loire, Vendée, and other regions. See Direct Coronavirus en France : bilan, nouveaux cas et foyers https://www.topsante.com/medecine/maladies-infectieuses/zoonoses/coronavirus-en-direct-nouveaux-cas-foyers-en-france-634781 [last consulted on May 19, 2020].

### Figures <a name="cap8"></a>

[*Back to Table of Contents*](#tbc)

<a name="fig1"></a>
<div class="text-center">
    <figure class="figure">
        <img src="/assets/images/Articles/covid-19-and-the-role-of-economic-conditions-in-french-regional-departments/figure-1.jpg" class="figure-img img-fluid" alt="Cumulated Number of Deaths by Department">
    </figure>
</div>

<a name="fig2"></a>
<div class="text-center" name="fig2">
    <figure class="figure">
        <img src="/assets/images/Articles/covid-19-and-the-role-of-economic-conditions-in-french-regional-departments/figure-2.jpg" class="figure-img img-fluid" alt="Cumulated Number of Discharged by Department">
    </figure>
</div>
