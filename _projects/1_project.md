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

<br>

# <span style="font-size: 20px;">Subobjective 2</span>

The second objective of this project was to develop a tracking algorithm capable of obtaining the ID of each pig housed in a group environment and re-identifying each pigs when going out of the field of view and then reappearing. Therefore, extra re-identification (re-ID) features were extracted in order to associate the pigs. Additionally, the total number of pigs was introduced as a constraint, and three associations based on Intersection over Union (IoU) and re-ID features were made to avoid introducing too many ID numbers. As a result, the developed tracking algorithm had a tracking percentage of 16.78% per individual on a 85-min-long video, which was improved a lot compared to studies not using re-ID features. Although there is still room to improve the performance, the developed tracking algorithm can solve the ID switching problem to some extent and could thus potentially be used for other applications as well. The video demo below displays a straightforward case of re-identifying pigs as they re-enter the field of view. The the corresponding paper can be accessed through this [link](https://doi.org/10.1016/j.biosystemseng.2022.07.017).

<!-- Video Embed -->
<div style="display: flex; justify-content: center; align-items: center;">
  <video autoplay controls loop muted style="max-width: 800px; width: 100%;">
    <source src="{{ site.baseurl }}/assets/img/project1-3.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
</div>

<br>

# <span style="font-size: 20px;">Subobjective 3</span>

Regarding the third subobjective, an experiment on the effect of varying temperature profile on RR was conducted on 5 pigs that were housed in a group. Four of these pigs wore ECG devices to collect the GS measurement, whereas one control pig did not wear a belt in order to rule out the effect of the belt. Videos were continuously recorded during the experiment. An algorithm was developed to monitor the RR of pigs in an automatic way, where each pig was detected first with an oriented bounding box, after which the RR was extracted by analysing the time-varying features extracted from the middle 1/3 of the bounding box. The comparison with GS showed good agreement with an MAE of 2.38 breaths/minute in the 4 pigs wearing belts and 1.72 breaths/min in the control pig, an RMSE of 3.46 breaths/min in the 4 pigs wearing belts and 2.26 breaths/min in the control pig, and a correlation coefficient of 0.92 in the 4 pigs wearing belts and 0.95 in the control pig. Below is a video demonstrating the RR monitoring of a pig housed in a group. The corresponding paper can be accessed through this [link](https://doi.org/10.1016/j.compag.2023.107899).

<!-- Video Embed -->
<div style="display: flex; justify-content: center; align-items: center;">
  <video autoplay controls loop muted style="max-width: 800px; width: 100%;">
    <source src="{{ site.baseurl }}/assets/img/project1-4.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
</div>


<br>