---
title: "Tree Count for two-month *Eucalyptus pellita* plantation in Riau using YOLOv5 computer vision"
excerpt: "Tree count"
collection: portfolio
---

This project started when Sinarmas Forestry, our sister company, upgraded their remote sensing imaging from fixed-wing to quadcopter drone UAVs, around late 2021. This new quadcopter technology was tested in 3 districts in Riau where the *Eucalyptus pellita* (or EPEL) plantations with two-month age are located. The quadcopter drone was claimed to be able to produce higher resolution photos and higher stability while flying 150 m above the ground. Our data science team at Asia Pulp and Paper Sinarmas, had developed tree count models on variety of species and ages (we call it Stratum) based on Faster R-CNN and Mask R-CNN object detection models, mostly on the fixed-wing images. When these models were tested on the new quadcopter images, the accuracy (F1-score) was not so good. 

This was the main motivation I decided to develop more robust and more accurate tree count model using YOLOv5. The YOLOv5 is the fifth generation of You Only Look Once (YOLO) families released by Ultralytics in June 2021. The main challenge of developing tree count model on two-month-old EPEL plants is that the size of plants at this age is very small (around 0.3-0.5 m in size). As a comparison, the whole copter orthomosaic photo has size of [30000,30000] pixels or 600x600 m2 area. The YOLOv5 is proven to be very robust for detection of tiny objects. 
