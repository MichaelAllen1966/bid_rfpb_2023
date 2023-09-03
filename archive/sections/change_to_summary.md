# Application to patient benefit (long)

Application of work to patient benefit: The modelling undertaken so far is planned to be incorporated into the national stroke audit from Spring 2024. This will provide teams with realistic target thrombolysis use for their own patient population, and identify which area of the stroke pathway to focus on (pathway speed, ascertainment of stroke onset time, thrombolysis decision making). Additionally, NHS-Elect, working with NHS-England, the SAMueL team, and the national stroke audit, have a NHS improvement target to “Improve access to thrombolysis such that by the end of 2027/28, 20% of stroke patients will receive thrombolysis treatment”. This collaborative will be working with 6 low-thrombolysing teams in the first instance, before extending work to all emergency stroke teams. As part of the QI work the SAMueL team will be providing modelling on use of thrombolysis, including on variation in decision-making between hospitals. We consider it important that this work should, if at all possible, include strengthened work on causality (the links between changes to pathway and decsion making, through to thrombolysis use, and through to outcome) so that we have greater confidence that changes suggested/made will lead to the expected improvement in thrombolysis use and, most importantly, in better outcomes and not 'just' increased thrombolysis use.

# See returned documents

* Cmoments from Leon
* Alternative version from Leon
* Comments from Martin 

# From Penny

In the penultimate paragraph is a sentence … during this project we will hold stakeholder workshops etc … you have the word ‘understable’ which I think should be ‘understandable’? 

So I have come up with : 

Our work has shown the use of thrombolysis differs between hospitals mainly from the decision making and processes within each hospital, not because of significant differences in patients attending. 

We are going to use multiple methods within analysis to establish for example, if the current observations are directly linked to early thrombolysis reducing the risk of death in mild stroke are coincidental or related to other factors within patients which hasn’t been considered. This would help to confirm cause and effect conclusions from current models. 

With regard to the patient benefit I think it could be beefed up a bit - this will assist in reducing levels of disability through stroke and potentially reduce deaths. 

# Comments from Antonieta

* Emphasise how we will reduce inequity of deliervy (see papers she has sent - - put in STROKE-IMPACT-BID section in Zotero)
* Emphasise route to real world patitent benefit:
  * Identify research questions with real world impact 
    * Incorporation of analysis into SSNAP palnned from Spring 2024
    * NHS-England Thrombolysis in Acute Stroke Collaborative, TASC
 
# Comments from Anna

In respnse to me asking:

1) Is it clear what we wish to do and why? 
2) Is it clear how this might benefit patients, or do we need to strengthen that bit?

All reads clearly to me. Point 1) is fine, and Point 2) is there but I struggled to find the relevant parts again when I went back looking for them. I'd say that the important sentence there is "These are important observations that may be used to advocate for change in clinical practice." which is currently buried in the middle of the long second paragraph. Is it possible to make it more prominent?

I think it's reasonable to let the reader infer that change in clinical practice would lead to a benefit for patients if you're already at the word limit.

Two minor typos:
+ Second paragraph, "Another example is that appears early use" --> "Another example is that it appears early use"
+ Penultimate paragraph, understable --> understandable

# Comments from Amy
Stroke IMPACT
Title - STOKE IMPACT
Spelling - stroke 

Title - "studies. A study using"
Would this normally be "studies: A study using"? Otherwise the title is two sentences

Title methods
If you're not certain on methods used, is there a danger of saying specifics in the title? Or are those terms "clinical trial emulation" and "causal inference studies" broad enough? I supposed latter is, not familiar with the former.

First sentence
Same as comment on the other proposal.

This would include a literature review, but we expect it to include methods such as:
Word "include" twice - could maybe change to "We would perform a literature review"

Stars
Formatting to bullet poitns

clot-bust
clost-bust or clot-busting?

a NIHR-funded
an NIHR-funded?

