---
title: "CoughTrigger: Earbuds IMU Based Cough Detection Activator Using An Energy-efficient Sensitivity-prioritized Time Series Classifier"
date: 2021-11-07T15:09:31-06:00
draft: false
primary_investigator: {name: "Nabil Alshurafa", 
                       title: "Ph.D., Director of HABits Lab", 
                       description: "Assistant Professor of Preventive Medicine and of Computer Science at Northwestern University and heading The HAbits Lab.", 
                       img: "/img/pro-big.png",
                       profile: "/profiles/firstname_lastname"}
authors: [{name: "Nabil Alshurafa", profile: "/profiles/firstname_lastname"}, {name: "Nabil Alshurafa", profile: "/profiles/firstname_lastname"}]
has_github_link: false
github_link: "https://github.com/"

---

### Abstract

Persistent coughs are a major symptom of respiratory-related diseases. Increasing research attention has been paid to detecting coughs using wearables, especially during the COVID-19 pandemic. Microphone is most widely used sensor to detect coughs. However, the intense power consumption needed to process audio hinders continuous audio-based cough detection on battery-limited commercial wearables, such as earbuds. We present CoughTrigger, which utilizes a lower-power sensor, inertial measurement unit (IMU), in earbuds as a cough detection activator to trigger a higher-power sensor for audio processing and classification. It runs all-the-time as a standby service with minimal battery consumption and triggers the audio-based cough detection when a candidate cough is detected from IMU. Besides, the use of IMU brings the benefit of improved specificity of cough detection. Experiments are conducted on 45 subjects and CoughTrigger achieved 0.77 AUC score. We also validated its effectiveness on free-living data and through on-device implementation.
