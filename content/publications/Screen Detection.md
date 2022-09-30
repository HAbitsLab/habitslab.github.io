---
title: "Detecting Screen Presence with Activity-Oriented RGB Camera in Egocentric Videos"
date: 2022-09-29T15:09:31-06:00
draft: false
authors: [{name: "Amit Adate", profile: ""}, {name: "Soroush Shahi", profile: "/profiles/soroush"}, {name: "Rawan Alharbi", profile: ""}, {name: "Sougata Sen", profile: ""}, {name: "Yang Gao", profile: ""}, {name: "Aggelos K Katsaggelos", profile: ""}, {name: "Nabil Alshurafa", profile: ""}]
has_github_link: false
github_link: "https://github.com"

---

### Abstract

Screen time is associated with several health risk behaviors including mindless eating, sedentary behavior, and decreased academic performance. Screen time behavior is traditionally assessed with self-report measures, which are known to be burdensome, inaccurate, and imprecise. Recent methods to automatically detect screen time are geared more towards detecting television screens from wearable cameras that record high-resolution video. Activity-oriented wearable cameras (i.e., cameras oriented towards the wearer with a fisheye lens) have recently been designed and shown to reduce privacy concerns, yet pose a greater challenge in capturing screens due to their orientation and fewer pixels on target. Methods that detect screens from low-power, low-resolution wearable camera video are needed given the increased adoption of such devices in longitudinal studies. We propose a method that leverages deep learning algorithms and lower-resolution images from an activity-oriented camera to detect screen presence from multiple types of screens with high variability of pixel on target (e.g., near and far TV, smartphones, laptops, and tablets). We test our system in a real-world study comprising 10 individuals, 80 hours of data, and 1.2 million low-resolution RGB frames. Our results outperform existing state-of-the-art video screen detection methods yielding an F1-score of 81%. This paper demonstrates the potential for detecting screen-watching behavior in longitudinal studies using activity-oriented cameras, paving the way for a nuanced understanding of screen time’s relationship with health risk behaviors.


![Example image](/img/screen_detection_framework.png)





