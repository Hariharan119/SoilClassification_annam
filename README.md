# 🌱 SoilClassification_annam

**Soil classification using SEResNeXt50 with cross-validation, ensembling, and advanced augmentations for the ANNAM.AI Hackathon.**

This repository presents a robust soil classification pipeline developed using PyTorch and `torchvision`. The model utilizes advanced training techniques such as MixUp, ColorJitter, 3-Fold Cross-Validation, and model ensembling to ensure high accuracy and generalization.

All functionalities are implemented within a single notebook, adhering to the hackathon submission requirements.

---

## 📁 Project Structure

•notebooks/

soil-classification.ipynb: Complete training, validation, and inference pipeline

•requirements.txt

Lists all required Python dependencies

•README.md

Overview of the project, setup instructions, and usage guide

---

## 🚀 Features

- ✅ SEResNeXt50_32x4d pretrained on ImageNet
- ✅ 3-Fold Cross-Validation for robust model evaluation
- ✅ MixUp and ColorJitter augmentations for better generalization
- ✅ Model ensembling of the best models from each fold
- ✅ Class-weighted loss function to handle class imbalance
- ✅ Optional Test Time Augmentation (TTA)
- ✅ Detailed evaluation with per-class F1 score and confusion matrix
- ✅ Submission-ready output format

---

## 🛠 Setup Instructions

1️⃣ Clone the repository

git clone https://github.com/your-username/SoilClassification_annam.git  
cd SoilClassification_annam

2️⃣ Install dependencies

pip install -r requirements.txt

requirements.txt contents:

torch>=2.0.0  
torchvision>=0.15.0  
albumentations>=1.3.0  
opencv-python-headless  
scikit-learn  
matplotlib  
pandas  
numpy  
tqdm

---

## 📈 Metrics & Performance

- Model: SEResNeXt50_32x4d with Weighted CrossEntropyLoss
- Cross-Validation: 3 Folds (Fold 1, 2, and 3)
- Evaluation Metrics:
  - Per-fold Macro F1 Score
  - Confusion Matrix visualization
  - Per-class F1 Score breakdown

---


