# Pneumonia-Detection-Deep-Learning
## Introduction

Automated pneumonia detection from chest X-ray images using deep learning has shown promising potential. However, a major challenge in developing reliable classification systems is handling invalid or out-of-distribution inputs, such as non-X-ray images, which may produce misleading predictions.

To address this input-handling challenge, this project presents a two-stage prototype. In the first stage, MobileNetV2 is used as a feature extractor, followed by a One-Class Support Vector Machine (One-Class SVM) to identify outlier inputs based on the feature distribution learned from chest X-ray training images. In the second stage, an SVM classifier classifies the accepted feature vectors into two categories: **NORMAL** and **PNEUMONIA**.

In addition to the primary detection system, a separate comparative experiment evaluates five pretrained CNN architectures under a common training configuration to investigate their classification performance.

These two experiments serve distinct purposes. The two-stage system represents the primary application-oriented prototype, focusing on input validation and pneumonia classification, whereas the CNN comparison provides an independent model-evaluation study. Therefore, their experimental results are reported separately and are not combined or treated as interchangeable.

This project is intended as a research prototype and should not be considered a substitute for professional medical diagnosis.
