# 🫁 Lung Cancer Detection Using CNN (VGG16)

This project focuses on detecting lung cancer from **Chest CT-Scan images** using a **Convolutional Neural Network (CNN)** built on top of the **VGG16** pre-trained model.  
The goal is to automatically classify CT images into different cancer types or identify normal tissue, helping medical professionals with faster and more accurate diagnoses.

The main aim of this project is to develop an AI model capable of classifying lung CT-Scan images into one of the following four categories:
- **Normal**
- **Adenocarcinoma**
- **Large Cell Carcinoma**
- **Squamous Cell Carcinoma**


## Model and Methodology
- **Base Model:** VGG16 (pre-trained on ImageNet)
- **Framework:** TensorFlow 
- **Optimizer:** Adam
- **Loss Function:** Categorical Crossentropy
- **Metrics:** Accuracy, Precision, Recall, F1-Score
- **Epochs:** 100

During training, model accuracy improved from **38.16% (Epoch 1)** to **93.01% (Epoch 100)** which shows strong learning and stability over time.

## Dataset
- **Source:** [Chest CT-Scan Images Dataset (Kaggle)](https://www.kaggle.com/datasets/mohamedhanyyy/chest-ctscan-images/) 
- **Classes:**
  - Adenocarcinoma  
  - Large Cell Carcinoma  
  - Squamous Cell Carcinoma  
  - Normal  



## Evaluation and Results

### 🧾 Classification Report
| Class | Precision | Recall | F1-Score | Support |
|:--|:--|:--|:--|:--|
| Normal | 0.82 | 0.86 | 0.84 | 120 |
| Squamous Cell Carcinoma | 0.86 | 0.75 | 0.80 | 51 |
| Large Cell Carcinoma | 1.00 | 0.94 | 0.97 | 54 |
| Adenocarcinoma | 0.83 | 0.88 | 0.85 | 90 |

**Accuracy:** 0.86  
**Macro Avg F1-Score:** 0.87  
**Weighted Avg F1-Score:** 0.86  



### 📉 Confusion Matrix
![Confusion Matrix](results/confusion_matrix.png)




