---
title: "THOR: Thermal-guided Hand-Object Reasoning via Adaptive Vision Sampling"
date: 2025-07-08T15:09:31-06:00
draft: false
authors: [{name: "Soroush Shahi", profile: "/profiles/soroush"},{name: "Farzad Shahabi", profile: "/profiles/farzad"},{name: "Rama Nabulsi"}, {name: "Glenn Fernandes", profile: "/profiles/glenn"}, {name: "Aggelos Katsaggelos"}, {name: "Nabil Alshurafa", profile: "/profiles/nabil"}]
has_github_link: true
github_link: "https://arxiv.org/abs/2507.06442"

---

### Abstract

Wearable cameras are increasingly used as an observational and interventional tool for human behaviors by providing detailed visual data of hand-related activities. This data can be leveraged to facilitate memory recall for logging of behavior or timely interventions aimed at improving health. However, continuous processing of RGB images from these cameras consumes significant power impacting battery lifetime, generates a large volume of unnecessary video data for post-processing, raises privacy concerns, and requires substantial computational resources for real-time analysis. We introduce THOR, a real-time adaptive spatio-temporal RGB frame sampling method that leverages thermal sensing to capture hand-object patches and classify them in real-time. We use low-resolution thermal camera data to identify moments when a person switches from one hand-related activity to another, and adjust the RGB frame sampling rate by increasing it during activity transitions and reducing it during periods of sustained activity. Additionally, we use the thermal cues from the hand to localize the region of interest (i.e., the hand-object interaction) in each RGB frame, allowing the system to crop and process only the necessary part of the image for activity recognition. We develop a wearable device to validate our method through an in-the-wild study with 14 participants and over 30 activities, and further evaluate it on Ego4D (923 participants across 9 countries, totaling 3,670 hours of video). Our results show that using only 3% of the original RGB video data, our method captures all the activity segments, and achieves hand-related activity recognition F1-score (95%) comparable to using the entire RGB video (94%). Our work provides a more practical path for the longitudinal use of wearable cameras to monitor hand-related activities and health-risk behaviors in real time.