---
title: "SmartAct: Energy Efficient and Real-Time Hand-to-Mouth Gesture Detection Using Wearable RGB-T"
date: 2022-09-29T15:09:31-06:00
draft: false
authors: [{name: "Soroush Shahi", profile: "/profiles/soroush"}, {name: "Mahdi Pedram", profile: "/profiles/mahdi"}, {name: "Glenn Fernandes", profile: "/profiles/glenn"}, {name: "Nabil Alshurafa", profile: "/profiles/nabil"}]
has_github_link: false
github_link: "https://github.com/"

---

### Abstract

Researchers have been leveraging wearable cameras to both visually confirm and automatically detect individuals' eating habits. However, energy-intensive tasks such as continuously collecting and storing RGB images in memory, or running algorithms in real-time to automate detection of eating, greatly impacts battery life. Since eating moments are spread sparsely throughout the day, battery life can be mitigated by recording and processing data only when there is a high likelihood of eating. We present a framework comprising a golf-ball sized wearable device using a low-powered thermal sensor array and real-time activation algorithm that activates high-energy tasks when a hand-to-mouth gesture is confirmed by the thermal sensor array. The high-energy tasks tested are turning on the RGB camera (Trigger RGB mode) and running inference on an on-device machine learning model (Trigger ML mode). Our experimental setup involved the design of a wearable camera, 6 participants collecting 18 hours of data with and without eating, the implementation of a feeding gesture detection algorithm on-device, and measures of power saving using our activation method. Our activation algorithm demonstrates an average of at-least 31.5\% increase in battery life time, with minimal drop of recall (5%) and without impacting the accuracy of detecting eating (a slight 4.1% increase in F1-Score).


![Example image](/img/SmartAct_Framework.png)





