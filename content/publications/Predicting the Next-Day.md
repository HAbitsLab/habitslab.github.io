---
title: "Predicting the Next-Day Perceived and Physiological Stress of Pregnant Women by Using Machine Learning and Explainability: Algorithm Development and Validation"
date: 2022-08-02T15:09:31-06:00
draft: false
authors: [{name: "Ada Ng", profile: "/profiles/firstname_lastname"}，
			name: "Boyang Wei", profile: "/profiles/firstname_lastname"},
			{name: "Jayalakshmi Jain", profile: "/profiles/firstname_lastname"}，
			{name: "Erin A Ward", profile: "/profiles/firstname_lastname"}，
			{name: "S Darius Tandon", profile: "/profiles/firstname_lastname"}，
			{name: "Judith T Moskowitz", profile: "/profiles/firstname_lastname"}，
			{name: "Sheila Krogh-Jespersen", profile: "/profiles/firstname_lastname"}，
			{name: "Lauren S Wakschlag ", profile: "/profiles/firstname_lastname"}，
			{name: "Nabil Alshurafa", profile: "/profiles/firstname_lastname"}]
has_github_link: false
github_link: "https://github.com/"

---

### 1. Background

Cognitive behavioral therapy–based interventions are effective in reducing prenatal stress, which can have severe adverse health effects on mothers and newborns if unaddressed. Predicting next-day physiological or perceived stress can help to inform and enable pre-emptive interventions for a likely physiologically and perceptibly stressful day. Machine learning models are useful tools that can be developed to predict next-day physiological and perceived stress by using data collected from the previous day. Such models can improve our understanding of the specific factors that predict physiological and perceived stress and allow researchers to develop systems that collect selected features for assessment in clinical trials to minimize the burden of data collection.

### 2. Objective

The aim of this study was to build and evaluate a machine-learned model that predicts next-day physiological and perceived stress by using sensor-based, ecological momentary assessment (EMA)–based, and intervention-based features and to explain the prediction results.

### 3. Methods

We enrolled pregnant women into a prospective proof-of-concept study and collected electrocardiography, EMA, and cognitive behavioral therapy intervention data over 12 weeks. We used the data to train and evaluate 6 machine learning models to predict next-day physiological and perceived stress. After selecting the best performing model, Shapley Additive Explanations were used to identify the feature importance and explainability of each feature.

### 4. Results

A total of 16 pregnant women enrolled in the study. Overall, 4157.18 hours of data were collected, and participants answered 2838 EMAs. After applying feature selection, 8 and 10 features were found to positively predict next-day physiological and perceived stress, respectively. A random forest classifier performed the best in predicting next-day physiological stress (F1 score of 0.84) and next-day perceived stress (F1 score of 0.74) by using all features. Although any subset of sensor-based, EMA-based, or intervention-based features could reliably predict next-day physiological stress, EMA-based features were necessary to predict next-day perceived stress. The analysis of explainability metrics showed that the prolonged duration of physiological stress was highly predictive of next-day physiological stress and that physiological stress and perceived stress were temporally divergent.

### 5. Conclusions

In this study, we were able to build interpretable machine learning models to predict next-day physiological and perceived stress, and we identified unique features that were highly predictive of next-day stress that can help to reduce the burden of data collection.




