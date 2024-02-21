---
layout: default
title: Research
nav_order: 2
---

# Social Relationship Knowledge

When we interact with other people, we make inferences about them, and act accordingly based in part on our social relationship to them. Key older work on social relationships in social psychology and sociology explored the semantic space of social relational concepts and hypothesized that these concepts are represented dimensionally and categoricall. However, these studies failed to reach agreement on the organizing dimensions of human relationships and no attempt was made to understand the neural foundations. The goal of this study was to understand the representational architecture of social relationship knowledge. We hypothesized that our concepts of social relationships are organized along multi-dimensional components, with categories embedded in the dimensional space.

## The Dimensional Representation
We conducted a survey on Amazon Mechanical Turk in which participants were asked to rate 159 social relationships on 30 dimensions derived from theories from the literature on social relationships. Next, we conducted Principal Component Analysis to find the overarching components that could account for the variance in social relationships. We found that five components – formality, activeness, valence, exchange, and equality - accounted for most of the variance in the dimensional ratings of social relationships. 

<img src="/assets/images/srk_behavioral_summary.png" alt="drawing" width="600"/>


## The Categorical Representation

Within the dimensional space we discovered above, we also explored categorical representations that may be embedded within this space. we use a variety of clustering techinques (k-means, hierarchical, UMAP, t-SNE) and data from our 5-component space, and two behavioral surveys to explore categorical representations. Across these data sources and clustering techinques, we found that the most consistent clusters are the fix that are shown below. This clustering is from a k-means clustering of our FAVEE model. It shows that categories of positive, negative, distant, occupational, and transactional relationships can be used to described social relationships. 

<img src="/assets/images/pca_5pc_12_scatter_kmeans.png" alt="drawing" width="400"/><img src="/assets/images/pca_5pc_34_scatter_kmeans.png" alt="drawing" width="400"/>

## The Neural Representation

In our final analysis, we wished to understand how social relationship knowledge is represented in the brain. Specifically, we wanted to test our FAVEE model to see if it is represented in regions of the social brain network, and whether a dimensional or categorical neural representation is stronger. 

During an fMRI task which asked participants to consider which of two scenarios was most appropriate for a given relationship, regions of the "social brain" network were reliably activated. This included the posterior cingulate cortex, medial prefrontal cortex, temporoparietal junction, and a region within the posterior cerebellum.

<img src="/assets/images/relb_map_sm_thr_surf.png" alt="drawing" width="400"/>

A representational similarity analysis was used to explore whether our FAVEE relationship dimensions were represented within these regions that were reliably activated in our task. Formality was found to be significantly represented, where relationships that were more similar in terms of how formal they were, had more similar patterns of activation throughout this network.
<img src="/assets/images/roi_subject-level_violinplot.png" alt="drawing" width="400"/>

# Social Cognition and the Cerebellum

The cerebellum has long been thought to solely process motor information. Yet, there is a growing literature that points to a role of the cerebellum in processes across multiple domains. Individuals with cerebellar lesions classically have motor deficits but, in some instances, also have problems with executive functioning, emotion processing, language, and social cognition. Multiple psychiatric disorders, including autism spectrum disorders (ASD), have been linked to structural and functional differences in the cerebellum. Moreover, numerous functional magnetic resonance imaging (fMRI) studies have reported neural responses in the cerebellum related to a host of non-motor tasks. These findings provide evidence that the cerebellum is involved in non-motor tasks, but it remains entirely unclear how the cerebellum contributes to performance on these tasks. 

Models have been successfully developed to explain the role of the cerebellum in motor processing. These models emphasize the cerebellum’s role as a learning machine that modulates and perfects ongoing processing through the online comparison of reality to an internal model, thereby utilizing sensory prediction errors. Recent findings in humans and mice suggest that portions of the cerebellum are involved in reward processing; a process which has primarily been investigated in regards to the basal ganglia. It is unclear what computational role the cerebellum plays in this reward processing, as the cerebellum has been said to explicitly operate without reward information. To understand this, my dissertation will use fMRI in healthy young adults to study the cerebellum’s contribution to both traditional (e.g. monetary) and social reward processing, and to differentiate it from the role of the basal ganglia in reward processing. 

Individuals with ASD exhibit deficits in social cognition and in social reward processing. Structural, functional, and connectivity differences have implicated the cerebellum in this disorder, with neonatal cerebellar damage being the second highest predictor of ASD. In my post-doc I hope to investigate how the cerebellum performs in individuals with autism, who have deficits in social reward processing. The training plan in this phase of the proposal will focus on learning computational modeling of reinforcement learning and applying these models to cerebellum functioning with fMRI.
