# AI-Powered Lung Disease Classification Using Neural Networks and CT-Scan Images.

This project focuses on developing a deep learning model to classify lung CT scan images into four categories: **Adenocarcinoma**, **Large Cell Carcinoma**, **Squamous Cell Carcinoma**, and **Normal Cell**. The goal is to assist radiologists and medical professionals in early and accurate detection of lung cancer types using automated image analysis.

---

## 🧠 Overview

Lung cancer is one of the leading causes of cancer-related deaths worldwide. Early and accurate classification of lung cancer types is crucial for effective treatment. This project uses convolutional neural networks (CNNs) to analyze grayscale CT scan images and classify them into one of the following:

- Adenocarcinoma  
- Large Cell Carcinoma  
- Squamous Cell Carcinoma  
- Normal (Healthy)  

---

## 📂 Dataset

The dataset is organized into three folders:

- `train/` (70%)  
- `valid/` (10%)  
- `test/` (20%)  

Each folder contains four subfolders corresponding to the classes above. All images are in grayscale format.

---

## 🛠️ Technologies Used

- Python  
- TensorFlow & Keras  
- NumPy, Pandas  
- Matplotlib, Seaborn  
- DenseNet121 (Transfer Learning)  
- Google Colab (for model training and experimentation)  

---

## 🚀 Model Architecture

The following models were tested:

- **ResNet50** (achieved ~53.65% accuracy)  
- **DenseNet121** (achieved ~90% accuracy ✅)  

The final model uses DenseNet121 pretrained on ImageNet, with fine-tuning for the specific classification task.

---

## 🔄 Preprocessing

- Conversion of grayscale images to RGB (for compatibility with pre-trained models)  
- Image normalization  
- Image resizing to 224x224 pixels  
- Data augmentation using `ImageDataGenerator`  

---

## 📌 Key Features

- Multi-class classification (4 lung conditions)  
- Transfer learning for higher accuracy and faster convergence  
- Real-time performance monitoring with training plots  
- Easily extendable for other medical imaging tasks  

---

## 📊 Results

- **Final Model:** DenseNet121  
- **Accuracy:** ~90%  
- **Loss:** Minimal (validation loss < training loss)  
- Confusion matrix and classification report included in the notebook  

