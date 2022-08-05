---
title: "Augmenting Information Technology for Precision Forestry Automation"
excerpt: "Closed loop"
collection: portfolio
---

<p align="center">
<img src="https://user-images.githubusercontent.com/51282928/183049871-0b0e974c-818e-4377-ab3c-9cd88e4cab5d.png" alt="drawing" width="700"/>
</p>

Nowadays, the use of Information Technology (IT) is inevitably crucial to deliver value to our planet. Since 2018, we agreed not to use wood from natural forests instead we use wood from our own harvested forest. We had planted more than 100,000 hectares of *Eucalyptus pellita* at every 3-4 years of rotation. During this period, we need to do inventory of trees as well as monitoring of tree growth and yield. To speed up the traditional process of inventory, we developed a computer vision-backed service to automate precision forestry. 

<p align="center">
<img src="https://user-images.githubusercontent.com/51282928/183049436-ffabbec8-376b-485d-bfbe-9b88ebf9f53c.png" alt="drawing" width="700"/>
</p>

## Relational Database Management System (RDBMS)

This is where inputs and outputs are stored. All metadata about each individual plantation area, called as *Petak*, are stored in the database. Examples of input metadata are captured date of UAV acquisition, stratum (plant species and age), province or district locations, area, land type, and many more. While each computer vision use case runs, it retrieves these input metadata from database. After it is completed, output is stored to database also as metadata. Some examples of output metadata are number of tree count, tree stocking percentage, weed percentage, and blankspot percentage. The database also serves as a geodatabase where the outputs such as geolocated tree coordinates and grid polygons are stored. The database also provides metadata to the mobile apps in a form of geolocated display of *Petak* and information related to alerts.

There are 5 elements that make this precision forestry 

## Computer vision

Computer Vision (CV) is the heart of our precision forestry technology. There are multiple use cases, such as tree counting, weed detection, and blankspot identification. A use case is a task that CV handles to serve as a service related to forestry inventory and management. The CV runs parallel on multiple computers enabled with GPU drivers. Before all use cases run, an Automated Image Quality Control (AutoQC) service which is also CV-based processes process the raw images captured by UAV drones, stored in, and transferred through the **File Transfer Protocol (FTP)**, and determines if an image passes or not depending on the quality of image. For example, the image must not be cloudy or blurred. 

After an image passes the AutoQC gate, use cases automatically run and start to retrieve metadata from the database about that particular image, for example which *Petak* does the image come from, what stratum (species and age) the *Petak* is, and so on. The stratum metadata triggers the service to pick the relevant CV model since different stratum use different model, for example tree count and weed. The results from the use cases are stored in the FTP server and the output metadata, for example tree stocking percentage, weed percentage, and blankspot percentage are stored in the database. 

Next, each use case triggers alert whenever the percentage threshold is reached, for example, when the *Petak* has high weed percentage of 50% above the acceptable threshold 5% percentage. 

## Extract, Transform, Load (ETL)

ETL technology plays an important role in processing and storing the metadata from and to the database which the computer vision use cases need to run. For example, the ETL is responsible for file transfer when moving the raw to passed images after AutoQC, and also processing the alert data triggered from the CV use cases that is already stored in the database. 

Realizing the potential of IT in delivering values for precision forestry, the future of more advanced IT applications pave a way to help more businesses and organizations towards sustainability. 

<!--
## Mobile apps

Mobile apps 

## Dashboard Forestry Management Information System (FMIS) 
