https://towardsdatascience.com/a-complete-guide-to-causal-inference-8d5aaca68a47

# Notes on stuff to possibly include:

* ML models of variation in suitability for thrombolysis and thrombectomy
* Clinical outcomes models for thrombolysis and thrombectomy trained and tested on multiple matched cohorts
* Exploration of effect of time to treatment in practice for thrombolysis and thrombectomy
* Haemorrhagic stoke outcome based on time to treatment
* Triangulation with clinical trial maths models

* We're in the ARC (good established links with hospitals/relevant clinicians)

* Say what we've done, what is missing, and how we plan to full the gap.


## Letters of support:

* Chris Price stating it's useful for another NIHR grant (OPTIMIST project)
* National clinical director of stroke (Dr Deb Lowe)

## Mike's holiday thoughts

Money is probably limitting for RfPB. Could we make the point that we will apply the RfPB methodology in projects where we can do some follow-up qual work?

Could we approach RfPB informally and ask whether they'd like us to build in qual work, but accepting that will take us to 'teir 1' (up to £500k). 

Based on what you've done so far, could we prepare some patient descriptions and ask people to grade them by mRS. Gary has said he thinks mRS 0-2 are easily confused or classified differently by different people. (In which case we may want to add up SHAPs into a single block for those).

MJA: Does confusion matrix support higher confusion among mRS 0-2? E.g. is is easier to distinguish 3 vs 4 than 1 vs 2?

Add in £5K for data request to finance if not there.

## Asking ChatGPT "Tell me a bout methods for causal machine learning, in a way a 14 year old could understand"

Causal machine learning is a way of understanding why things happen, not just predicting what will happen based on past data. Here are some methods for causal machine learning that a 14-year-old could understand:

    Causal inference: This is a way of understanding the relationship between cause and effect. It involves asking questions like "What would have happened if X had not occurred?" and "What would happen if we changed Y?"
    
    Bayesian networks: This is a framework for causal inference that involves creating a graph showing how events cause each other. It can be used to predict the probability of an event occurring based on other events
    
    Do-calculus: This is a set of rules for manipulating causal models. It can be used to answer questions like "What would happen if we intervened to change X?"
    
    Counterfactual reasoning: This is a way of thinking about what would have happened if things had been different. It involves imagining different scenarios and comparing them to the actual outcome3
   
    Reinforcement learning: This is a method for learning incrementally using interactions with an environment. It can be used to learn causal relationships between actions and outcomes4
  
    Randomized controlled trials: This is a way of testing the effectiveness of a treatment or intervention by randomly assigning participants to different groups. It can be used to establish causal relationships between the treatment and the outcome5
   
Overall, causal machine learning is a way of understanding why things happen and how we can change them. It involves asking questions, creating models, and testing hypotheses to uncover causal relationships between variables.

"Tell me more about Bayesian networks"

Bayesian networks are probabilistic graphical models that represent the dependency structure of a set of variables and their joint distribution efficiently in a factorized way. Here are some more details about Bayesian networks:

    Bayesian networks combine graph theoretic approaches with approaches of probability theory
    
    Each node in a Bayesian network corresponds to a random variable, and the edges between nodes represent the relationship between them
    
    Bayesian networks consist of a directed acyclic graph (DAG), which is a causal graph where nodes represent random variables and edges represent the relationship between them, and a conditional probability distribution (CPD) associated with each of the random variables
    
    The links between variables in Bayesian networks encode dependency but not necessarily causality. However, in some cases, Bayesian networks can be used to represent causal relationships between variables
    
    Bayesian networks can be used to answer questions about the relationships between variables, such as whether two variables are independent or whether one variable causes another
    
    Bayesian networks can be used to visualize the probabilistic model for a domain, review all of the relationships between the random variables, and reason about causal probabilities for scenarios given available evidence
    
    Bayesian networks are a type of probabilistic graphical model that explicitly capture the known conditional dependence with directed edges in a graph
    
    Bayesian networks are useful for dealing with uncertainty and complexity and are playing an increasingly important role in the design and analysis of machine learning algorithms

Overall, Bayesian networks are a powerful tool for representing and reasoning about the relationships between variables in a probabilistic way. They can be used to answer questions, visualize relationships, and reason about causal probabilities.

https://medium.com/towards-data-science/introduction-to-bayesian-networks-81031eeed94e

https://medium.com/towards-data-science/conditional-independence-the-backbone-of-bayesian-networks-85710f1b35b

https://medium.com/towards-data-science/causality-and-bayesian-networks-fcd959d4c80a

https://medium.com/towards-data-science/bbn-bayesian-belief-networks-how-to-build-them-effectively-in-python-6b7f93435bba

https://medium.com/codex/how-to-create-ai-hybrid-models-models-in-python-using-causalnex-a-guide-for-bayesian-networks-6d9387f06556

