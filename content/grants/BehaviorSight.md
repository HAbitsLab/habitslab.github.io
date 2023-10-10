---
title: "BehaviorSight: Privacy Enhancing Wearable System to Detect Health Risk Behaviors in Real-time"
date: 2020-09-07T15:09:31-06:00
draft: false
logo_image: "/img/nh.png"
start_year: 2020
end_year: 2023
funding_amount: "$606,713"
primary_investigator: {name: "Nabil Alshurafa", 
                       title: "Ph.D., Director of HABits Lab", 
                       description: "Assistant Professor of Preventive Medicine and of Computer Science at Northwestern University and heading The HAbits Lab.", 
                       img: "/img/pro-big.png",
                       profile: "https://www.github.com"}
coinvestigators: [{name: "Aggelos Katsaggelos", title: "Assistant Professor of Computer Science", description: "description description description", img: "/img/aggelos.png"}
                ]
---

### 1. Introduction

Many health-risk behaviors—such as overeating, smoking, drinking, substance abuse, and medication non-adherence—correlate with increased morbidity and mortality. Eliminating these behaviors can help prevent several diseases. However, this requires understanding, knowing, and altering what people put into their mouth. Current efforts to understand behaviors associated with detecting what people put in their mouth are limited and rely on inaccurate and biased self-reports. Detecting these behaviors objectively and in real time, learning to automatically predict them, and adaptively intervening to problematic behaviors will pave the way for novel behavioral interventions.

Wearable video cameras can automatically detect these health-risk behaviors in real time, enabling personalized and adaptive interventions, while providing valuable visual confirmation of wearer’s activities to an end user (e.g., clinical team, health coach, and dietitian). However, video recordings pose serious bystander privacy concerns, which is a leading cause for people’s inhibition to wearing cameras in daily life. To address this concern, new methods must be developed to automatically detect health-risk behaviors and record videos of only the wearer and objects in close proximity to the wearer, while de-identifying distant objects or bystanders. Infrared (IR) sensor arrays have the potential to provide independent temperature readings, which allows determining whether an object is near or far. Applying machine learning algorithms to IR sensor array data enables detection of nearby objects (e.g., wearer’s hand, objects in the hand). These algorithms can further infer what the wearer is putting in his or her mouth.


### Aim 1: Develop a new, lightweight, power-efficient wearable device where the IR sensor controls camera recording

#### __Components__
We aimed for modularity in designing our component schematic, future-proofing the device against the removal of specific components from the market. We also prioritized energy-efficient components to reduce power draw of the device.

##### HabitSense Components:
![Example image](/img/r21-components.png)
<!-- *Components used in the HabitSense device* -->

#### __Form-Factor__
We iterated through several designs of the 3D-printed enclosure before arriving at our final design. We sought to devise a casing that is lightweight, slim, aesthetically pleasing, and composed of product-quality material.

##### HabitSense Enclosure Iterations:
![Example image](/img/r21-case.png)
<!-- *Components used in the HabitSense device* -->

#### __Comparison to past iterations__

This wasn't our first rodeo! Here is what earlier wearable camera systems we developed look like, to give a sense of how we found our way to the present design.

##### HabitSense Generations:
![Example image](/img/r21-generations.jpg)
<!-- *Components used in the HabitSense device* -->

#### __Thermal-RGB Triggering System__

##### Trigger System Overview:
![Example image](/img/r21-trigger.png)
<!-- *Components used in the HabitSense device* -->


### Aim 2: Develop machine learning algorithms to reliably detect eating and smoking

### Aim 3: Validate the system’s ability to detect and visually confirm eating and smoking in real time


