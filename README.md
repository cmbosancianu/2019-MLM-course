# Applied Multilevel Regression Modeling
 This repository contains class materials for a 2019 2-week course in Applied Multilevel Regression Modelling.
 
 Though all materials were developed from the ground up, a great deal of insight was gained from past experiences TAing for similar classes and workshops taught over the years by Zoltan Fazekas ([https://zfazekas.github.io/](https://zfazekas.github.io/)) and Levente Littvay ([https://levente.littvay.hu/](https://levente.littvay.hu/)). I am grateful to both for the opportunity.

 ## Introduction

 "Once you know that hierarchies exist, you see them everywhere." (Kreft & de Leeuw, 1998, p. 1).

 This course introduced participants to a class of statistical specifications that allows for the rigorous analysis of data that exhibit such hierarchical properties: multilevel models. Beyond their desirable statistical properties, though, the primary sell-point of these models is that they allow us to pose, and find supportive evidence for, more complex questions about the world. They do so by treating variation at multiple levels of the nesting structure not as a nuisance but as a substantively interesting feature of the data, to be modeled rather than corrected for. An additional desirable feature of these models is their versatility: wherever data is nested in higher-order groups, it's a good bet that a multilevel can be adapted and applied to such data.

The two weeks were devoted, first, to covering the foundations of multilevel modeling and, second, to exploring extensions of this core framework to alternative data configurations. In the first week we explored common linear specifications: random-intercept and random-slope models. We covered statistical notation for these models, interpretation of coefficients, presenting uncertainty, reporting results from such models, testing and displaying the effect of interactions between group-level and observation-level variables, as well as what sample size considerations should be kept in mind when analyzing such data. In the second week we allocated each day to an extension of the standard hierarchical linear framework. We introduced generalized linear mixed specifications, with an application to a dichotomous response variable. We then covered how to use a multilevel specification to analyze change over time, as well as how to produce sub-national estimates of public opinion based solely on national-level data. Finally, the materials highlighted how multilevel specifications can be applied to data structures that are not hierarchical, as well as to data that has the added complication of spatial correlations. Throughout the sessions we made intensive use of the `lme4` and `nlme` packages for **R**, along with a variety of functions from connected packages that assist in plotting, model comparison, and data reshaping.

## Course schedule

The first week set the foundations. We started from basic hierarchical linear models (HLMs), with only random intercepts, to more complex specifications, that allow us to understand how an effect varies across contexts. As part of this progression we covered estimation, 2- and 3-level configurations, what sample size considerations apply to HLMs, and how to assess models' adequacy. In the second week we explored alterations to this fundamental framework introduced the week prior. We covered the use of dichotomous outcomes, applying a multilevel specification to assess change over time (growth curve modeling), as well as how to analyze non-hierarchical data configurations. The sessions were conducted entirely in **R**.

In the reading lists provided for each session, readings marked with an **M** denote a mandatory text, whereas those marked with an **O** denote an optional one.

### Day 1: Multilevel models: introduction

Lecture topics:
- Where OLS breaks down;
- OLS-based solutions to address nested data;
- MLMs as a solution to these problems.

Lab topics:
- **R** for regression warm-up;
- Diagnosing and addressing heteroskedasticity;
- Introducing practice data for Week 1.

Reading list:
1. [**M**] Kreft, Ita, and Jan De Leeuw. 1998. *Introducing Multilevel Modeling*. London: Sage. Chapter 1.
2. [**M**] Gelman, Andrew, and Jennifer Hill. 2007. *Data Analysis using Regression and Multilevel / Hierarchical Models*. New York: Cambridge University Press. Chapters 1 and 11.
3. [**O**] Snijders, Tom A. B., and Roel J. Bosker. 1999. *Multilevel Analysis: An introduction to basic and advanced multilevel modeling*. London: Sage. Chapters 2 and 3.
4. [**O**] Bickel, Robert. 2007. *Multilevel Analysis for Applied Research: It's Just Regression!* New York: Guilford Press. Chapters 2 and 3.
5. [**O**] Scott, Marc A., Patrick E. Shrout, and Sharon L. Weinberg. "Multilevel Model Notation–Establishing the Commonalities." In Marc A. Scott, Jeffrey S. Simonoff, and Brian D. Marx. *The SAGE Handbook of Multilevel Modeling*. Los Angeles: Sage Publications. Chapter 2 (pp. 21–38).

### Day 2: Random intercepts in MLM & Notation for models

Lecture topics:
- MLM statistical notation.
- Basic setup for a multilevel specification;
- Group-level predictors: estimation and inference.

Lab topics:
- How MLM notation translates to **R** syntax;
- Running first model: random-intercept specification;
- Interpreting output from model;
- Gradually testing more complex specifications.

Reading list:
1. [**M**] Gelman, Andrew, and Jennifer Hill. 2007. *Data Analysis using Regression and Multilevel / Hierarchical Models*. New York: Cambridge University Press. Chapter 12.
2. [**M**] Enders, Craig K., and Davood Tofighi. 2007. "Centering Predictor Variables in Cross-Sectional Multilevel Models: A New Look at an Old Issue." *Psychological Methods* **12**(*2*): 121–138.
3. [**O**] Gill, Jeff, and Andrew J. Womack. 2013. "The Multilevel Model Framework." In Marc A. Scott, Jeffrey S. Simonoff, and Brian D. Marx. *The SAGE Handbook of Multilevel Modeling*. Los Angeles: Sage Publications. Chapter 1 (pp. 3–20).
4. [**O**] Snijders, Tom A. B., and Roel J. Bosker. 1999. *Multilevel Analysis: An introduction to basic and advanced multilevel modeling*. London: Sage. Chapter 4.
5. [**O**] Raudenbush, Stephen W., and Anthony S. Bryk. 2002. *Hierarchical Linear Models: Applications and Data Analysis Methods*. Advanced Quantitative Techniques in the Social Sciences Series. Thousand Oaks, CA: Sage Publications. Chapter 2.
6. [**O**] Steenbergen, Marco R., and Bradford S. Jones. 2002. "Modeling Multilevel Data Structures." *American Journal of Political Science* **46**(*1*): 218–237.

### Day 3: Random slopes & Cross-level interactions

Lecture topics:
- Centering predictors: grand-mean and group-mean.
- Adding group-level predictors for slopes;
- Cross-level interactions: interpretation and plotting.

Lab topics:
- More complex specifications: random slopes;
- Performing centering;
- Cross-level interactions: **R** code and graphical presentation;
- Presenting MLMs in written work.

Reading list:
1. [**M**] Gelman, Andrew, and Jennifer Hill. 2007. *Data Analysis using Regression and Multilevel / Hierarchical Models*. New York: Cambridge University Press. Chapter 13.
2. [**M**] McNeish, Daniel M., and Laura M. Stapleton. 2016. "The Effect of Small Sample Size on Two-Level Model Estimates: A Review and Illustration." *Educational Psychology Review* **28**(*2*): 295–314.
3. [**O**] McNeish, Daniel M. 2017. "Small Sample Methods for Multilevel Modeling: A Colloquial Elucidation of REML and the Kenward-Roger Correction." *Multivariate Behavioral Research* **52**(*5*): 661–670
4. [**O**] Snijders, Tom A. B., and Roel J. Bosker. 1999. *Multilevel Analysis: An introduction to basic and advanced multilevel modeling*. London: Sage. Chapter 5.
5. [**O**] Brambor, Thomas, William Roberts Clark, and Matt Golder. 2005. "Understanding Interaction Models: Improving Empirical Analyses." *Political Analysis* **14**(*1*), 63–82.

### Day 4: Model fit & Diagnostics

Lecture topics:
 - Model fit in MLM specifications;
 - Model comparisons;
 - Assessing model quality: diagnostics.

Lab topics:
- Model diagnostics: examining problems;
- Correcting problems in tested specifications.

Reading list:
1. [**M**] Steele, Russell. 2013. "Model Selection for Multilevel Models." In Marc A. Scott, Jeffrey S. Simonoff, and Brian D. Marx. *The SAGE Handbook of Multilevel Modeling*. Los Angeles: Sage Publications. Chapter 7 (pp. 109–126).
2. [**M**] Raudenbush, Stephen W., and Anthony S. Bryk. 2002. *Hierarchical Linear Models: Applications and Data Analysis Methods*. Advanced Quantitative Techniques in the Social Sciences Series. Thousand Oaks, CA: Sage Publications. Chapter 9.
3. [**O**] Snijders, Tom A. B., and Roel J. Bosker. 1999. *Multilevel Analysis: An introduction to basic and advanced multilevel modeling*. London: Sage. Chapter 9.
4. [**O**] Snijders, Tom A. B., and Johannes Berkhof. 2008. "Diagnostic Checks for Multilevel Models." In J. de Leeuw & E. Meijer (eds.), *Handbook of Multilevel Analysis* (pp. 141–175). Springer New York.

### Day 5: 3-level models & Recap

Lecture topics:
- Sample size considerations in MLM: level-1 and level-2;
- Extending framework to 3-level models
- Centering and sample size in 3-level specifications;
- Recap of core topics from the past 4 days.

Lab topics:
- Testing a 3-level specification;
- Practice session for running 2-level specification with random intercepts, random slopes, and a cross-level interaction.

Reading list:
1. [**M**] Goldstein, Harvey. 2011. *Multilevel Statistical Models*. 4th edition. London: Wiley. Chapter 3 (sections 3.1 and 3.2 only).
2. [**M**] McNeish, Daniel, and Kathryn R. Wentzel. 2017. "Accommodating Small Sample Sizes in Three-Level Models When the Third Level is Incidental." *Multivariate Behavioral Research* **52**(*2*): 200–215.
3. [**M**] Brincks, Ahnalee M., Craig K. Enders, Maria M. Llabre, Rebecca J. Bulotsky-Shearer, Guillermo Prado, and Daniel J. Feaster. 2017. "Centering Predictor Variables in Three-Level Contextual Models." *Multivariate Behavioral Research* **52**(*2*): 149–163.
4. [**O**] Bickel, Robert. 2007. *Multilevel Analysis for Applied Research: It's Just Regression!* New York: Guilford Press. Chapter 9.

### Day 6: Generalized linear mixed models (GLMMs): dichotomous outcomes

Lecture topics:
- Quick review of standard logistic regression;
- GLMMs: the case of dichotomous outcomes;
- Coefficient interpretation;
- Sample size considerations.

Lab topics:
- GLMMs through the `glmer()` function;
- Group-level predictors, cross-level interactions, and presenting marginal effects.

Reading list:
1. [**M**] Gelman, Andrew, and Jennifer Hill. 2007. *Data Analysis using Regression and Multilevel / Hierarchical Models*. New York: Cambridge University Press. Chapter 14.
2. [**M**] Hox, Joop J. 2010. *Multilevel Analysis: Techniques and Applications*. 2nd edition. New York: Routledge. Chapter 6.
3. [**O**] Snijders, Tom A. B., and Roel J. Bosker. 1999. *Multilevel Analysis: An introduction to basic and advanced multilevel modeling*. London: Sage. Chapter 14.
4. [**O**] Bates, Douglas M. 2010. *lme4: Mixed-effects modeling with R*. Chapter 6. Available at: [https://stat.ethz.ch/~maechler/MEMo-pages/lMMwR.pdf](https://stat.ethz.ch/~maechler/MEMo-pages/lMMwR.pdf) (last accessed: January 30, 2023).

### Day 7: Modeling change over time

Lecture topics:
- Growth curve modeling as a specialized application of multilevel models;
- Time-varying and time-invariant predictors;
- Cross-level interactions in growth curve modeling;
- Error covariance structures for growth curve modeling.

Lab topics:
- Graphical displays of change over time;
- Multilevel specifications with the `nlme()` package;
- Introducing time-varying and time-invariant predictors;
- Allowing for curvilinear change.

Reading list:
1. [**M**] Singer, Judith D., and John B. Willett. 2003. *Applied Longitudinal Data Analysis: Modeling Change and Event Occurrence*. New York: Oxford University Press. Chapters 3, 4, 5, and 6.
2. [**O**] Singer, Judith D., and John B. Willett. 2003. *Applied Longitudinal Data Analysis: Modeling Change and Event Occurrence*. New York: Oxford University Press. Chapter 7.
3. [**O**] Hox, Joop J. 2010. *Multilevel Analysis: Techniques and Applications*. 2nd edition. New York: Routledge. Chapter 5.
4. [**O**] Goldstein, Harvey. 2011. *Multilevel Statistical Models*. 4th edition. London: Wiley. Chapter 5.
5. [**O**] Laird, Nan M., and Garrett M. Fitzmaurice. 2013. "Longitudinal Data Modeling." In Marc A. Scott, Jeffrey S. Simonoff, and Brian D. Marx. *The SAGE Handbook of Multilevel Modeling*. Los Angeles: Sage Publications. Chapter 9 (pp. 141–160).
6. [**O**] Núñez-Antón, Vicente, and Dale L. Zimmerman. "Complexities in Error Structures Within Individuals." In Marc A. Scott, Jeffrey S. Simonoff, and Brian D. Marx. *The SAGE Handbook of Multilevel Modeling*. Los Angeles: Sage Publications. Chapter 10 (pp. 161–182).

### Day 8: Cross-classified & Multiple membership models

Lecture topics:
- Data structures with no clear hierarchy;
- Complex error structures;
- Simultaneous membership in hierarchies;
- Extensions to modeling age-period-cohort (APC) effects.

Lab topics:
- Example of cross-classified structure;
- Modeling strategy in **R**.

Reading list:
1. [**M**] Fielding, Antony, and Harvey Goldstein. 2006. *Cross-classified and Multiple Membership Structures in Multilevel Models: An Introduction and Review*. Department for Education and Skills, UK Home Office: London. Research Report 791. Available at: [https://dera.ioe.ac.uk/6469/1/RR791.pdf](https://dera.ioe.ac.uk/6469/1/RR791.pdf) (last accessed: January 30, 2023).
2. [**M**] Snijders, Tom A. B., and Roel J. Bosker. 1999. *Multilevel Analysis: An introduction to basic and advanced multilevel modeling*. London: Sage. Chapter 11.
Optional:
3. [**O**] Goldstein, Harvey. 2011. *Multilevel Statistical Models*. 4th edition. London: Wiley. Chapters 12 and 13.
4. [**O**] Yang, Yang, and Kenneth C. Land. 2008. "Age–Period–Cohort Analysis of Repeated Cross-Section Surveys: Fixed or Random Effects?" *Sociological Methods & Research* **36**(*3*): 297–326.
5. [**O**] Hox, Joop J. 2010. *Multilevel Analysis: Techniques and Applications*. 2nd edition. New York: Routledge. Chapter 9.

### Day 9: Multilevel regression with post-stratification (MRP)

Lecture topics:
- Problem: studying sub-national attitudes with nationally-representative data;
- Cross-classification as a strategy of obtaining estimates;
- Practical example.

Lab topics:
- Working through example of MRP.

Reading list:
1. [**M**] Ghitza, Yair., and Andrew Gelman. 2013. "Deep Interactions with MRP: Election Turnout and Voting Patterns Among Small Electoral Subgroups." *American Journal of Political Science* **57**(*3*): 762–776.
2. [**M**] Lax, Jeffrey R., Justin H. Phillips. 2009. "Gay Rights in the States: Public Opinion and Policy Responsiveness." *American Political Science Review* **103**(*3*): 367–386.
3. [**O**] Lax, Jeffrey R., and Justin H. Phillips. 2009. "How Should We Estimate Public Opinion in The States?" *American Journal of Political Science* **53**(*1*): 107–121.
4. [**O**] Leemann, Lucas, and Fabio Wasserfallen. 2017. "Extending the Use and Prediction Precision of Subnational Public Opinion Estimation." *American Journal of Political Science* **61**(*4*): 1003–1022.


### Day 10: Multilevel spatial modeling

Lecture topics:
- Adapting MLM specifications to deal with spatial correlations;
- The `W` matrix;
- Estimation and interpretation of effects.

Lab topics:
- Working through one example of spatial analysis.

Reading list:
1. [**M**] Dong, Guanpeng, Jing Ma, Richard Harris, and Gwilym Pryce. 2016. "Spatial Random Slope Multilevel Modeling Using Multivariate Conditional Autoregressive Models: A Case Study of Subjective Travel Satisfaction in Beijing." *Annals of the American Association of Geographers* **106**(*1*): 19–35.
2. [**M**] Corrado, Luisa, and Bernard Fingleton. 2011. "Multilevel Modeling with Spatial Effects." Scottish Institute for Research in Economics: Edinburgh. Available at: [https://strathprints.strath.ac.uk/67923/1/Corrado_Fingleton_DPIE_2011_multilevel_modelling_with_spatial_effects.pdf](https://strathprints.strath.ac.uk/67923/1/Corrado_Fingleton_DPIE_2011_multilevel_modelling_with_spatial_effects.pdf) (last accessed: January 30, 2023).
3. [**O**] Harris, Richard, John Moffat, and Victoria Kravtsova. 2011. "In Search of `W`." *Spatial Economic Analysis* **6**(*3*): 249–270.
4. [**O**] Gelfand, Alan E., Sudipto Banerjee, C. F. Sirmans, Yong Tu, and Seow Eng Ong. 2007. "Multilevel modeling using spatial processes: Application to the Singapore housing market." *Computational Statistics & Data Analysis* **51**(*7*): 3567–3579.


## Later modifications

To update the code, changes to the materials were made over the course of 2022. These included (1) converting `R` scripts to the `Quarto` format, and (2) creating **Python** companion code.
