---
title: "WildCam: A Privacy Conscious Wearable Eating Detection Camera People will Actually Wear in the Wild"
date: 2021-01-29T15:09:31-06:00
draft: false
logo_image: "/img/nh.png"
start_year: 2020
end_year: 2022
funding_amount: "$233,587"
primary_investigator: {name: "Nabil Alshurafa", 
                       title: "Ph.D., Director of HABits Lab", 
                       description: "Assistant Professor of Preventive Medicine and of Computer Science at Northwestern University and heading The HAbits Lab.", 
                       img: "/img/pro-big.png",
                       profile: "https://www.github.com"}
coinvestigators: [
    # {name: "Name1", title: "Researcher", description: "description description description", img: "/img/im-8.png", profile: "https://www.github.com"}, 
    #             {name: "Name2", title: "Researcher", description: "desction description description", img: "/img/im-7.png", profile: "https://www.github.com"}
                ]
---

<!-- #### Grant Information
**Funding Agency:** National Institute of Health (NIH)  
**Funding Institute:** National Institute of Diabetes and Digestive and Kidney Diseases (NIDDK)  
**Type:** Small Research Grants (R03)  
**Project #:** 1R03DK127128-01  
**Project Start:** 1 Feb 2021  
**Project End:** 31 Jan 2023 -->

<!-- [Grantome page](https://grantome.com/grant/NIH/R03-DK127128-01) -->

### Background

The research, assessment, and treatment of unhealthy eating habits all rely on self reporting. That is, the patient or client must record their own dietary intake by using a food journal. This method of diet tracking has [proven problematic](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3268700/), as much dietary information is lost due forgetting, non-adherence, dishonesty, and so forth. Because diet information is critical to the work of behavioral clinicians and researchers, a better method for diet monitoring is needed. In our project, "WildCam", we aim to develop such a method via a wearable camera system, accounting for known user-experience issues associated with wearable cameras, including comfort, privacy concerns, and social stigma. 

### System Development

We develop "WildCam", a wearable camera that sits on the chest and hosts an upward-facing sensor array that captures the user's face and mouth area with both RGB and infrared thermal imaging.

##### Internal design schematics:
![Schematics GIF](/img/wc-sch-crop.gif)
<!-- ![Schematic image of WildCam Device](/img/wildcamschema.png) -->
A master PCB (light green) houses the MCU, which controls the attached thermal (red), RGB (dark green), and night vision (purple) modules. Users power the device on and off via a switch (black and grey). When the device is on, input from the thermal and RGB sensors is written to the onboard SD card (red and gold) in an encrypted format. 

##### Enclosure design

![Enclosure gif](/img/eager/wc2.gif)

WildCam's enclosure is a drop-safe 3D-printed casing made of a rigid filament. To account for different body shapes across the patient population, the backplate is removable and swappable with several other backplates of varying angles. 

##### Photo

![Photo of device on dummy](/img/wc-dummy.jpg)

The device on a mannequin. The neckband is adjustable to correct for height differences between patients. 

##### Obfuscation

Wearable cameras raise obvious privacy concerns among users. Obfuscation—the automatic censoring of visual data that are not essential to the assessment of dietary behaviors—can protect patients from the unwanted capture of sensitive information, reducing privacy concern and increasing acceptability (AKA willingness to wear) of the device.

In this project, we test 4 different obfuscation techniques in a randomized clinical trial:
1. raw (no obfuscation)
2. blur (sensitive information is blurred/pixelated)
3. edge (sensitive information is blacked out)
4. cartoon/avatar (a cartoon face covers the wearer's face)
  
*Examples:*
![Gif of obfuscation techniques](/img/obf.gif)

<!-- ![gif of CHI video](/img/chi-cartoon.gif) -->
### Research Approach


##### Research Question 1: How do different activity-oriented partial obfuscation filters affect the visual confirmation utility of identifying hand-related activities that involve hand-to-head gestures by a human viewer?

We investigate the *visual confirmation utility* of obfuscated video frames. That is, we apply obfuscation to videos and then check whether the desired dietary information is still intact. 

In particular, we want to compare the accuracy of human labels obtained from viewing non-obfuscated videos with the accuracy of the labels derived from viewing the obfuscated videos with different filters. Hand-to-head gestures can be confounding to each other if fine-grained and some contextual information is lost. Therefore, this comparison can help us to determine if the visual confirmation utility is preserved, or not, after applying activity-oriented partial obfuscation to it with different filters. It will also help us to understand the limitations of activity-oriented partial obfuscation and the filters applied.

##### Research Question 2: How do different activity-oriented partial obfuscation filters affect users' privacy concerns and willingness to wear the device?

Second, we explore patient attitudes towards each of the obfuscation techniques by presenting them daily clips of the data they have collected with obfuscation applied (or, in the *raw* condition, not applied). We assess patient attitudes both through directly surveying them and by comparing the mean daily wear time of patients using each obfuscation setting.

#### Results

Our clinicial trial has concluded and we are now analyzing the data. A results paper is coming soon!