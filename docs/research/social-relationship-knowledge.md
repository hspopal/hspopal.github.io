---
layout: default
title: Social Relationship Knowledge
nav_order: 1
parent: Research
---


## FAVEE-HPP - A Social Relationship Model
There has been considerable work in psychology, sociology, biology, and economics to try to understand social relationships. This has led to a variety of theories, in which some features have been used to describe a social relationship knowledge "space". For example, one can think of relationships along certain dimensions like valence. Relationships can be positive, negative, and everything in between. Another perspective could be that relationships are categorical; we have relationships between people in our family, our friends, or at our work. In graduate school, my colleagues and I developed a dimensional model of describing social relationships, in which categories could be embedded within. These dimensions were Formality, Activeness, Valence, Exchange, and Equality (FAVEE), with three large categories of Hostile, Positive, and Private (HPP) that could fit within those dimensions. 

### The Dimensional Representation
To develop the FAVEE social relationship model, we collected data from thousands of participants, using online surveys. First, we created a comprehensive list of social relationships. To do this, we used natural langauge processing (NLP) tools. These methods are the basis that things like ChatGPT were built off of. In our context, we started off with some "seed" social relationship words that we brainstormed (e.g., friend, brother, wife). We feed these words in to [GloVe](https://nlp.stanford.edu/projects/glove/), an unsupervised learning algorithm that would provide us a list of words that highly co-occur with our seed word within a large database of text built from books, Twitter, Wikipedia, and other sources. Through a series of filtering steps, we condensed this list of tens of thousands of words, to 159 social relationship phrases (e.g., siblings, customer - cashier, student - teacher).

Next, we needed features that could be used to rate the relationships. We looked at all the previous literature on social relationships we could find, and made a dictionary of all the features described in each previous source. This led to 30 unique features. In our initial study with participants from the US, we had over 1000 participants rate a subset of the relationships on a subset of the features. This lead to a large dataset with at least 20 ratings per relationship on each feature. The matrix below shows the average data, where we can see how strongly participants thought each feature described each relationship. 


This could be one model of social relationship knowledge. However, this is hard to understand! It is a lot of data, and doesn't provide us with an easy to use model that we can intuitively use to describe social relationships. So, we applied a dimensionality reduction technique called principal component analysis (PCA), to reduce the number of dimensions, while still being able to capture enough of the original data to be a good model. This led us to the five dimensional FAVEE model. Below, we can see how the original features map onto these new dimensions, and how the 159 social relationships are organized in this 5-dimensional space. 

<iframe src="/assets/images/rel_score_plot.html" width="400%" height="700" style="border:1px solid black;">  </iframe>

### The Categorical Representation

Now we have a model that can describe each social relationship as being some part formality, activeness, valence, exchange, and equality. But can we get categories that could group the relationships and describe each group with just one concept. To do this, we used clustering algorithms to group relationships. Hierarchical clustering allowed us to start with all relationships in one group, and continually break things down until we get a good solution. This lead to a solution in which three large categories and six smaller categoroes that can be used to group relationships. What we also see is that these categories can be organized along the five dimensions as well, where for example, Hostile relationships are negative Valence.

<img src="/assets/images/pca_5pc_12_scatter_kmeans.png" alt="drawing" width="400"/><img src="/assets/images/pca_5pc_34_scatter_kmeans.png" alt="drawing" width="400"/>



## The Neural Representation

In our final analysis, we wished to understand how social relationship knowledge is represented in the brain. Specifically, we wanted to test our FAVEE model to see if it is represented in regions of the social brain network, and whether a dimensional or categorical neural representation is stronger. 

During an fMRI task which asked participants to consider which of two scenarios was most appropriate for a given relationship, regions of the "social brain" network were reliably activated. This included the posterior cingulate cortex, medial prefrontal cortex, temporoparietal junction, and a region within the posterior cerebellum.

<img src="/assets/images/relb_map_sm_thr_surf.png" alt="drawing" width="400"/>

A representational similarity analysis was used to explore whether our FAVEE relationship dimensions were represented within these regions that were reliably activated in our task. Formality was found to be significantly represented, where relationships that were more similar in terms of how formal they were, had more similar patterns of activation throughout this network.
<img src="/assets/images/roi_subject-level_violinplot.png" alt="drawing" width="400"/>
