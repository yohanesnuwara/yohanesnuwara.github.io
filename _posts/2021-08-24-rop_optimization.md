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

<p align="center">
  <img src="https://user-images.githubusercontent.com/51282928/140704897-6645b57a-f797-459b-9619-4c238cfa9e62.png" width="600" />
</p>

Drilling break is an issue in oil field. This occurs when the rate of drilling penetration (ROP) suddenly drops, for example, from 36 meter/hour to 7 meter/hour, which causes financial loss. This may be caused by incorrectly controlling the Rotation Per Minute (RPM) and Weight On Bit (WOB) of the drillbit during drilling activity. When encountering different lithologies, for example sandstone and shale, drilling engineers may not have enough knowledge to keep the ROP. That is why we need to estimate the appropriate RPM and WOB to avoid the ROP from sudden break. We can combine machine learning and optimization to solve this problem. 

In this work, the open-source datasets from Volve oilfield in North Sea was used. To achieve the objective, two different datasets (real-time drilling data and mud log) were integrated. After the data has been pre-processed, the data was trained using Gradient Boosting Machine (GBM) model. Following the training, a prediction space was made by predicting ROP over a range of WOB and RPM values, while keeping rock properties such as porosity and clay content constant. This prediction space will be later on used as the objective function for optimization step. Finally, Particle Swarm Optimization (PSO) was used to optimize the ROP on the prediction space. This was done by finding the values of WOB and RPM that optimize the ROP. 

With this work, I hope more industries to apply data-driven modeling to optimize their activities. This can not only increase the efficiency of the processes, but also avoid undesirable situation that leads to financial costs. 
