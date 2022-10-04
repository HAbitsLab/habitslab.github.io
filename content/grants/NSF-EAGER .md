---
title: "EAGER: Privacy Enhancing Framework to Advance Behavior Models"
date: 2019-06-05 T15:09:31-06:00
draft: false
logo_image: "/img/nsf.png"
start_year: 2019
end_year: 2022
funding_amount: "$299,471"
primary_investigator: {name: "Nabil Alshurafa", 
                       title: "Ph.D., Director of HABits Lab", 
                       description: "Assistant Professor of Preventive Medicine and of Computer Science at Northwestern University and heading The HAbits Lab.", 
                       img: "/img/pro-big.png",
                       profile: "https://www.feinberg.northwestern.edu/faculty-profiles/az/profile.html?xid=33330"}
                       
coinvestigators: [{name: "Josiah Hester", title: "Associate Professor of Interactive Computing and Computer Science
College of Computing, Georgia Institute of Technology", description: "desction description description", img: "/img/josiah.png", profile: "https://josiahhester.com/cv/"},{name: "Aggelos Katsaggelos", title: "Prof. of Electrical and Computer Engineering and Computer Science", description: "description description description", img: "/img/aggelos.png", profile: "https://www.mccormick.northwestern.edu/research-faculty/directory/profiles/katsaggelos-aggelos.html"}, 
                {name: "Bonnie Spring", title: "Professor of Preventive Medicine (Behavioral Medicine), Psychiatry and Behavioral Sciences and Weinberg College of Arts and Sciences", description: "desction description description", img: "/img/bonnie_spring.png", profile: "https://www.feinberg.northwestern.edu/faculty-profiles/az/profile.html?xid=16136"},
                {name: "Andrea Graham", title: "Assistant Professor of Medical Social Sciences and Preventive Medicine", description: "desction description description", img: "/img/andrea_graham.png", profile: "https://www.feinberg.northwestern.edu/faculty-profiles/az/profile.html?xid=41225"}]
---

### 1. Introduction

This project is designed to advance research on problematic eating behavior. The project investigates wearable sensors to measure eating behavior and developing models of behavior that comprise multiple observable behaviors such as eating alone or with friends, or chewing speed. These data can help scientists improve upon current traditional methods such as self-reported eating diaries, which tend to be inconsistent, sparse, and rarely timely. We capture human behavior using a custom wearable augmented camera. Wearable cameras provide rich data, but raise privacy concerns. The project will address these concerns by building a framework using machine learning and information theory while including human-reported privacy concerns. The framework will address wearers' concerns that may limit recording authentic behavior in real-world settings and will optimize algorithms to enhance the detection and classification of human behavior.

The project explores the acceptability of obfuscation techniques on varied activities and their requisite tasks. The proposed research will design a suite of computationally efficient task-specific algorithms that use raw images in computationally restrictive (in situ) and obfuscated images in unrestrictive environments (offline) to build information-performance curves for the scalable development of personalized ground truth wearable cameras. The project also will develop a modular, plug-and-play, low-complexity and efficient obfuscation computing hardware device to facilitate and accelerate the use of the proposed methods and algorithms. This work will validate an overeating behavior model in a real-world setting using the design framework and device, providing visual confirmation of eating behaviors, showing how it can be used to test existing models. This project is likely to be useful to other domains in the social sciences, fundamentally changing the way researchers build and validate behavioral models in real-world settings. There are potential applications in health (especially preventive medicine), social, and economic sciences: energy balance, infant development, medication adherence, consumer behavior, and human-environment interaction.  
<p align="center">
![image](/img/eager/lhs.png)  
</p>  
Our system aims to provide robust and untethered monitoring of behavioral health that can follow users throughout their daily lives with minimal burden and privacy concern. 

This award reflects NSF's statutory mission and has been deemed worthy of support through evaluation using the Foundation's intellectual merit and broader impacts review criteria.


### 2. Development
## Prototyping the wearable
![image](/img/eager/PROTOTYPE.png)

Previous wearable cameras were egocentric, meaning they capture a field-of-view similar to the wearer's perspective (i.e., "POV"). Egocentric camera orientations impose substantial privacy costs on wearers, as information irrelevant to health behaviors (e.g., eating, drinking, smoking) is frequently captured. To address the challenges of egocentric recording, we developed an activity-oriented wearable visual system that aims to capture only the most relevant area (in this case, the mouth) to the detection of health behaviors.  
## ActiSight: An activity-oriented wearable camera
For our first iteration, we built an activity-oriented wearable that is mounted on the chest and faces directly upwards, as shown below:
![image](/img/eager/as1a.png)

ActiSight collects a dual-image multimodal sensor stream. Color video is recorded by a camera module (ArduCam OV2640) and thermal images are captured with a low-res 8x8 infrared sensor array (SparkFun Grid-EYE AMG8833). For each module, a sample frame is shown below:
![image](/img/eager/as1b.png)

To conserve power, we implemented a trigger system that continuously monitors the thermal array (low power draw) and selectively activates the camera module (high power draw). The trigger responds to thermal utility, i.e., whether the thermal image alone is intelligible to an onboard computer vision model. A diagram depicting the trigger logic is shown below:
![image](/img/eager/as1c.png)

With our combined thermal and visual inputs, we perform feature extraction on the collected images. Wearer/background extraction is depicted on sample frames below:
![image](/img/eager/as1d.png)

ActiSight Hardware/Firmware: https://github.com/HAbitsLab/ActiSight  
## SenseWhy: High-res thermal and low-light recording
In our next iteration, we used a thermal array with a higher resolution (32x24), incorporated an analog night-vision circuit comprised of a photoresistor and infrared light-emitting diode (IR-LED), and designed a new case that is 3D printed from a flexible filament.
![image](/img/eager/sw1.png)  
We present the hardware schematic here:  
![image](/img/eager/sw5.png)


SenseWhy Hardware/Firmware: https://github.com/HAbitsLab/R03-Wildcam  
## WildCam: A user-centric visual wearable
We then re-designed the device based on lessons learned from deploying the previous designs in studies.  

Schematic:
![image](/img/eager/wc1.png)  
We attach a flatpack battery directly to the main PCB to reduce the bulk of the backplate. We improve the stability of the night vision circuit by attaching the photocell and IR-LED components to a dedicated breakout board.  

We also revised the case design:  
![image](/img/eager/wc2.gif)  
We developed four backplates, each at a different angle, to accomodate a wider range of body-shapes. We also return to the rigid enclosure design, this time printing with material jetting for a high-quality feel.  
![image](/img/eager/wc3.png)  
We improved our alignment of the RGB and high-res thermal sensor inputs with a procedural registration process, allowing us to perform more sophisticated multimodal operations on the datastream.  

WildCam Hardware/Firmware: https://github.com/HAbitsLab/R03-Wildcam  
## HeatSight: Thermal behavior understanding
We experimented with thermal-only systems with HeatSight:  
![image](/img/eager/hs1f.png) 
## SmartAct: A wearable smartcam
Finally, we developed SmartAct:
![image](/img/eager/sa1.png) 
SmartAct Hardware/Firmware: https://github.com/HAbitsLab/BSN22Trigger  

### 3. Publications

1. Zhang, Shibo and Zhao, Yuqi and Nguyen, Dzung Tri and Xu, Runsheng and Sen, Sougata and Hester, Josiah and Alshurafa, Nabil "NeckSense: A Multi-Sensor Necklace for Detecting Eating Activities in Free-Living Conditions" Proceedings of the ACM on Interactive, Mobile, Wearable and Ubiquitous Technologies , v.4 , 2020 10.1145/3397313

2. Bolton, Connor and Fu, Kevin and Hester, Josiah and Han, Jun "How to curtail oversensing in the home" Communications of the ACM , v.63 , 2020 10.1145/3396261

3. Alharbi, Rawan and Tolba, Mariam and Petito, Lucia C. and Hester, Josiah and Alshurafa, Nabil "To Mask or Not to Mask?: Balancing Privacy with Visual Confirmation Utility in Activity-Oriented Wearable Cameras" Proceedings of the ACM on Interactive, Mobile, Wearable and Ubiquitous Technologies , v.3 , 2019 10.1145/3351230

4. Alharbi, R., Tolba, M., Petito, L. C., Hester, J., & Alshurafa, N. (2019). To Mask or Not to Mask? Balancing Privacy with Visual Confirmation Utility in Activity-Oriented Wearable Cameras. Proceedings of the ACM on Interactive, Mobile, Wearable and Ubiquitous Technologies, 3(3), 72:1-72:29. https://doi.org/10.1145/3351230

5. Shahi, S., Alharbi, R., Gao, Y., Sen, S., Katsaggelos, A. K., Hester, J., & Alshurafa, N. (2022). Impacts of Image Obfuscation on Fine-grained Activity Recognition in Egocentric Video. 2022 IEEE International Conference on Pervasive Computing and Communications Workshops and Other Affiliated Events (PerCom Workshops), 341–346. https://doi.org/10.1109/PerComWorkshops53856.2022.9767447

6. Adate, A., Shahi, S., Alharbi, R., Sen, S., Gao, Y., Katsaggelos, A. K., & Alshurafa, N. (2022). Detecting Screen Presence with Activity-Oriented RGB Camera in Egocentric Videos. 2022 IEEE International Conference on Pervasive Computing and Communications Workshops and Other Affiliated Events (PerCom Workshops), 403–408. https://doi.org/10.1109/PerComWorkshops53856.2022.9767433

7. F. Shahabi, Y. Gao and N. Alshurafa, "ActiveSense: A Novel Active Learning Framework for Human Activity Recognition," 2022 IEEE International Conference on Pervasive Computing and Communications Workshops and other Affiliated Events (PerCom Workshops), 2022, pp. 224-229, doi: 10.1109/PerComWorkshops53856.2022.9767388.

8. Alharbi, R., Sen, S., Ng, A., Alshurafa, N., & Hester, J. (2022). ActiSight: Wearer Foreground Extraction Using a Practical RGB-Thermal Wearable. 2022 IEEE International Conference on Pervasive Computing and Communications (PerCom), 237–246. https://doi.org/10.1109/PerCom53586.2022.9762385

9. Zhang, S., Zhao, Y., Nguyen, D. T., Xu, R., Sen, S., Hester, J., & Alshurafa, N. (2020). NeckSense: A Multi-Sensor Necklace for Detecting Eating Activities in Free-Living Conditions. Proceedings of the ACM on Interactive, Mobile, Wearable and Ubiquitous Technologies, 4(2), 72:1-72:26. https://doi.org/10.1145/3397313

10. Bolton, C., Fu, K., Hester, J., & Han, J. (2020). How to curtail oversensing in the home. Communications of the ACM, 63(6), 20–24. https://doi.org/10.1145/3396261

11. Alshurafa, N., Zhang, S., Romano, C., Zhang, H., Pfammatter, A. F., & Lin, A. W. (2021). Association of number of bites and eating speed with energy intake: Wearable technology results under free-living conditions. Appetite, 167, 105653. https://doi.org/10.1016/j.appet.2021.105653

12. Alharbi, R., Feng, C., Sen, S., Jain, J., Hester, J., & Alshurafa, N. (2021). HeatSight: Wearable Low-power Omni Thermal Sensing. 2021 International Symposium on Wearable Computers, 108–112. https://doi.org/10.1145/3460421.3478811

13. Sen, S., Lee, S. I., Jackson, R., Wang, R., Alshurafa, N., Hester, J., & Gummeson, J. (2020). Towards Battery-Free Body Sensor Networks. Proceedings of the 8th International Workshop on Energy Harvesting and Energy-Neutral Sensing Systems, 79–81. https://doi.org/10.1145/3417308.3430275

14. Zhang, Y. C., Zhang, S., Liu, M., Daly, E., Battalio, S., Kumar, S., Spring, B., Rehg, J. M., & Alshurafa, N. (2020). SyncWISE: Window Induced Shift Estimation for Synchronization of Video and Accelerometry from Wearable Sensors. Proceedings of the ACM on Interactive, Mobile, Wearable and Ubiquitous Technologies, 4(3), 107:1-107:26. https://doi.org/10.1145/3411824
