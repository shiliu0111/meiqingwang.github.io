---
layout: page
title: Development of Automatic Physiological and Behavioural Monitoring Systems for Pigs
description: Doctoral project 
img: assets/img/12.jpg
importance: 1
category: work
related_publications: true
---

# <span style="font-size: 22px;">Project Background and Objective</span>


Automated physiological and behavioural monitoring can play a major role in assessing the welfare of pigs. Conventional behaviour monitoring through human observers is time-consuming and labour-intensive. Wearable sensors to measure activity and physiological signals also need to be attached to animals, and so are not robust and animal-friendly for long-term monitoring. The aim of this project was to explore new approaches for monitoring of physiological and behavioural parameters of pigs as a means towards improving animal welfare.  More specifically, given the prevailing advantages this project focuses on developing contactless video-based methods to monitor the heart rate (HR), respiration rate (RR) and postural behaviour of pigs. The project was devided into 3 sub-objectives:
 
  - to verify whether the physiological parameters and behaviours could be extracted from and monitored based on RGB videos.
  - to develop a tracking algorithm capable of identifying and tracking individual pigs in a group-housed environment.
  - to assess whether physiological parameters can be effectively monitored in group-housed situations.

# <span style="font-size: 20px;">Subobjective 1</span>

For the first sub-objective, HR and postural behaviour of a single pig were extracted and monitored respectively. To monitor the HR, the videos of an anesthetized and a resting pig were recorded while pigs wore electrocardiogram (ECG) devices for collecting the Gold Standard (GS) of HR. The HR of the pigs were extracted by frequency analysis. Compared with the GS, the extracted HR had 2.33 beats/minute in mean absolute error (MAE) resulting in 2.13% of MAE over averaged HR, 3.09 beats/min in root mean square error (RMSE) resulting in 2.83 % of RMSE over averaged HR, and 67% in HR estimation error below 3.5 beats/min for the anesthetized pig, and 4.69 beats/min in MAE (2.91% over averaged HR), 6.43 beats/min in RMSE (3.98% over averaged HR) and 57% in for the resting pig. A video demo in below shows the monitroing of HR from a short RGB video. This work has been published in a peer-reviewed journal, and the paper can be accessed via this [link](https://doi.org/10.3390/ani11020442).   

<!-- Video Embed -->
<div style="display: flex; justify-content: center; align-items: center;">
  <video autoplay controls loop muted style="max-width: 800px; width: 100%;">
    <source src="{{ site.baseurl }}/assets/img/project1-1.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
</div>

<br>

In a similar way, behaviour monitoring was conducted on the video of lactating sows, where each sow was separately housed and the videos of different postural behaviours were recorded. The behaviours were classified by extracting the spatial and temporal features from the videos based on a deep learning method and Principle Component Analysis (PCA). Accuracies of 95.33% and 92.67% were obtained on videos without and with piglets, respectively. The video below demonstrates the monitoring of the sow's postural behavior. The paper regarding this work can be found via this [link](https://doi.org/10.1016/j.compag.2021.106351).

<!-- Video Embed -->
<div style="display: flex; justify-content: center; align-items: center;">
  <video autoplay controls loop muted style="max-width: 800px; width: 100%;">
    <source src="{{ site.baseurl }}/assets/img/project1-2.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
</div>
