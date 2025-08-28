---
title: "Multi-Modal Hand-to-Mouth Gesture Recognition in Activity-Oriented RGB-Thermal Footage"
date: 2025-04-11T15:09:31-06:00
draft: false
authors: [{name: "Glenn Fernandes", profile: "/profiles/glenn"}, {name: "Meixi Lu"}, {name: "Farzad Shahabi", profile: "profiles/farzad"}, {name: "Jiayi Zheng", profile: "profiles/jiayi"}, {name: "Aggelos Katsaggelos"}, {name: "Nabil Alshurafa", profile: "/profiles/nabil"}]
has_github_link: true
github_link: "https://ojs.aaai.org/index.php/AAAI/article/view/35254"

---

### Abstract

Health-risk behaviors such as overeating and smoking have a profound impact on public health, making their monitoring and mitigation critical. Wearable RGB-Thermal cameras are being employed to monitor these behaviors by capturing hand-to-mouth (HTM) gestures, which are central to them. However, detection models relying on single modalities—either RGB or thermal—often struggle to accurately distinguish these confounding gestures due to inherent sensor limitations, such as sensitivity to lighting conditions or thermal occlusions. We present a family of fusion models that integrate RGB and thermal video data using early-, decision- , and a novel mid-fusion architecture, RGB-Thermal Fusion Video Network (RTFVNet), designed to enhance the recognition of HTM gestures associated with eating and smoking. Our evaluation shows that while decision fusion achieves the highest F1-score of 88% (0.44 TFLOPs), RTFVNet offers an optimal balance between performance (85%) and complexity (0.37 TFLOPs) for gesture classification of eating, smoking, and non-gesture activities.