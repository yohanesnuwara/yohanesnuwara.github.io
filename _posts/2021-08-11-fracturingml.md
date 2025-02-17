---
title: 'Machine Learning for Prediction in Hydraulic Fracturing'
date: 2021-08-11
permalink: /posts/2021/08/fracturingml/
tags:
  - Statistical Test
  - Decision Tree
  - petroleum engineering
---

<img src="https://user-images.githubusercontent.com/51282928/140687832-381c13a0-7a2b-495c-8817-eee5064c11b5.png" align="left" width="30" height="30">[Read this work](https://medium.com/analytics-vidhya/machine-learning-for-prediction-in-hydraulic-fracturing-43de92b0e10a) in Analytics Vidhya

<p align="center">
  <img src="https://user-images.githubusercontent.com/51282928/140769539-7109c40f-70e2-4614-882c-6915191b3672.png" width="400" />
</p>

In unconventional oilfield, fracturing is the only way to extract the oil from the subsurface. Designing fracturing parameter such as number of clusters per stage is critical to contribute to its success. A cluster is a set of perforations shot into the casing and repeated over a number of intervals or spacing. The group of clusters then form the stage that will be stimulated with the proppant. One stage may consist of as little as 1 to more than 15 clusters. Usually, frac engineer develops numerical model to design the fracturing. However, as complexity in the formation rises, a numerical model can be insufficient. Therefore, data-driven modeling can be useful.  

In this work, an open-source dataset from SPE was used. The dataset consists of records from 53 wells consisting of reservoir temperature, pressure, water saturation, gas specific gravity, and perforation geometry. Feature selection using statistical R-test was done to reduce from 25 to only 13 useful features. Next, Decision Tree model was used as regressor. To handle with small dataset, Leave-One-Out Cross-Validation (LOOCV) was used as a strategy to avoid model overfitting. From this LOOCV, two hyperparameters of Decision Tree are determined to achieve the most desirable model. 

The trained model was finally used to predict the number of clusters per stage given a mock case of a fracturing company. Modeling based on data-driven approach which is demonstrated in this work makes the fracturing design more efficient. 

![image](https://user-images.githubusercontent.com/51282928/140768074-1dcf5632-866f-4a15-9e5e-f62d36702c02.png)

