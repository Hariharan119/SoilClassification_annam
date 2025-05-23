🌱 SoilClassification_annam
============================

Soil classification using SEResNeXt50 with cross-validation, ensembling, and advanced augmentations for the ANNAM.AI Hackathon.

This repository contains a robust soil classification pipeline built with PyTorch and torchvision. The pipeline employs 3-Fold Cross-Validation, MixUp and ColorJitter augmentations, and model ensembling to achieve state-of-the-art classification performance. The entire solution is contained within a single notebook as per the hackathon submission guidelines.

──────────────────────────────
📁 Project Structure
──────────────────────────────

SoilClassification_annam/
│
├── notebooks/
│   └── soil-classification.ipynb    # Complete training, validation, and inference pipeline
├── requirements.txt                 # List of required Python packages
└── README.md                       # Project overview, setup, and usage instructions
──────────────────────────────
🚀 Features
──────────────────────────────

✅ SEResNeXt50_32x4d pretrained on ImageNet  
✅ 3-Fold Cross-Validation for robust evaluation  
✅ MixUp and ColorJitter augmentations for improved generalization  
✅ Model ensembling of the best fold models for higher accuracy  
✅ Weighted loss with class weights to handle class imbalance  
✅ Optional Test Time Augmentation (TTA)  
✅ Per-class F1 score visualization and confusion matrix analysis  
✅ Submission-ready prediction format  

──────────────────────────────
🛠 Setup Instructions
──────────────────────────────

1️⃣ Clone the repository

    git clone https://github.com/your-username/SoilClassification_annam.git
    cd SoilClassification_annam

2️⃣ Install dependencies

    pip install -r requirements.txt

Contents of requirements.txt (all pre-installed on Google Colab):

    torch>=2.0.0
    torchvision>=0.15.0
    albumentations>=1.3.0
    opencv-python-headless
    scikit-learn
    matplotlib
    pandas
    numpy
    tqdm

──────────────────────────────
📈 Metrics & Performance
──────────────────────────────

- Training performed using 3-Fold Cross-Validation (Fold 1, 2, and 3)  
- Model: SEResNeXt50_32x4d with weighted CrossEntropyLoss  
- Evaluation metrics include:  
    • Per-fold Macro F1 Score  
    • Confusion Matrix visualization  
    • Per-class F1 score visualization  

──────────────────────────────
🙏 Thank You!
──────────────────────────────

Thank you for checking out this project!
