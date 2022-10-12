---
title: "EAGER: SaTC: Early-Stage Interdisciplinary Collaboration: Privacy Enhancing Framework to Advance Behavior Models"
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

### Introduction

Studying human behavior has traditionally been theory-based, deriving a set of constructs or complex concepts (e.g., self-efficacy or attitude towards behavior) and relationships between variables to explain or predict behavior and then subjecting components of the theory to empirical testing. Ecological momentary assessments (EMAs) allow participants to report behavior when events occur using their smartphones. However, they are still prone to bias and prevent contextual understanding of behavior in free-living settings. Wearable mobile sensors enable quantitative representation of coarse (e.g., a person eating alone or with friends) and fine-grained behaviors (e.g., number of feeding gestures), facilitating the development of new behavioral models that explain and predict problematic behavior such as overeating. This will allow the behaviorist to construct models that more closely represent reality and enable the improved design of interventions that change behavior. However, building models of these behaviors requires a reliable, consistent, and constant source of ground truth for development and verification. Researchers can automatically uncover contextual information about human behavior in their natural habitat using wearable cameras combined with IR-sensor arrays and advanced computational methods. However, wearers' perception of the bystanders' privacy concerns is reported to be the leading reason people are not willing to wear cameras in daily life continuously. 

In this project, we designed and developed multiple wearable RGB cameras equipped with an infrared-sensing system that evaluates various obfuscation methods to verify human behavior in a real-world setting. In addition, we studied and tested the tradeoff between the wearer's acceptability of different obfuscation techniques before recording the video footage and the performance of various online and offline algorithms detecting specific human behavior. Our proposed method addresses the challenges for human behavior monitoring that can enable the development of behavioral models. Our approach supports how we build behavioral models based on objective, real-world behavior in free-living people. EAGER research tasks included (1) prototyping a modular and configurable hardware platform for energy-constrained human behavior monitoring, (2) developing intelligent obfuscation algorithms for enhancing privacy, and (3) running research studies to identify user's preferred obfuscation methods to evaluate the general utility of the wearable device for human behavior monitoring. 

![image](/img/eager/lhs.png)

We built a suite of wearable cameras equipped with a low-resolution thermal camera for all-day monitoring of four human activities including: eating, smoking, socializing, and screen time. We conducted multiple experiments to test acceptability, privacy concerns, and utility of different wearable cameras in free-living settings. We tested the device on 367 Amazon Mechanical Turkers, 20 people in a 2-day free-living study aimed at detecting eating, and 60 people in a 2-week study of people with obesity to detect overeating. As our cameras evolved, so did the number of hours of video footage collected per day by the participants, as privacy considerations continued to be addressed. The device is also miniaturized (last iteration was approximately golf-ball sized), can continuously collect RGB and thermal sensing data on-device, can transmit data via Bluetooth to a smartphone app, incorporates night-vision, and several case designs are available to address different body shapes and sizes. We have also tested several algorithms that can run offline on the obfuscated image, and also on-device to detect human gestures for applications related to eating and smoking. Our wearable device is configurable, and we have designed five different types of wearable devices depending on the application and need, ranging from privacy concern to battery lifetime, and depending on the type of activity that needs to be detected and whether real-time processing is necessary. 

Our wearable camera suite opens a new research program for human behavior recognition. This research enables the computational means for low-cost, continuous monitoring of human behavior. In the future, these devices can operate independently and extract all the required information using on-device machine learning for human behavior at a reduced size and cost. These devices will deliver actionable data, including notifications and suggestions to users, to control and observe their daily habits. In addition, these devices will provide human behavioralists with a tool that supports them in understanding human behaviors, enabling visual confirmation of human behavior using a tool that people are much more likely to wear in free-living settings. 

We have designed a scalable, low cost system that is capable of informing computational constraints and requirements in-situ and post-processing of obfuscation methods to allow for future information theory and resource allocation experts to optimize where algorithms should run taking into consideration wearer levels of concern. Our platform could be applied to nearly every study of human behavior to obtain precise predictors and determinants of behavior. This also significantly advances behavioral science to build more precise models and interventions that improve behavior in many fields. 

Our system aims to provide robust and untethered monitoring of behavioral health that can follow users throughout their daily lives with minimal burden and privacy concern. 

This award reflects NSF's statutory mission and has been deemed worthy of support through evaluation using the Foundation's intellectual merit and broader impacts review criteria.


### Development
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
### Activity Orietned Obfuscation
![image](/img/eager/activity-oriented-obfuscation.png)


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
HeatSight is (A) a chest-worn wearable system consisting of five independent low-power thermal sensing arrays allowing a thermal Omni capture (180◦) of the wearer’s surroundings, including (B) the thermal radiation emitted from objects around the wearer, and (C) the human thermal signature emitted from the wearer’s body over time. These thermal human-object interaction signatures can be used for human activity detection. 
![image](/img/eager/hs1f.png) 
## SmartAct: A wearable smartcam
Diagram of the methodological framework; (a) We use a low-powered RGB-T wearable device to collect data. (b) The device stays in low power mode by only obtaining thermal images from a thermal sensor (c) The activation algorithm selects a candidate from the live stream of thermal images. (d) The candidates are further processed with a high-power task, either saving RGB correspondence to the disk or running a feeding gesture model that takes binary image motion as input. 
![image](/img/eager/sa1.png) 
SmartAct Hardware/Firmware: https://github.com/HAbitsLab/BSN22Trigger  

### Publications

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
