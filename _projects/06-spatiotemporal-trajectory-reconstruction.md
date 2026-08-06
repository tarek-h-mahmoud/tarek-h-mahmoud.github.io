---
layout: page
title: Spatiotemporal Trajectory Reconstruction
permalink: /projects/spatiotemporal-trajectory-reconstruction/
group: Applied ML & Data Systems
order: 6
context: Billions of spatiotemporal records per day
summary: Designed a scalable trajectory-reconstruction algorithm for billions of spatiotemporal records, reducing computational complexity and achieving a 20× processing improvement over the existing approach.
tech: [Algorithm Design, PySpark, Cloud Pipelines, Python]
---

### Problem

Published methods for spatiotemporal track and trip reconstruction could not keep pace with the required data volume, which made them unusable for time-critical processing.

### My role

Sole designer and implementer of the algorithm, including the benchmark against the published baseline.

### Approach

An unsupervised pipeline turning raw spatiotemporal pings into coherent tracks and trips. An initial compression pass followed by reconstruction heuristics brings the algorithm to linear time in the number of records — the compression stage, rather than the heuristics, is the real source of the speedup. The result runs inside automated cloud pipelines processing two to three billion records per day.

### Outcome

A 20× processing improvement over the published baseline for roughly a 5% accuracy tradeoff. Became a reused production building block for downstream applications, including COVID-19 movement and exposure flagging.

### Technologies

Custom algorithm design, PySpark, cloud data pipelines, Python.
