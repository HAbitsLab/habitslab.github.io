---
title: "ActiveSense: A Novel Active Learning Framework for Human Activity Recognition"
date: 2014-05-06T15:09:31-06:00
draft: false
authors: [{name: "Farzad Shahabi", profile: "/profiles/farzad"}, {name: "Yang Gao", profile: ""}, {name: "Nabil Alshurafa", profile: ""}]
has_github_link: false
github_link: "https://github.com/"

---

### Abstract
One of the persistent challenges in building machine-learned models for mobile health applications of fine-grained activity is the generation of accurate annotations with well-defined start/end time labels. Large amounts of unlabeled data exist, and annotation is often labor-intensive and costly. Moreover, it is not clear whether labeling all the data is even necessary to building the most effective machine-learned model. Active learning approaches harness model uncertainty by selecting the most informative samples, reducing the time and effort in labeling unnecessary segments of the data. Model uncertainty, however, is strongly linked to classifier performance, introducing bias in sample selection and impacting model generalizability. In this paper, we propose and study the effects of a new active learning framework on the Necksense dataset which harnesses intrinsic uncertainty as well as model uncertainty by utilizing the Area Under the Margin (AUM) statistic, leading to a significant reduction in the number of samples needed to annotate. We also show that we are able to design a more generalizable model training on 0.15% (n=192 samples) of the data compared to the original model trained on 85% (n=104,681 samples) of the data.