The methodological development
Maybe being super clear that that is where the new project sentence starts (as otherwise may think its still talking about existing work) - e.g. methodological development "from the proposed project" or something like that. Also, is it possible to dedicate more of that paragraph to what the benefit of the enhanced methodology is? Obviously context super important! But like that second bullet point about pathways as it dedicates more time to explaining what the immediate uses are - whereas the first bullet only has one sentence which is to "identify and isolate causal relationships" - could maybe expand on why that is important to know? Otherwise they might think, you've already done all this work, why do you need to do some new methods. Unless the audience is "causal people", in which case, maybe less so.

Figure
Find it hard to read "health economics" and initial assumption is "its light grey because not doing it" and wasn't until read the description that realised that is because its collaborative.

pubslished
spelling: published.

# Comments from Martin James

Hi Mike
I'm sure it is wise to formulate our research into questions! However we need to avoid drifting into the territory of RCTs. I think question 2 is worth reformulating as the 'observed and expected' benefit and harm. It's fair to say that with the dataset we have we can provide valuable knowledge about what happens in UK clinical practice to the people with any of those three conditions prior to thrombolysis and that might help reassure reluctant thrombolysing sites about the risk of harm. I don't think that information is available from other sources, so it could be influential.
Question 3 is along lines that we have previously discussed, although we will have limited information from the SSNAP dataset as to the relation between onset-to-arrival and outcomes for haemorrhage patients. I wouldn't say that ICH and IS patients are 'easily confused' - it's more a case that severely affected patients with either IS or ICH look identical in pre-hospital selection for redirection, but in doing so it may mean that ICH patients have delayed treatment for blood pressure or stroke unit admission - both interventions that improve outcomes for ICH patients as demonstrated in the recently published INTERACT-3 trial, which would be worth citing as the most recent example of specific hyperacute interventions benefitting ICH patients (however they don't provide information on the relation to time-to-arrival). https://www.thelancet.com/article/S0140-6736(23)00806-1/fulltext 
BW
Martin

# Comments from Joaoa

* J uses Cox models for "time to event" outcomes; a little differetn to our plans
* Consider randonly assigning patients to different units (and predict outcomes) to mimic a trial (MA: similarly could send all patients to all units, or send the sample of patients to all units - maybe pick a 5-10k sample of patients with 20-80% average probability of rceiving thrombolysis, and predict use of thrombolysis and then outcomes with the predict use or no-use of thrombolysis?)
* Consider converting outcome to a binary outcome (e.g ability to return to where they were before, or no more than +1 change)
* Include caveats in the bid. Can never establish 100% causality unless have instrumental variable (tricky to find). But can make a best guess. Talk about association. Hospital SHAP for use of thrombolysis could be usedf as an instrumental variable.
* When comparing outcomes create groups of no-use of IVT and use of IVT that are similar for key patient characteristics (e.g. those determinign use of thrombolysis)  - spread out from propnesity to use thrombolysis = 0.5 until groups become disimialr (MA: prob need to use an avergare or nenchmark propensity for thrombolysis).
* Alternative include all patients but then reduce from both ends of confounders until similar distribution for using and not using thrombolysis
* Look at DAGitty tool 
* Contact: Jack Bowden. Develops methods for establishing causality (https://www.dagitty.net/): online or on R. MA: Does Python DoWhy library do something similar, or shoudl we start to use R a bit?
* Compare multipel tools:
  * Inverse propnsensity score weighting
  * Instrument variable (using hopsital SHAP for thrombolysis)
  * Co-variable adjustment
* Specify that these tools can be used in the hospital context.
  

# Thoughts from Mike

* Mention Judea Pearl's Causal Inference Framework (desbed in The Book of Why) - based heavily on Directed Acycyclic Graphs (DAGs) which provide a very easily interprtable hypothesis for causes and effect relationships

* Methods (for sceintific summary):
  * DAGs
  * Target Trial Emulation
  * Instrument variables
  * Matching
  * Covariate adjustment (response surface modelling) - conditional average treatment effect (CATE)
  * Propensity score reweighting (inverse treatment probability weighting)
  * Propensity score stratification
  * Doubly robust estimates
  * Double ML









