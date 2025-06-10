# 🦴 Bone Fracture Detection Using Deep Learning

This project demonstrates a **binary classification** model to detect **bone fractures in X-ray images** using **transfer learning** with the VGG16 model. It includes data preprocessing, augmentation, fine-tuning, model training, evaluation, and real-time prediction on a single image.

---

## 📁 Project File

- `DL_PROJECT_BONE.ipynb`:  
  Jupyter Notebook containing all steps — from **data loading** to **model evaluation** and **prediction**.

---

## 🗂 Dataset Used

- **Source**: Kaggle [Bone Fracture X-ray Dataset] 
- **Type**: X-ray images of bones  
- **Classes**:
  - `Fractured`  
  - `Non_Fractured`

### 📌 Directory Structure

datasets/
└── FracAtlas/
└── images/
├── Fractured/
└── Non_Fractured/


---

## 🧠 Model Summary

- **Base Model**: VGG16 (pre-trained on ImageNet)  
- **Techniques Used**:
  - Transfer Learning
  - Fine-tuning (unfreezing top layers)
  - Data Augmentation (rotation, zoom, width/height shift, horizontal flip)
- **Training Utilities**:
  - `EarlyStopping`
  - `ModelCheckpoint`
- **Loss Function**: Binary Cross-Entropy  
- **Optimizer**: Adam

---

## 📈 Model Performance

- **Final Accuracy**: ~83%
- **Evaluation Metrics**:
  - Accuracy and Loss plots
  - Confusion Matrix
  - Classification Report

---

## 🖼️ Single Image Prediction

The notebook includes a function to perform **real-time prediction** for a new X-ray image:

predict_single_image("path_to_image.jpg")

## ⚙️ Setup

Install the required packages using:

```python
pip install numpy pandas matplotlib seaborn scikit-learn tensorflow pillow

