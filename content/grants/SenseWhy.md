---
title: "SenseWhy: Overeating in Obesity Through the Lens of Passive Sensing"
date: 2017-12-05T15:09:31-06:00
draft: false
logo_image: "/img/nh.png"
start_year: 2018
end_year: 2023
funding_amount: "$850,000"
primary_investigator: {name: "Nabil Alshurafa", 
                       title: "Ph.D., Director of HABits Lab", 
                       description: "Assistant Professor of Preventive Medicine and of Computer Science, Northwestern University", 
                       img: "/img/pro-big.png" ,
                       }
coinvestigators: [{name: "Bonnie Spring", title: "Director, Institute for Public Health and Medicine (IPHAM)", description: "Professor of Preventive Medicine (Behavioral Medicine), Northwestern University", img: "/img/bonnie_spring.png"}, 
                {name: "Tammy Stump", title: "Research Associate, Huntsman Cancer Institute, University of Utah", description: "desction description description", img: "/img/p-2.png"}]
---

### 1. Introduction

Obesity, caused primarily by overeating relative to need, is a preventable chronic disease that affects 42.4% of US adults, increasing their risk of cardiovascular disease. Obesity also exacts staggering costs on the US healthcare system. 

A challenge in treating obesity is that, unlike substance abuse, the treatment goal cannot be simply to extinguish the ingestive behavior, as eating is necessary to sustain life. Obesity treatment would benefit greatly from an ability to discriminate between and intervene upon the specific problematic eating behavioral phenotypes that foster obesity. 

In the SenseWhy project, our approach is to identify eating patterns via wearable sensor data that characterize episodes of excess calorie intake. This approach may facilitate detection of known (e.g., emotional eating, impulsive eating in response to cues, hedonic eating) and novel eating phenotypes that have different treatment implications. A wearable system designed to detect overeating objectively and passively and then intervene in a manner that adapts to an individual’s problematic overeating profile
paves the way toward personalized behavioral medicine interventions.

### The wearable system

We first develop 3 wearables, each designed to capture different features of eating behavior.

#### Chest-worn Infrared Activity-Oriented Device (IR-AOD)

The IRAOD is a chest-worn camera and thermal imager designed to visually capture the occurrence and context of eating episodes, providing ground truth against which other sensor metrics can be confirmed.

##### Components and enclosure:

![IR-AOD Schematica](/img/eager/sw1.png)

##### Data streams

The IR-AOD is positioned on the center of the chest and points upward, orienting both sensors towards the face and mouth. RGB and thermal frames are shown below:

![IR-AOD Preview](/img/eager/swcrop.png)

#### NeckSense necklace device

![NeckSense System](/img/eager/ns-fig1.png)

[NeckSense](https://dl.acm.org/doi/pdf/10.1145/3397313) is a necklace with several onboard sensors, including proximity, ambient light, and IMU. 

The proximity sensor enables chew detection by capturing jaw movement. The ambient light sensor complements the proximity sensor and gives additional information about the eating environment. The IMU's gyroscope signal encodes the lean angle of the wearer, namely leaning forward (generally associated with eating) and leaning backwards (generally associated with drinking).

Recording these signals in tandem allows us to characterize masticulation during eating in much greater detail than in typically possible, illuminating new features of eating behavior that may prove useful in our effort to define behavioral phenotypes.


#### Smartwatch

Using a custom application on a Fossil Sport smartwatch (AndroidOS), we record IMU and PPG data from the dominant wrist. Wrist IMU captures hand-to-mouth gestures (integral to eating) and also provides a proxy to physical activity/energy expenditure, the caloric counterbalance to eating/energy intake. Wrist PPG—a continuous measure of capillary blood oxygenation—serves as a proxy to heart rate and blood pressure, indicative of stress as well as general cardiovascular health.

##### Wearable System Overview

Pictured below is a high-level example of how the SenseWhy wearable system characterizes an eating episode through the use of 3 multi-sensing devices worn concurrently and continuously:

![sys overview](/img/eager/sysov.png)

### EMA, self-reporting, and 24-hr diet recall

In addition to passive sensing, we developed FoodTrck, a mobile application that participants use to record meals by photographing them and inputting affective and contextual information associated with the meal, both before and after eating occurs. 

We also utilize 24-hr diet recalls in which a trained dietitian contacts participants by telephone daily to ascertain via interview the food types and portions consumed on the prior day. 

#### FoodTrck

A FoodTrck entry consists of 3 survey pages, each with its own unique prompts and collection instruments relevant to a given meal:

![FoodTrck overview](/img/eager/ft-ov.png)

#### Diet recall

In our proposed study, dietitans are able to supplement the standard 24-hr recall technique by viewing the meals recorded via FoodTrck. This allows dietitians to begin some of their inquiries into a participants diet from objective data rather than pure memory recall reporting.

### SenseWhy Study

We recruited 60 participants with BMI > 30 (obese) to record their eating intake with the SenseWhy wearable sensor, EMA, and diet recall system for 14 days. Sensors were worn during all waking hours, EMAs completed with every meal/snack, and diet recalls were completed daily.

For a detailed explanation of our methodology, see our [study design paper](https://journals.sagepub.com/doi/10.1177/20552076231158314), published in Digital Health.

#### Results
Coming soon...