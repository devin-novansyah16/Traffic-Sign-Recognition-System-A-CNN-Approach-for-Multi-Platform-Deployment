 #Klasifikasi GTSRB


# Traffic Sign Recognition System: A CNN Approach for Multi-Platform Deployment

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?style=for-the-badge&logo=Keras&logoColor=white)

An end-to-end Deep Learning project focused on classifying traffic signs using a Convolutional Neural Network (CNN). This project achieves high accuracy on the GTSRB dataset and is exported into multiple formats for web, mobile, and server-side deployment.

## 🚀 Project Overview
This project aims to solve the challenge of automated traffic sign recognition, a crucial component for Autonomous Vehicles and Advanced Driver Assistance Systems (ADAS).

### Key Features:
*   **High Performance**: Achieved over **95% accuracy** on both training and testing sets.
*   **Large Dataset**: Trained on over **39,000 images** from the German Traffic Sign Recognition Benchmark (GTSRB).
*   **Multi-Platform Ready**: Includes exported models in `SavedModel`, `TF-Lite`, and `TFJS` formats.
*   **Real-world Preprocessing**: Handles images with non-uniform resolutions and implements data augmentation.

## 📊 Dataset
The project utilizes the **German Traffic Sign Recognition Benchmark (GTSRB)**, which consists of 43 classes of traffic signs.
*   **Total Images**: 39,209 (Train) + 12,630 (Test)
*   **Classes**: 43 distinct categories (Speed limits, warnings, yield, etc.)
*   **Source**: [Kaggle - GTSRB Dataset](https://www.kaggle.com/meowmeowmeowmeowmeow/gtsrb-german-traffic-sign)

## 🏗️ Model Architecture
The model is built using the Keras `Sequential` API with the following layers:
*   **Convolutional Layers**: 3 layers of `Conv2D` with ReLU activation.
*   **Normalization**: `BatchNormalization` for faster convergence.
*   **Pooling**: `MaxPooling2D` for spatial downsampling.
*   **Regularization**: `Dropout` (0.5) to prevent overfitting.
*   **Output**: `Dense` layer with Softmax activation for 43-class classification.

## 📈 Performance
The training process was optimized using a custom **Callback** to stop training once target accuracy was met.

| Metric | Accuracy |
| :--- | :--- |
| **Training Accuracy** | > 95% |
| **Validation Accuracy** | > 95% |
| **Test Accuracy** | > 95% |

*(Note: You can insert your accuracy/loss plots here by adding: `![Plots](./path_to_your_plot_image.png)`)*

## 📂 Directory Structure
```text
.
│   ├── tfjs_model/          # Model for Web (TensorFlow.js)
│   ├── tflite/              # Model for Mobile (TF-Lite)
│   │   ├── model.tflite
│   │   └── label.txt
│   └── saved_model/         # Standard TensorFlow format
├── notebook.ipynb           # Main implementation notebook
├── requirements.txt         # List of dependencies
└── README.md

#Developed by Devin Novansyah
├── notebook.ipynb           # Main implementation notebook
├── requirements.txt         # List of dependencies
└── README.md
