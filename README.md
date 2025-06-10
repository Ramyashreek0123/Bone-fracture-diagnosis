🦴 Bone Fracture Detection Using Deep Learning
This project demonstrates a binary classification model that detects bone fractures in X-ray images using transfer learning with VGG16. It includes data preprocessing, augmentation, fine-tuning, training, evaluation, and a real-time single image prediction function.

📁 File
DL_PROJECT_BONE.ipynb: Jupyter Notebook containing all steps from data loading to model evaluation and prediction.

🗂 Dataset Used
Source: Kaggle
Type: Bone X-ray images with two classes:
Fractured
Non_Fractured

📌 Directory Structure: datasets/ └── FracAtlas/ └── images/ ├── Fractured/ └── Non_Fractured/

🧠 Model Summary
Base Model: VGG16 (ImageNet weights)
Techniques:
Transfer Learning
Fine-Tuning (unfreeze top layers)
Data Augmentation: rotation, zoom, shift, flip
EarlyStopping and ModelCheckpoint
Loss Function: Binary Cross-Entropy
Optimizer: Adam

📈 Performance
Final Accuracy: ~83%
Evaluation: Accuracy & Loss plots, Confusion Matrix, Classification Report
Supports real-time prediction for a single image

🖼️ Single Image Prediction 
The notebook includes a function to predict whether a new X-ray image is fractured or non-fractured using the trained model. Use the final cell for single image prediction: predict_single_image("path_to_image.jpg")

⚙️ Setup Install required packages:
pip install numpy pandas matplotlib seaborn scikit-learn tensorflow pillow
