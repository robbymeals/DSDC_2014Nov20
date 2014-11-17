---

1. Lets assume a classification/rank ordering task. All these techniques should work fine with a regression task.
1. This is meant as a practical, introductory guide, for your "data scientist in the trenches". 

# Prediction

---

# Inference

---

# Second Question: What does the structured part of your dataset look like?
- sparse indicator/boolean values?
- dense continuous values

---

# Sparse

---

# Dense

---

# Third Question: what do you know about the unstructured data?
1. Got labels?
    - For all documents?
    - For some authors for some documents?
1. How does it relate to your structured dataset?
    - classifying authors?
    - classifying object of discussion?
    - single "documents" per link vs hierarchical corpus?
1. you do actually think there is some valuable information in there, right?

---

# Last question: Model evaluation? or how do you feel about p-values?
1. "I need them. All of them."
2. "I don't need them."
3. "I hate them."
4. "All of the above."

---

# Prediction-focused Methods
The Kitchen Sink Approach
    - pro: Objective Function? What Objective Function?
    - con: Depending on your role, often it isn't enough to just predict well.
    - con: People are suspicious of the black box.

---

# Inference-focused Methods
Manually generated derivative features 
    - pro: easy to explain/interpret
    - con: potentially the path to madness
Full Generative Model (now with more DAG)
    - pro: you wrote a dissertation without the fuss of getting a PHd
    - con: you probably don't work there anymore, as it is now fifteen years later

---

# I like a nice blend...
1. Feature Learning
    - Some unsupervised or semisupervised work with the text data
2. Using the results as features in my core mode - represented in a way that propagates the uncertainty. 

---

# Things to watch out 
1. so what do these p-values even mean now?
2. 

---

# Other stuff

---
