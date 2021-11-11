---
title: 'Drilling Data Dashboard'
date: 2020-12-12
permalink: /posts/2020/12/drilling_dashboard/
tags:
  - Visualization
  - Dashboard
  - petroleum engineering
---

![realtime-drilling-dashboard](https://user-images.githubusercontent.com/51282928/141255359-8a55898e-1b0d-4d4a-bb26-44f12cd14dd6.gif)

[Open project notebook](https://nbviewer.org/github/yohanesnuwara/geostatistics/blob/main/project_notebooks/integrated_dashboarding_project.ipynb)

Building a dashboard is a smart move for data visualization to show insights from data for the asset management team. A good dashboard should consist of many statistical visualization elements. Drilling data is one of crucial data in the petroleum industry, which is acquired in real-time. 

In this project, I built a data dashboard using Plotly (programmed in Python). The visual elements I developed in this dashboard are 3D plot of wellbore trajectory, box plot, Kernel Density Estimated (KDE) distribution plot, and timeseries panel. What is unique in this dashboard is that the box plot and KDE plot is decomposed into time intervals. This will allow the users to see how the data changes with time. This is something that (I believe) Tableau or Power BI lacks. 

It was expected that using with dashboard, any data scientists could use this tool for predictive modeling e.g. predicting future rate of penetration (ROP) from historical records or identifying drilling anomalies.  
