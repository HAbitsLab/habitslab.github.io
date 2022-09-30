---
title: "Impacts of Image Obfuscation on Fine-grained Activity Recognition in Egocentric Video"
date: 2022-09-29T15:09:31-06:00
draft: false
authors: [{name: "Soroush Shahi", profile: "/profiles/soroush"}, {name: "Rawan Alharbi", profile: ""}, {name: "Yang Gao", profile: ""}, {name: "Sougata Sen", profile: ""}, {name: "Aggelos K Katsaggelos", profile: ""}, {name: "Josiah Hester", profile: ""}, {name: "Nabil Alshurafa", profile: ""}]
has_github_link: true
github_link: "https://github.com/HAbitsLab/HOBM"

---

### Abstract

Automated detection and validation of fine-grained human activities from egocentric vision has gained increased attention in recent years due to the rich information afforded by RGB images. However, it is not easy to discern how much rich information is necessary to detect the activity of interest reliably. Localization of hands and objects in the image has proven helpful to distinguishing between hand-related fine-grained activities. This paper describes the design of a hand-object-based mask obfuscation method (HOBM) and assesses its effect on automated recognition of fine-grained human activities. HOBM masks all pixels other than the hand and object in-hand, improving the protection of personal user information (PUI). We test a deep learning model trained with and without obfuscation using a public egocentric activity dataset with 86 class labels and achieve almost similar classification accuracies (2% decrease with obfuscation). Our findings show that it is possible to protect PUI at smaller image utility costs (loss of accuracy).


![Example image](/img/imapcts_of_image_obfuscation.png)





