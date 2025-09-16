---
title: "Deep Fake Videos"
excerpt_separator: "<!--more-->"
subtitle: "Using Nueral Networks to detect deep fake videos"
date: 2025-09-15
permalink: /posts/deepfake/
read_time: true
categories:
  - Blog
tags:
  - Publications
---

### The Problem: The Rise of Deepfakes 

Deepfake technology is a growing threat to determining authentic media from fake, AI-generated content. With the rise of powerful AI models, it's becoming increasingly difficult to tell what is real from what is fake. While many deepfakes are created for entertainment, they can also be used to manipulate groups of people, which can be dangerous.

---

### Our Approach: Facial Landmark Analysis 

Our research explored a novel technique that focuses on the differences in facial movements to find abnormalities in a video. We hypothesized that artificially generated videos would fail to capture fully realistic movements of facial features, like the eyes and mouth, giving rise to subtle inconsistencies that our model could detect.

To test this, we used a dataset of real and deepfake videos. Our methodology involved:

* **Data Extraction**: We extracted 67 specific facial landmark points from thousands of video frames.
* **Data Preprocessing**: We preprocessed the data to create a uniform dataset. This included removing rows with negative values, which appeared when a facial feature was not found. We also resized all video frames to a uniform $256 \times 256$ pixel size and standardized all videos to a uniform length of 720 frames. Additionally, we engineered new features by calculating the first, second, and third derivatives of the frame movements.
* **Model Training**: We trained and tested three different models on the preprocessed data: an **Artificial Neural Network (ANN)**, a **Convolutional Neural Network (CNN)**, and a **Recurrent Neural Network (RNN)**.

---

### Our Results: RNN Shines 

We found that the **RNN model was the best performer**. It was tied with the ANN model in accuracy, but it required less computational power than the other models.

* **RNN Model**: This model is well-suited for this task because it predicts data points based on previously observed patterns in sequential data. The RNN model achieved an accuracy of approximately **96%**.
* **ANN Model**: The ANN model acted as a baseline for comparison and did much better than expected, achieving an accuracy of **95.65%**. However, it was more computationally expensive than the RNN model.
* **CNN Model**: The CNN model used an image-like data structure to train on. It achieved an accuracy of approximately **91%**. This model was found to be computationally heavy, and the preprocessing for it took many steps to accomplish.

The findings of the paper emphasize the importance of facial feature analysis in addressing the growing threat of deepfake misuse and provide a foundation for future advancements in deepfake detection technology.

---

### Links

* [**Full Paper**](https://arxiv.org/abs/2507.18815)
* [**GitHub Repository**](https://github.com/BenCarter44/ANN440)
