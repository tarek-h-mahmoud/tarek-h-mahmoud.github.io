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

Designer and implementer of the algorithm, including the benchmark against the published baseline.

### Approach

An unsupervised pipeline turning raw spatiotemporal pings into coherent tracks and trips. A compression step collapses runs of consecutive pings from the same location into a single record spanning a start and end time, and reconstruction heuristics then operate over the compressed sequence. The algorithm makes only one pass over the data, which is what brings it to linear time in the number of records. The result runs inside automated cloud pipelines processing two to three billion records per day.

### Outcome

A 20× processing improvement over the published baseline for roughly a 5% accuracy tradeoff. Became a reused production building block for downstream applications.

### Technologies

Custom algorithm design, PySpark, cloud data pipelines, Python.
