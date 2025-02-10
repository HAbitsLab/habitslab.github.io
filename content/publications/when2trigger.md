---
title: "When2Trigger: Evaluation Trade-Offs in Vision-Based Real-Time Eating Detection Systems"
date: 2024-10-15T15:09:31-06:00
draft: false
authors: [{name: "Soroush Shahi", profile: "/profiles/soroush"}, {name: "Glenn Fernandes", profile: "/profiles/glenn"}, {name: "Chris Romano", profile: "profiles/chris"}, {name: "Nabil Alshurafa", profile: "/profiles/nabil"}]
has_github_link: true
github_link: "https://ieeexplore.ieee.org/abstract/document/10780481"

---

### Abstract

Wearable camera and thermal sensing systems are increasingly used for real-time eating detection and timely notifications to remind users to log their meals. However, confounding gestures such as irrelevant hand movements can cause false device confirmations of eating in real-time. Delaying the device confirmation of an eating episode, until the system is certain, can improve accuracy of eating detection, but prevents the capture of shorter bouts of eating. Balancing the trade-off between errors and detection delay is key to developing effective methods that provide immediate user feedback. This paper presents a real-time, hand-object-based method for automated detection of eating and drinking gestures and identifies the minimum number of gestures needed to reliably detect an eating episode. Unlike prior work, our method considers both hand motion and the object-in-hand and uses a low-power thermal sensor to reduce false positives. We evaluated our method on 36 participants, 28 of whom wore a wearable camera for up to 14 days in free-living environments. The results show that eating episodes can be accurately detected using 10 gestures or within the first 1.5 minutes of the eating episode, achieving an Fl-score of 89.0%. Our findings provide evaluation guidelines for designing real-time intervention systems to address problematic eating behaviors.