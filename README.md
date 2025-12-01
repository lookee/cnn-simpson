# Advanced ConvNet50 for Detecting Simpsons Characters  
**Transfer Learning, Data Augmentation & Fine-Tuning**

RESNET50 • CNN • TRANSFER LEARNING • DATA AUGMENTATION • KAGGLE DATASET

![cnn-simpson](https://camo.githubusercontent.com/da086dccdf1de6356f20d8957b2e4b9bd9bfb72f9f7447f80e48577c3776643a/68747470733a2f2f7777772e6c756361616d6f72652e636f6d2f77702d636f6e74656e742f75706c6f6164732f323032342f31312f73696d70736f6e2d636e6e2d6c6974746c652e706e67)

**Author:** Luca Amore  
📧 luca.amore at gmail.com  
🌍 https://www.lucaamore.com

![Python](https://img.shields.io/badge/Python-3.10-blue.svg)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange.svg)
![Keras](https://img.shields.io/badge/Keras-API-red.svg)
![ResNet50](https://img.shields.io/badge/Model-ResNet50-green.svg)
![Transfer Learning](https://img.shields.io/badge/Transfer%20Learning-Enabled-brightgreen.svg)
![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)
![Kaggle](https://img.shields.io/badge/Kaggle-Notebook-20beff.svg?style=flat&logo=kaggle)
[![Kaggle Dataset](https://img.shields.io/badge/Kaggle-Dataset-20beff.svg?style=flat&logo=kaggle)](https://www.kaggle.com/datasets/alexattia/the-simpsons-characters-dataset)

---

## 🎯 Project Overview

This project explores **character recognition** from *The Simpsons* TV show using a modern **Convolutional Neural Network** approach.  
Starting from a **pre-trained ResNet50** backbone (trained on ImageNet), a **transfer learning** pipeline was designed to classify **42+ iconic characters** from the show.

Perfect for demonstrating:
- Feature extraction via deep residual networks  
- Robust data augmentation to prevent overfitting  
- Fine-tuning on domain-specific datasets  
- Real-world deployment potential on entertainment/comics datasets  

---

## 🧠 Model Architecture

✔ **Base Model**: ResNet50 (frozen convolutional layers initially)  
✔ **Classifier Head**:
- Global Average Pooling
- Dense + ReLU
- Dropout regularization
- Final Dense Softmax output layer

✔ **Training Strategies**
- Initial training with frozen backbone
- Fine-tuning last residual blocks
- Early stopping and learning-rate scheduling

---

## 🧪 Dataset

👉 Kaggle: **The Simpsons Characters Dataset**  
A curated set including thousands of labeled images of the show’s characters.

Dataset contains:
- High intra-class variability (expressions, clothing, scenes)
- Real-world occlusions and backgrounds
- Uneven sample distribution across characters

🔗 https://www.kaggle.com/datasets/alexattia/the-simpsons-characters-dataset

Images are processed through:
- Random rotation & flipping
- Label-preserving shifts and zooms
- Normalization to ImageNet mean/std

---

## 📊 Performance

Key Metrics:
- Accuracy
- Validation loss trend
- Confusion matrix for character confusion patterns

> Best-performing configuration after fine-tuning showed strong separation even between visually similar characters.

# Results

![simpson-simulation-1](simpson-simulation-1.png)
![simpson-simulation-2](simpson-simulation-2.jpg)

---

## 🛠️ Tech Stack

| Component | Version |
|----------|---------|
| Python | 3.10 |
| TensorFlow | 2.x |
| Keras | Latest API |
| GPU Acceleration | Optional (highly recommended) |

Training was executed through Kaggle GPUs.

---

## ▶️ Try It Yourself

Access the runnable training notebook on Kaggle:

🔗 https://www.kaggle.com/code/lucaamore/convnet50-simpson-character-identifer

---

## 📝 Related Blog Article

Detailed walkthrough and project explanation available here:

🔗 https://www.lucaamore.com/?p=2301

---

## 📜 License

Distributed under the **GPL v3** license.  
Feel free to fork, contribute, and extend this project!

---

> _D’oh! Let’s see if neural networks can tell Homer apart from Ned Flanders..._

