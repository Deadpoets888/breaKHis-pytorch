# breaKHis-pytorch
This project implements a deep learning pipeline to classify breast cancer histopathological images into subtypes using the BreaKHis dataset. It leverages EfficientNet-B0, transfer learning, and patient-level data splitting to ensure robust evaluation.
⚠️ Note: This project is currently under active development.

📁 Dataset
Source: https://www.kaggle.com/datasets/ambarish/breakhis/data

Classes:
Benign: adenosis, fibroadenoma, phyllodes tumor, tubular adenoma
Malignant: ductal carcinoma, lobular carcinoma, mucinous carcinoma, papillary carcinoma

Magnification Levels: 40X, 100X, 200X, 400X

📌 Key Features
✅ Metadata extraction with subtype, patient ID, and magnification
✅ Patient-wise train/val/test split to prevent data leakage
✅ Data augmentation applied only to training set
✅ Image preprocessing: Resize → ToTensor → Normalize (ImageNet stats)
✅ EfficientNet-B0 model finetuned on histopathology images

📊 Current Progress
 Metadata extraction
 Dataset splitting (stratified by patient ID)
 Custom PyTorch Dataset class
 Data augmentation for training
