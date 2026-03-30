# INM705-Deep-Learning-for-image-analysis
Here you go — clean and professional for a README.

---

## Dataset

MOT17 (Multiple Object Tracking 2017) is a standardised benchmark dataset widely used in pedestrian detection and multi-object tracking research. It consists of 7 video sequences captured across diverse real-world scenarios — including static and moving cameras, varying crowd densities, and different lighting conditions. The dataset provides approximately 11,000 annotated frames with over 1,638 unique pedestrian identities, each assigned persistent IDs across frames along with precise bounding box annotations. MOT17 is the de facto benchmark for evaluating multi-object tracking systems, making results directly comparable to published state-of-the-art methods.
Since the dataset is small, the idea is to combine or augment it with the crowdHuman dataset. 
---

## Motivation

In crowded real-world scenes, tracking individual people across video frames remains a fundamentally difficult problem. Pedestrians frequently occlude one another, move unpredictably, and can temporarily disappear from view — causing tracking systems to lose or confuse identities. Standard object detectors treat all spatial features equally, making no distinction between person-relevant regions and cluttered background, which degrades both detection quality and downstream re-identification.

---

## Problem Statement

This project investigates whether incorporating an attention mechanism into a pedestrian detection and re-identification pipeline can improve tracking consistency in crowded scenes. Specifically, a CBAM attention block is injected into the feature pyramid of a Faster R-CNN detector to selectively emphasise spatially and semantically relevant features. The impact of this contribution is measured through a controlled ablation study comparing detection accuracy and multi-object tracking metrics — MOTA, IDF1, and HOTA — with and without the attention module, evaluated on the MOT17 benchmark.

---
