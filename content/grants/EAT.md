---
title: "EAT: A Reliable Eating Assessment Technology for Free-living Individuals"
date: 2021-07-27T15:09:31-06:00
draft: false
logo_image: "/img/nh.png"
start_year: 2021
end_year: 2026
funding_amount: "$3,868,150"
primary_investigator: 
    {name: "Nabil Alshurafa", 
     title: "Director of HABits Lab", 
     img: "/img/pro-big.png" ,
    profile: "/profiles/nabil"}

mpis: {}

coinvestigators: [
     {name: "Angela Fidler Pfammatter", 
      title: "Associate Professor of Public Health, University of Tennessee Knoxville",
      img: "/img/Angela.jpg",
     profile: "https://www.feinberg.northwestern.edu/faculty-profiles/az/profile.html?xid=34056"},

     {name: "Annie W. Lin",
     title: "Assistant Professor of Nutrition Informatics, Hormel Institute, University of Minnesota",
     img: "/img/Annie.jpg",
     profile: "https://hi.umn.edu/research/faculty/annie-w-lin-phd"},

    {name: "Josiah Hester",
    title: "Associate Professor of Interactive Computing and Computer Science College of Computing, Georgia Institute of Technology",
    img: "/img/josiah.png",
    profile: "https://josiahhester.com/cv/"},

    {name: "Jacob M. Schauer",
    title: "Assistant Professor of Preventive Medicine, Northwestern University",
    img: "/img/jake.jpg",
    profile: "https://www.jmschauer.com/"}
    ]
studentinvestigators: [
    {name: "Blaine Rothrock",
    img: "/img/im-8.png",
    profile: "https://blainerothrock.com/"}, 

    {name: "Soroush Shahi",
    img: "/img/im-7.png",
    profile: "/profiles/soroush"},
    
    {name: "Boyang Wei",
    img: "/img/im-1.png",
    profile: "/profiles/boyang"}
    ]
mentors: {}
---

### Project Overview

Monitoring an individual’s eating behavior will provide detailed understanding of the causal relationship between the eating activity and conditions such as problematic eating and obesity. Manual self-reports are often erroneous and biased. The availability of wearable video cameras makes it possible to objectively capture the eating activity. However, manually observing video frames to obtain the objective measure of eating is burdensome. Additionally, wearable video cameras pose privacy concerns in real-world settings. To overcome these challenges, we are developing an automated eating detection system to monitor real-time eating behavior via a privacy-conscious wearable device that individuals will wear. We will confirm eating activities in real time. Such automatic and privacy-conscious real-time eating detection will allow us to advance our understanding of the eating activity, laying the foundation for future interventions to change problematic eating behaviors.

To this end, first we will develop an activity detection algorithm that will allow detecting the eating activity using data from an IR sensor array and RGB images. Next, we will test various obfuscation methods in a cross-over trial and select the best obfuscation method based on the greatest participant acceptability. We will then deploy the eating detection algorithm with the best obfuscation approach on a novel wearable camera that has an infrared sensor array. We will use this camera to test the possibility of detecting eating in a real-world setting. To validate our algorithm, we will ask people to confirm or refute predicted eating and non-eating moments. We will compare the performance of this algorithm against both real-time user response and 24-hour dietary recall to objectively evaluate the algorithm’s performance. Our proposed system will improve current research practices of evaluating dietary intake and pave the way for personalized interventions for behavioral medicine.

### Aims

##### Aim 1: Compare accuracy of the eating detection algorithm that incorporates each obfuscation method in controlled environments 
Participants performed eating and non-eating activities in a controlled environment for an entire day. We developed an automated eating detection algorithm using data from each obfuscation method to determine accuracy of eating detection across methods.

###### The study team after setting up for one of the Aim 1 study sessions!
![Photo of study team during Aim 1 study](/img/eatstudypic.jpeg "The study team during an Aim 1 study session!")

##### Aim 2: Measure acceptability/feasibility of the EAT real-time obfuscation methods
A cohort of 72 participants will wear the camera using three obfuscation and one non-obfuscation methods (7 consecutive days for each method) during the entire wake period, separated by a 7-day washout. We will assess subjective acceptability and conduct a fully powered experiment by objectively measuring total wear time of each version.

##### Aim 3: Test and validate algorithm to assess accuracy of detecting eating in free-living people
New participants (n=60, 50% with obesity, 50% female) will wear EAT with the best obfuscation method identified by considering results from Aim 1 and 2 for 7-days while self-reporting eating moments and context using a quick tap app implemented on a smartwatch. We will determine how many eating episodes are detected by an EAT informed algorithm and the number of gestures required to capture an eating moment in a real-world setting. 



