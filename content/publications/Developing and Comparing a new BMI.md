---
title: "Developing and comparing a new BMI inclusive energy expenditure algorithm on wrist-worn wearables"
date: 2025-06-19T15:09:31-06:00
draft: false
authors: [{name: "Boyang Wei", profile: "/profiles/boyang"}, {name: "Chris Romano", profile: "profiles/chris"}, {name: "Mahdi Pedram", profile: "/profiles/mahdi"}, {name: "Bonnie Nolan", profile: "/profiles/bonnie"}, {name: "Whitney A Morelli"}, {name: "Nabil Alshurafa", profile: "/profiles/nabil"}]
has_github_link: true
github_link: "https://www.nature.com/articles/s41598-025-99963-0"

---

### Abstract

Estimating energy expenditure (EE) in real-world settings is crucial for studying human behavior and energy balance. Despite advances in wrist-worn inertial measurement units (IMU), actigraphy remains the most accepted measure for estimating EE, despite known Errors in accuracy, particularly in people with obesity. We developed an algorithm estimating EE from commercial smartwatch sensor data, and validated it against actigraphy-based energy estimates in people with obesity. In an in-lab study, 27 participants wore a Fossil Sport smartwatch and ActiGraph wGT3X+ while performing activities of varying intensities. Another 25 participants wore the smartwatch for 2 days in a free-living study. We built a machine learning model to estimate metabolic equivalent of task (MET) values/minute using smartwatch accelerometer and gyroscope data. Analysis included 2,189 minutes of in-lab and 14,045 minutes of free-living data. Compared to the metabolic cart, our model achieved lower root mean square error (0.28–0.32) across various sliding windows. In the free-living study, our algorithm’s estimates fell within +-1.96 SD of the best actigraphy-based estimates for 95.03% of minutes. Our proposed method accurately estimated METs compared to 11 algorithms primarily validated in non-obese populations, suggesting that commercial wrist-worn devices can provide more inclusive and reliable EE measures using our algorithm.