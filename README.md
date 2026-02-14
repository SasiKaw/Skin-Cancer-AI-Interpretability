# 🩺 Skin Cancer Classification with AI Safety & Interpretability

This project is my first step into exploring **AI Safety** and **Interpretability**. It demonstrates a deep learning approach to skin cancer classification, moving beyond a simple "Black Box" model to visualize the reasoning behind the AI's medical diagnosis.

---

## 🌟 Project Overview
In healthcare, high accuracy is not enough. An AI must be **interpretable** so that clinicians can verify its decisions. This project uses a Convolutional Neural Network (CNN) to classify 7 types of skin lesions and employs **Saliency Maps** to show exactly which parts of the image the model focuses on.

## 🛠️ Key Technical Features
- **Framework:** Developed using **PyTorch**.
- **Dataset:** Trained on the **MedMNIST (DermaMNIST)** dataset, a collection of dermatoscopic images.
- **Architecture:** Custom CNN designed for medical image feature extraction.
- **AI Safety Integration:**
    - **Saliency Maps:** Visualizes pixel importance to prevent "Shortcut Learning" (e.g., checking if the model focuses on rulers or skin hair instead of the actual lesion).
    - **Distributional Shift Awareness:** Understanding biases regarding skin tones in the training data and how it affects real-world applications.

## 🔍 Interpretability in Action
Through Saliency Maps, we can audit the model. If the "heat map" aligns with the lesion's borders, we have higher confidence. If it highlights background noise or rulers, we identify a risk of the model learning the wrong correlations.

## 🚀 What I Learned
- Building and training a Convolutional Neural Network (CNN) from scratch using PyTorch.
- Opening the "Black Box" of AI using Saliency Maps to understand the model's focus.
- The practical importance of AI Safety concepts like Outer Alignment and Distributional Shifts.

## 💻 How to Run
1. Open the provided `.ipynb` file in **Google Colab**.
2. Ensure the Runtime is set to **GPU (T4)**.
3. Run the cells sequentially to train the model and generate your own Saliency Maps.

---
*Developed as a learning project focused on AI Safety and Deep Learning.*
