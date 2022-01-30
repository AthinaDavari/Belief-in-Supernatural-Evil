---
jupyter:
  kernelspec:
    display_name: Python 3
    language: python
    name: python3
  language_info:
    codemirror_mode:
      name: ipython
      version: 3
    file_extension: .py
    mimetype: text/x-python
    name: python
    nbconvert_exporter: python
    pygments_lexer: ipython3
    version: 3.9.1
  nbformat: 4
  nbformat_minor: 2
---

::: {.cell .markdown}
# Belief in Supernatural Evil and Guns

In this assignment you will replicate a study of belief in supernatural
evil and attitudes towards guns in the United States. The study is:

Christopher G. Ellison, Benjamin Dowd-Arrow, Amy M. Burdette, Pablo E.
Gonzalez, Margaret S. Kelley, Paul Froese, \"Peace through superior
firepower: Belief in supernatural evil and attitudes toward gun policy
in the United States\", Social Science Research, Volume 99, 2021,
<https://doi.org/10.1016/j.ssresearch.2021.102595>.

Read the paper, locate, download, and familiarize yourself with the
dataset.

------------------------------------------------------------------------

> Panos Louridas, Associate Professor `<br />`{=html} Department of
> Management Science and Technology `<br />`{=html} Athens University of
> Economics and Business `<br />`{=html} <louridas@aueb.gr>
:::

::: {.cell .markdown}
## Questions

### Q1: Belief in Supernatural Evil Metric

In order to measure the belief in supernatural evil, we will use the
answers to three questions asked by the participants in the survey:

-   Whether the respondent believes in the devil.

-   Whether the respondent believes in hell.

-   Whether the respondent believes in demons.

You will investigate how the answers to these three questions can be
combined to a single metric. Justify your approach.
:::

::: {.cell .markdown}
### Q2: Variables Selection

Apart from the belief in supernatural evil metric, you will use several
other variables to control your estimates. The variables are (see
Appendix B of the original publication):

-   Dependent Variables

    -   Ban on Semi-Auto Guns
    -   Ban on High-Capacity Ammo Clips
    -   Banning Civilian Handguns
    -   Support for Concealed Carry Laws
    -   More Armed Security at Schools
    -   More Teachers/Faculty having Guns
    -   More Gun Safety Programs
    -   Expanded Mental Health Screening

-   Independept Variables

    -   Religious Variables
        -   Attendance
        -   Bible (Human Error, History and Fables)
        -   Biblical Inerrancy
        -   Biblical Literalism
    -   Religious Affiliation
        -   Conservative Protestant
        -   Mainline Protestant
        -   Black Protestant
        -   Catholic
        -   Other
        -   No Affiliation
    -   Political Ideology
    -   Age
    -   Sex
        -   Female
        -   Male
    -   Race
        -   White
        -   Hispanic
        -   African American/Black
        -   Other
    -   Education
        -   Less Than High School
        -   High School or Equivalent
        -   Some College
        -   College Degree
        -   Post-graduate Degree
    -   Household Income
    -   Marital Status
        -   Not Partnered/Single
        -   Married/Cohabitating
    -   Children
        -   No kids under 18 in home
        -   Kids under 18 in home
    -   Area Demographics
        -   Small Town/Rural
        -   Urban Area
    -   Region
        -   South
        -   Other Region

Derive descriptive statistics of your variables and encode them with
dummy variables where needed.

Be *very careful* in your dummy variables encoding. In the end, you
should use the variables as shown in Table 1 and Table 2 of the original
publication.
:::

::: {.cell .markdown}
### Q3: Predict Support for Various Gun Policies

You will then proceed to predict support for various gun policies from
the metric of supernatural evil, controlling for background variables.

The gun policies are:

-   Semi-Auto Weapons Ban

-   High-Capacity Magazine Ban

-   Cilivian Hand Gun Possession Ban

-   Support for Concealed Carry

-   More Armed Security at Schools

-   More Teachers / Faculty with Guns

-   Required Gun Safety Programs

-   Expanded Mental Health Screening

Discuss the effects and the strengths of the various predictors (metric
of supernatural evil, which is our focal variable, plus any others that
you see significant). You should cross-check with Table 1 and Table 2 of
the original publication.

The research was reported in *The Economist*, on November 6, 2021, under
the title \"Belief in supernatural evil is a strong predictor of pro-gun
beliefs\" (United States section), available at
<https://www.economist.com/united-states/2021/11/06/belief-in-supernatural-evil-is-a-strong-predictor-of-pro-gun-beliefs>
(you may access it after a free registration).

Do you agree with the reporting of the research on the newspaper?
:::

::: {.cell .markdown}
### Q4: Additional Estimations of the Strength of Predictors

In addition to logistic regression, you will run a complementary series
of linear regressions to estimate the strength of the various
predictors. In this way you will obtain [standardized
coefficients](https://en.wikipedia.org/wiki/Standardized_coefficient)
that are easier to interpret than the coefficients of logistic
regression. For more on this approach, see:

Von Hippel, Paul, 2015. "Linear vs. Logistic models: which is better,
and when?" Statistical horizons. July 5. Retrieved on December 3, 2021.
<https://statisticalhorizons.com/linear-vs-logistic>.
:::

::: {.cell .markdown}
### Q5: Compare with Decision Trees / Random Forest Estimators {#q5-compare-with-decision-trees--random-forest-estimators}

Having worked with logistic and linear regression models, carry out
predictions by using Decision Trees / Random Forests of your choice; you
may have to try different ones and pick up the best. Then, check if the
predictors, primarily the belief in supernatural evil, make also a
strong showing with the best model you have found.
:::

::: {.cell .markdown}
## Submission Instructions

You will submit a Jupyter notebook that will contain all your code and
analysis. Ensure that the notebook will run correctly in a computer that
is not your own. That means, among other things, that it does not
contain absolute paths. Remember that a notebook is not a collection of
code cells thrown together; it should contain as much text as necessary
for a person to understand what you are doing.
:::

::: {.cell .markdown}
## Honor Code

You understand that this is an individual assignment, and as such you
must carry it out alone. You may seek help on the Internet, by Googling
or searching in StackOverflow for general questions pertaining to the
use of Python, libraries, and idioms. However, it is not right to ask
direct questions that relate to the assignment and where people will
actually solve your problem by answering them. You may discuss with your
fellow students in order to better understand the questions, if they are
not clear enough, but you should not ask them to share their answers
with you, or to help you by giving specific advice.
:::
