# Simplifying assumptions
1. simple generalized linear models, not panel data or time series
2. introductory, practical, short
3. unstructured == text documents, could concievably take similar approach with 
   audio or visual data if you know equivalent preprocessing 
   dsp or image processing, but I haven't done it

# Motivations
1. improve overall predictive power of model
2. imputation: fill in sparse or missing values in your structured dataset
    1. only have gender or visit reason 
       or other categorical value for a subset
    2. have labeled data for observations outside of your dataset
       and equivalent corpora 
3. infer relationships between a variable of interest 
   and some latent random variable or variables you believe 
   are represented in some way, obvious or not, in your unstructured data 
    1. discussions of interactions with staff
    2. operational incidents 
    3. ongoing operational issues

# Some questions
1. what's the expected product of your work? 
    1. pure prediction? 
    2. inference or analysis of relationships? 
    3. a mix of both?
2. what does your structured data look like?
    1. how many observations you got?
    2. sparse, dense? 
    3. missing values?
3. What does your unstructured data look like?
    1. what's the link?
        1. predictions about authors?
        2. about objects of discussion?
        3. 1-to-1 vs 1-to-many (hierarchical)
    2. how much of it you got?
    3. labeled? how? 
    4. you have some reason to believe there is valuable information
      in there somewhere
4. How important are specific model evaluation techniques?
    1. statistical significance
        1. do you need p-values? do you need all the p-values?
    1. How do you feel about precision and recall?

# examples
1. predict receptiveness of potential targets for a promotional campaign
    - use for rank ordering
    - structured data: demographic info, customer activity
    - unstructured data: social media presence/postings
2. predicting operational metrics at different locations of a business
    - use for informing business decisions, changes in operations
    - structured data: operational metrics, geographic/region demographics
    - unstructured data: social reviews and survey responses for location
3. predict merchant upside for participating in a "daily deal" promotion
    - use for rank ordering sales decisions and informing business decisions
    - structured data: operational metrics, geographic/region demographics
    - unstructured data: social reviews and survey responses for location

# techniques
1. Heuristics
    - pro: simple to explain/interpret
    - con: difficult to capture subtlety/nuance in any real way 
2. Full generative model
    - pro: full probability model
    - con: difficult to do well, time consuming
    - con: probably not worth the effort
3. Sub-classifiers, with predictions used as features in core model
4. unsupervised and semi-supervised "summarization", with results used
   as features in core model
    1. clustering 
    2. abstraction 
    3. dimensionality reduction

# preprocessing
1. bag-of-ngrams
2. chunking
3. stopword filtering

# useful tools
1. NLTK (comprehensive python NLP package)
2. scikit-learn (python machine-learning package)
3. gensim (python topic modeling toolkit)
4. tm (R package)

