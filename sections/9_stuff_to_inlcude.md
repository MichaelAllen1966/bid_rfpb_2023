https://towardsdatascience.com/a-complete-guide-to-causal-inference-8d5aaca68a47

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


