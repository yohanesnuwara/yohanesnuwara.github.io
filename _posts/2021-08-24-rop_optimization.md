---
title: 'Faster Drilling with Machine Learning and Particle Swarm Optimization'
date: 2021-08-24
permalink: /posts/2021/08/rop_optimization/
tags:
  - Gradient Boosting
  - Particle Swarm Optimization
  - petroleum engineering
---

<img src="https://user-images.githubusercontent.com/51282928/140687832-381c13a0-7a2b-495c-8817-eee5064c11b5.png" align="left" width="30" height="30">[Read this work](https://towardsdatascience.com/faster-drilling-with-machine-learning-and-particle-swarm-optimization-335bb28d687) in Towards Data Science

Drilling break is an issue in oil field. This occurs when the rate of drilling penetration (ROP) suddenly drops, for example, from 36 meter/hour to 7 meter/hour, which causes financial loss. This may be caused by incorrectly controlling the Rotation Per Minute (RPM) and Weight On Bit (WOB) of the drillbit during drilling activity. When encountering different lithologies, for example sandstone and shale, drilling engineers may not have enough knowledge to keep the ROP. That is why we need to estimate the appropriate RPM and WOB to avoid the ROP from sudden break. We can combine machine learning and optimization to solve this problem. 

In this work, the open-source datasets from Volve oilfield in North Sea was used. To achieve the objective, two different datasets (real-time drilling data and mud log) were integrated. After the data has been pre-processed, the data was trained using Gradient Boosting Machine (GBM) model. Following the training, a prediction space was made by predicting ROP over a range of WOB and RPM values, while keeping rock properties such as porosity and clay content constant. This prediction space will be later on used as the objective function for optimization step. 

Finally, Particle Swarm Optimization (PSO) ...
