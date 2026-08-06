---
layout: page
title: Synthetic Data for Object Detection
permalink: /projects/synthetic-data-object-detection/
group: Applied ML & Data Systems
order: 8
context: Document understanding with limited labeled data
summary: Developed a synthetic-data pipeline for training YOLO-based document object-detection models with limited labeled data. The approach reduced annotation requirements and was extended to multiple document-understanding tasks.
tech: [YOLO, PyTorch, NVIDIA DGX, Python]
---

### Problem

Detecting specific marks within documents required labeled training data that did not exist, and no off-the-shelf document-understanding model was usable for the task at the time.

### My role

Conceived and built the pipeline end to end: data sourcing, augmentation strategy, model training, and evaluation.

### Approach

A synthetic-data factory composites a randomized number of target objects per image onto real background documents, with heavy per-composite augmentation — discoloration, blur, rotation, flipping, grayscale conversion, scaling, tilting — to simulate scan and photo noise and force generalization. Output feeds directly into YOLO training on distributed GPUs, with fine-tuning against a held-out benchmark of real documents.

### Outcome

The models generalized to real documents despite training almost entirely on synthetic data. The approach substantially reduced annotation requirements and was reused by teammates for other document-understanding tasks.

### Technologies

Synthetic data generation, YOLO, PyTorch, distributed training on NVIDIA DGX, Python.
