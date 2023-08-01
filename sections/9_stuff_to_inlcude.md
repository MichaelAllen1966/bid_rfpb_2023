https://towardsdatascience.com/a-complete-guide-to-causal-inference-8d5aaca68a47

https://shap.readthedocs.io/en/latest/example_notebooks/overviews/Be%20careful%20when%20interpreting%20predictive%20models%20in%20search%20of%20causal%C2%A0insights.html

"Unless features in a model are the result of experimental variation, applying SHAP to predictive models without considering confounding is generally not an appropriate tool to measure causal impacts used to inform policy. SHAP and other interpretability tools can be useful for causal inference, and SHAP is integrated into many causal inference packages, but those use cases are explicitly causal in nature. To that end, using the same data we would collect for prediction problems and using causal inference methods like double ML that are particularly designed to return causal effects is often a good approach for informing policy. "


Double machine learning: https://towardsdatascience.com/double-machine-learning-for-causal-inference-78e0c6111f9d

# Notes on stuff to possibly include:

* ML models of variation in suitability for thrombolysis and thrombectomy
* Clinical outcomes models for thrombolysis and thrombectomy trained and tested on multiple matched cohorts
* Exploration of effect of time to treatment in practice for thrombolysis and thrombectomy
* Haemorrhagic stoke outcome based on time to treatment
* Triangulation with clinical trial maths models

* We're in the ARC (good established links with hospitals/relevant clinicians)

* Say what we've done, what is missing, and how we plan to full the gap.

## Packages

https://pypi.org/project/psmpy/


## Letters of support:

* Chris Price stating it's useful for another NIHR grant (OPTIMIST project)
* National clinical director of stroke (Dr Deb Lowe)

## Mike's holiday thoughts

Money is probably limitting for RfPB. Could we make the point that we will apply the RfPB methodology in projects where we can do some follow-up qual work?

Could we approach RfPB informally and ask whether they'd like us to build in qual work, but accepting that will take us to 'teir 1' (up to £500k). 

Based on what you've done so far, could we prepare some patient descriptions and ask people to grade them by mRS. Gary has said he thinks mRS 0-2 are easily confused or classified differently by different people. (In which case we may want to add up SHAPs into a single block for those).

MJA: Does confusion matrix support higher confusion among mRS 0-2? E.g. is is easier to distinguish 3 vs 4 than 1 vs 2?

Add in £5K for data request to finance if not there.

Use a Pearlian model for causation.

## Cusal inference with DoWhy library:

https://github.com/py-why/dowhy
https://youtu.be/Ts0hnNBRIWg?si=u4seW0loTShtKQFn

Documentation: https://www.pywhy.org/dowhy/v0.9.1/
Tutorial: https://causalinference.gitlab.io/kdd-tutorial/
Video: https://www.microsoft.com/en-us/research/video/foundations-of-causal-inference-and-its-impacts-on-machine-learning/
Repo: https://github.com/amit-sharma/causal-inference-tutorial/

## Stuff 

* People interpret results as causal even if the C-word is not used




More methods:

* Workshops to draw DAGs
 
Covariate adjustment (response surface modelling) - conditional average treatment effect (CATE)
Propensity score reweighting (inverse treatment probability weighting)
Propensity score stratification
Doubly robust estimates
Double ML
Matching




Drawing a DAG (from https://youtu.be/Ts0hnNBRIWg?si=u4seW0loTShtKQFn):
* Develop and state a clear research question?:
  * What is yoiur focal relationship?
    * What is your exposure?
    * What is your outcome?
    * What is your estimand?  
* Condsider and state your context
* Draw your DAG(s) as early as possible
* Get help - don't draw it alone
* Include all relevant variables (what total infoirmation would you have in an ideal world - show latent varaible that could be important but you don't have)
* Draw your DAG(s) in tempral order
* Draw forwards arcs, unless confident otherwise (assume links could be causal, unless sure otherwise) - then prune back. e.g could differences in stroke severity cause a change in arrival-to-scan time; if uncertain draw an arc
* Check your DAG9s) against your data
* Use your DAG(s) to inform and interpret your model - clearly state the causal model in your analysis and discussion
* Share and publish your DAG

## Notes

Confounder = common cause, or background variable, that is a variable that influences both the independent variable and dependent variable, causing a spurious association. The influence my be direct or indirect. Confounders are removed by conditioning on the confounder, or including the confounder in a model (to isolate its effect).

A collider is a variable in statistics and causal graphs that is causally influenced by two or more variables. If we condition on the collider (e.g. pick a fixed value/range), then we can see a spurious association between the two causal variables.

"We should condition on any factor that is causilty relevant to the effect" Nancy Cartwright 1983. But - causal diagrams give a better/fuller answer.


Showing causality with the do operator

X causes Y if P(Y/*do*(X)) > P(Y)

This is different to observational conditioning: P(Y|X) > P(Y)

## Quotes

"Probabilities encode our beliefs about a static world; causality tells us whether and how probabilties change when the world changes, be it by intervention or by an act of imagination" The Book Of Why

"Causal inference is a core task of science. However, authors and editors often refrain from explicitly acknowledging the causal goal of research projects; they refer to causal effect estimates as associational estimates. This commentary argues that using the term “causal” is necessary to improve the quality of observational research. Specifically, being explicit about the causal objective of a study reduces ambiguity in the scientific question, errors in the data analysis, and excesses in the interpretation of the results." Hernan, from The C-Word: Scientific Euphemisms Do Not Improve Causal Inference From Observational Data




