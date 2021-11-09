---
title: 'Prediction of P-Sonic Log in the Volve Oil Field using Machine Learning'
date: 2020-10-15
permalink: /posts/2020/10/sonicsynthesis/
tags:
  - Data Pre-processing
  - Gradient Boosting
  - geoscience
---

<img src="https://user-images.githubusercontent.com/51282928/140687832-381c13a0-7a2b-495c-8817-eee5064c11b5.png" align="left" width="30" height="30">[Read this work](https://towardsdatascience.com/prediction-of-p-sonic-log-in-the-volve-oil-field-using-machine-learning-9a4afdb92fe8) in Towards Data Science

In the exploration for petroleum resource, missing well log is an issue. When a geophysical logger acquires well log data from the subsurface, there may be some issues such as formation damage in the borehole that makes it unable to be recorded, or may be problem with the tool. One of the most frequent missing logs are sonic logs. In fact, sonic logs are very crucial for formation evaluation (type of rock classification and hydrocarbon indicator). Therefore, it's better if we can recover the missing data. People very often uses simple linear regression to synthesize sonic log. In this work, I implement ML algorithm to solve this problem. 

In this work, an open-source well log dataset from Volve oil field in the North Sea was used. 3 wells which have complete sonic logs are used for training dataset and 2 wells for blind prediction. The wells have log measurements such as Gamma Ray, Bulk Density, Neutron Porosity, Caliper, Resistivity, and Photoelectric Factor. Before ML, the data was pre-processed using Yeo-Johnson power transform method for normalization and One-class SVM method for removing some data outliers. 

<p align="center">
  <img src="https://user-images.githubusercontent.com/51282928/140873280-14ed2b70-1beb-44e9-9f20-3f02d8960dba.png" width="600" />
</p>

