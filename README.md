# 🦠 Malaria Cell Detection using CNN

This project uses a **Convolutional Neural Network (CNN)** built with **TensorFlow/Keras** to automatically detect malaria-infected cells from microscopic blood smear images. It is designed to aid early diagnosis and support healthcare professionals in resource-constrained environments.

---

## 📌 Overview

Malaria is a life-threatening disease caused by parasites transmitted to people through the bites of infected mosquitoes. Manual diagnosis of malaria from blood smear images is time-consuming and requires expertise. This project applies deep learning techniques to automate and improve the accuracy of malaria detection.

---

## 📂 Dataset

The dataset used is the **Malaria Cell Images Dataset** from the [NIH](https://lhncbc.nlm.nih.gov/publication/pub9932), which consists of:

- `Parasitized/` – Images of infected cells.
- `Uninfected/` – Images of healthy cells.

Each image is a colored microscopic image (typically 134x134 pixels).

---

## 🧠 Model Architecture

A custom CNN was built with the following layers:

- **Convolutional Layers**: For extracting spatial features.
- **MaxPooling Layers**: For downsampling.
- **Dropout Layers**: For regularization to prevent overfitting.
- **Dense Layers**: Fully connected layers for classification.

The model was compiled with:

- `optimizer='adam'`
- `loss='binary_crossentropy'`
- `metrics=['accuracy']`

---

## 📈 Performance

After training for several epochs with image augmentation, the model achieved:

- ✅ **High accuracy (~95%)**
- ✅ **Low overfitting due to Dropout & Augmentation**
- ✅ **Good generalization on test set**

**Evaluation Metrics**:

- Accuracy
- Precision
- Recall
- Confusion Matrix

---
