---
layout: page
title: Hierarchical Name Classification Service
permalink: /projects/name-classification-service/
group: Applied ML & Data Systems
order: 7
context: Large-scale identity and entity analytics
summary: Built a production classification service trained on more than 30 million weakly labeled samples, achieving 98% accuracy and supporting large-scale identity and entity analytics.
tech: [scikit-learn, Docker, REST API, Python]
---

### Problem

Names had to be classified at scale from noisy, weakly labeled data with severe class imbalance, replacing a process that was until then manual.

### My role

Designed the classification taxonomy and the hierarchical model architecture, then built and deployed the production service.

### Approach

A hierarchical tree of classifiers rather than a single flat model, which handles the severe class imbalance considerably better. Trained on more than 30 million weakly labeled records and deployed as a containerized REST microservice.

### Outcome

98% accuracy in production, with substantial time and cost savings from automating work that had previously been manual.

### Technologies

Hierarchical classification, scikit-learn, weak supervision, Docker, REST APIs, Python.
