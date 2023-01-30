# Applied Multilevel Regression Modeling
 This repository contains class materials for a 2019 2-week course in Applied Multilevel Regression Modelling. Though all materials were developed from the ground up, a great deal of insight was gained from past experiences TAing for similar classes and workshops taught by Zoltan Fazekas ([https://zfazekas.github.io/](https://zfazekas.github.io/)) and Levente Littvay ([https://levente.littvay.hu/](https://levente.littvay.hu/)). I am grateful to both for the opportunity.

 ## Introduction

 "Once you know that hierarchies exist, you see them everywhere." (Kreft & de Leeuw, 1998, p. 1).

 This course introduced participants to a class of statistical specifications that allows for the rigorous analysis of data that exhibit such hierarchical properties: multilevel models. Beyond their desirable statistical properties, though, the primary sell-point of these models is that they allow us to pose, and find supportive evidence for, more complex questions about the world. They do so by treating variation at multiple levels of the nesting structure not as a nuisance but as a substantively interesting feature of the data, to be modeled rather than corrected for. An additional desirable feature of these models is their versatility: wherever data is nested in higher-order groups, it's a good bet that a multilevel can be adapted and applied to such data.

The two weeks were devoted, first, to covering the foundations of multilevel modeling and, second, to exploring extensions of this core framework to alternative data configurations. In the first week we explored common linear specifications: random-intercept and random-slope models. We covered statistical notation for these models, interpretation of coefficients, presenting uncertainty, reporting results from such models, testing and displaying the effect of interactions between group-level and observation-level variables, as well as what sample size considerations should be kept in mind when analyzing such data. In the second week we allocated each day to an extension of the standard hierarchical linear framework. We introduced generalized linear mixed specifications, with an application to a dichotomous response variable. We then covered how to use a multilevel specification to analyze change over time, as well as how to produce sub-national estimates of public opinion based solely on national-level data. Finally, the materials highlighted how multilevel specifications can be applied to data structures that are not hierarchical, as well as to data that has the added complication of spatial correlations. Throughout the sessions we made intensive use of the **lme4** and **nlme** packages for *R*, along with a variety of functions from connected packages that assist in plotting, model comparison, and data reshaping. Companion code using the **MixedModels** package for *Julia* was also developed, and added to this repository.

## Course schedule

### Day 1: Multilevel models: introduction

Lecture topics:
- Where OLS breaks down;
- OLS-based solutions to address nested data;
- MLMs as a solution to these problems;

Lab topics:
- *R* for regression warm-up;
- Diagnosing and addressing heteroskedasticity;
- Introducing practice data for Week 1.
