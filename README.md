# 🥔 Plant Disease Detection using Machine Learning

> Detect potato leaf diseases (Early Blight, Late Blight, Healthy) using image classification models like CNN, Random Forest, and SVM.

![Demo GIF](demo.gif) <!-- Optional: add a GIF or image -->

## 📌 Overview

Potato crops are vulnerable to diseases like Early Blight and Late Blight, leading to severe yield loss. This project uses machine learning—particularly **Convolutional Neural Networks (CNNs)**—to detect diseases from leaf images with up to **99% accuracy**.

## 🎯 Objectives

- Classify potato leaves into **Early Blight**, **Late Blight**, or **Healthy**.
- Build a **high-accuracy deep learning model**.
- Handle **class imbalance** using **augmentation** and **SMOTE**.
- Create a pipeline for **real-time disease detection**.

## 🧠 Techniques Used

- **Traditional ML**: Support Vector Machine (SVM), Random Forest with feature extraction
- **Deep Learning**: Custom CNN using TensorFlow & Keras
- **Data Preprocessing**: Resizing, Normalization
- **Data Augmentation**: Rotation, Flip, Zoom
- **Class Balancing**: SMOTE

## 📁 Dataset

- Source: [Kaggle](https://www.kaggle.com/datasets/rhythm007/potato-disease-data)
- Total Images: **5403**
  - Early Blight: 2303
  - Late Blight: 2132
  - Healthy: 968
- Image Size: Resized to **224×224** or **256×256**

## 🛠️ Model Comparison

| Model           | Accuracy | Strengths                           |
|----------------|----------|-------------------------------------|
| **SVM**         | 79%      | Works with handcrafted features     |
| **Random Forest** | 94%      | Balanced and interpretable          |
| **CNN**         | 99%      | Best performer, deep feature learning|

## 🧪 CNN Evaluation

- **Overall Accuracy**: 99%
- **Early Blight**: Precision: 0.99, Recall: 1.00
- **Late Blight**: Precision: 1.00, Recall: 0.99
- **Healthy**: Precision: 0.99, Recall: 1.00

> 🟢 The CNN model demonstrated **near-perfect classification** performance across all categories.

## 📈 Results

- **Confusion Matrix**: Very few misclassifications, mostly in Late Blight.
- **Test Predictions**: Model achieved 99.21% to 100% confidence.

## 🚧 Challenges Faced

- **SVM**: Underfitting due to shallow features.
- **Random Forest**: Initial overfitting resolved via tuning & class weights.
- **Class Imbalance**: Healthy class underrepresented, mitigated using SMOTE and augmentation.

## 🔍 Future Scope

- Add explainable AI (e.g., Grad-CAM)
- Expand dataset for better generalization
- Deploy on edge devices (e.g., mobile phones)
- Real-time disease detection app with feedback loop

## 🧑‍💻 Contributors

- [Ayushi Mitra](https://github.com/ayushimitra)
- Indranil Chatterjee
- Hirak Naskar
- Agnik Sarkar  
👨‍🏫 Under the guidance of **Mr. Sourendranath Mallick**

## 📚 References

- Agarwal et al., "ToLeD: Tomato Leaf Disease Detection", ScienceDirect, 2020  
- Mamun et al., "Potato Disease Detection Using ML", IEEE, 2021  
- Albattah et al., "Plant Disease Classification with DL", Springer Nature, 2021  
- And more...

---

## 📽️ Demo Video

[![Watch the video]([https://www.youtube.com/watch?v=YOUR_VIDEO_ID](https://drive.google.com/drive/u/0/folders/1hNwD3HEYje43ijC5-pqcWt5zLskN8T0W))


---

## 📂 How to Run

```bash
git clone https://github.com/yourusername/plant-disease-detection.git
cd plant-disease-detection

# Install dependencies
pip install -r requirements.txt

# Run the model training or inference
python train_cnn.py
