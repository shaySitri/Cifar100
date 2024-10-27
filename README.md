# CIFAR-100 Image Classification 🖼️🔍
[![Jupyter Notebook](https://img.shields.io/badge/Notebook-cifar100_ass1.ipynb-orange?logo=jupyter)](https://github.com/shaySitri/Cifar100/blob/main/cifar100_ass1.ipynb)

This repository contains a Jupyter Notebook focused on image classification techniques for the CIFAR-100 dataset, exploring model performance and improvements.

---

## 📄 Project Overview
The **CIFAR-100** dataset comprises 60,000 images across 100 balanced classes, each containing 500 training and 100 test samples. Each image is 32x32 pixels with three color channels. The project applies deep learning models, aiming to improve accuracy by addressing dataset challenges and complex class distinctions.

---

## 📊 Data Insights
- **Dataset Size**: 60,000 images (500 training, 100 test per class).
- **Augmentation**: Applied techniques like translations and grayscale to diversify the dataset.
- **Challenging Classes**: Some classes had similar visual features, making classification difficult.

---

## 🧩 Model Development
### Initial Model - CNN
The initial model used a simple CNN architecture with:
- **Convolutional Layers**: 4 layers with 3x3 kernels, ReLU activation, and max-pooling.
- **Batch Size**: 64
- **Epochs**: 11
- **Learning Rate**: 2e-4
- **Optimizer**: Adam

#### Training Results:
- **Training Loss**: Averaged around 1.2
- **Training Accuracy**: Approximately 52%
- **Validation Loss**: 2.7
- **Validation Accuracy**: Around 36%

### Enhanced Model - Improvements
To address underfitting, several enhancements were tested:
1. **Data Augmentation**: Random cropping and resizing improved generalization.
2. **Increased Network Complexity**: Added layers and complexity to better capture data patterns.
3. **Additional Epochs**: Extended training to allow more weight updates, leading to better convergence.

#### Enhanced Model Results:
- **Validation Accuracy**: 64.4%
- **Validation Loss**: 1.25
- **Test Accuracy**: 42.5%
- **Test Loss**: 2.16

### Benchmark Models
The report also compares benchmark models:
- **ResNet**: Achieved around 65% test accuracy.
- **DenseNet**: Showed 55% test accuracy.
- **VGG16**: Faced limitations, achieving only minimal accuracy due to computational constraints.

---

## 🔍 Key Findings
- **Underfitting**: The initial model lacked complexity, resulting in low accuracy.
- **Augmentation Benefits**: Image transformations helped the model generalize better.
- **Improved Architecture**: Increasing the model depth and complexity reduced loss and increased accuracy.
