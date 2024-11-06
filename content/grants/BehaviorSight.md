---
title: "BehaviorSight: Privacy Enhancing Wearable System to Detect Health Risk Behaviors in Real-time"
date: 2020-09-07T15:09:31-06:00
draft: false
logo_image: "/img/nh.png"
start_year: 2020
end_year: 2023
funding_amount: "$606,713"
primary_investigator: 
    {name: "Nabil Alshurafa", 
    title: "Director of HABits Lab", 
    description: "Assocate Professor of Preventive Medicine and Computer Science, Northwestern University", 
    img: "/img/pro-big.png",
    profile: "/profiles/nabil"}

coinvestigators: [
    {name: "Bonnie Spring",
    title: "Professor of Preventive Medicine", 
    img: "/img/bonnie_spring.png"},

    {name: "Aggelos Katsaggelos",
    title: "Professor of Electrical and Computer Engineering",
    img: "/img/aggelos.png"},

    {name: "Josiah Hester",
    title: "Associate Professor of Interactive Computing and Computer Science",
    img: "/img/josiah.png"}
    ]

studentinvestigators: [
    {name: "Glenn Fernandes",
    img: "/img/im-6.png",
    profile: "/profiles/glenn"},
    {name: "Soroush Shahi",
    img: "/img/im-7.png",
    profile: "/profiles/soroush"},
    {name: "Saki Amagai",
    img: "/img/saki.jpg",
    profile: "/profiles/saki"},
    ]

mentors: {}
---

### Introduction

Many health-risk behaviors—such as overeating, smoking, drinking, substance abuse, and medication non-adherence—correlate with increased morbidity and mortality. Eliminating these behaviors can help prevent several diseases. However, this requires understanding, knowing, and altering what people put into their mouth. Current efforts to understand behaviors associated with detecting what people put in their mouth are limited and rely on inaccurate and biased self-reports. Detecting these behaviors objectively and in real time, learning to automatically predict them, and adaptively intervening to problematic behaviors will pave the way for novel behavioral interventions.

Wearable video cameras can automatically detect these health-risk behaviors in real time, enabling personalized and adaptive interventions, while providing valuable visual confirmation of wearer’s activities to an end user (e.g., clinical team, health coach, and dietitian). However, video recordings pose serious bystander privacy concerns, which is a leading cause for people’s inhibition to wearing cameras in daily life. To address this concern, new methods must be developed to automatically detect health-risk behaviors and record videos of only the wearer and objects in close proximity to the wearer, while de-identifying distant objects or bystanders. Infrared (IR) sensor arrays have the potential to provide independent temperature readings, which allows determining whether an object is near or far. Applying machine learning algorithms to IR sensor array data enables detection of nearby objects (e.g., wearer’s hand, objects in the hand). These algorithms can further infer what the wearer is putting in his or her mouth.


### Developing "HabitSense", a new, lightweight, power-efficient wearable device where the IR sensor controls camera recording

[ACM IMWUT Paper Link](https://dl.acm.org/doi/abs/10.1145/3678591)

__HabitSense__ is a neck-worn wearable platform that combines RGB, thermal, and accelerometer sensors to detect health-risk behaviors like eating and smoking in real-time. The device is designed to prioritize user privacy and effectiveness, providing an innovative solution for real-world health monitoring applications.

![Example image](/img/hs-fig-main.png)  
  

#### __Key Features:__

__Clinically-Informed Design:__ HabitSense was developed in collaboration with 36 weight management and smoking cessation experts. Their insights were crucial in shaping a device that meets real-world healthcare needs, ensuring alignment with clinical workflows and enhancing adoption in healthcare settings.

__User-Centric Development:__ Extensive feedback from 105 participants guided the design of HabitSense, resulting in a lightweight, comfortable, and unobtrusive device optimized for all-day wear. The platform effectively detects eating and smoking gestures using a combination of RGB and thermal sensors while maintaining user privacy.

__Modular and Expandable Architecture:__ HabitSense features a modular design that allows for easy repair, sensor upgrades, and component additions. This flexibility not only reduces costs and electronic waste but also ensures the device can be adapted for various health-monitoring applications, such as monitoring UV exposure or medication adherence.

![Example image](/img/r21-components.png)

__Advanced Privacy Protection:__ The platform employs the S.E.C.U.R.E. (Sensor-Enabled Control for Ubiquitous Recording and Evaluation) algorithm, which activates recording only during detected health-risk behaviors. This smart activation reduces data storage by 48% and extends battery life by 30%, balancing privacy with functionality.

![Example image](/img/flowchart.png)

__On-Device Obfuscation Algorithm:__ To further protect privacy, HabitSense utilizes a novel on-device obfuscation algorithm. This algorithm uses thermal data to mask background details while keeping relevant foreground activities like hand-to-mouth gestures visible, ensuring user privacy while maintaining the accuracy of behavior detection.

![Example image](/img/obfuscation.png)

__Energy-Efficient Operation:__ The device employs a multi-tiered activation strategy that leverages accelerometer data, thermal sensors, and intelligent algorithms to minimize power consumption. This approach ensures HabitSense can operate for a full day on a single charge, providing reliable and continuous monitoring.

__HELP Tool for Enhanced Data Annotation:__ The HabitSense Exploration and Labeling Platform (HELP) was developed to streamline the annotation of multimodal data collected by HabitSense. This tool improves the accuracy and efficiency of labeling behaviors, enhancing the training of AI models used for behavior detection.

__AI-Powered Gesture Recognition:__ HabitSense incorporates state-of-the-art AI models that achieved a 92% F1-score in detecting hand-to-mouth gestures, critical for recognizing eating and smoking behaviors. The models are robust against varying conditions, such as low light and intense movement, ensuring reliable performance in diverse settings.

__Comprehensive Real-World Evaluation:__ The device was tested in real-world settings with 15 participants, capturing 768 hours of footage. The evaluation demonstrated high user acceptability and effectiveness in detecting health-risk behaviors, confirming HabitSense’s suitability for use in everyday environments.

__Iterative Design Process:__ HabitSense was developed through multiple design iterations, from Gen 1 to the final version, incorporating feedback from users and addressing challenges related to comfort, usability, and data accuracy. This iterative process resulted in a refined device that is practical and user-friendly.

![Example image](/img/r21-case.png)

### Impact

HabitSense offers a groundbreaking approach to real-time, privacy-preserving monitoring of health-risk behaviors. With its clinician-informed design, user-centric development, advanced privacy features, and robust performance, it provides a feasible and effective tool for real-world health applications. Beyond detecting eating and smoking, HabitSense has the potential to monitor other behaviors, such as medication adherence, further expanding its scope in healthcare. Join us on this journey to revolutionize health monitoring!