# Rice Leaf Disease Detection — Basic CNN and Transfer Learning Comparison

![Python](https://img.shields.io/badge/Python-3.x-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Keras-orange)
![MobileNetV2](https://img.shields.io/badge/Model-MobileNetV2-purple)
![Accuracy](https://img.shields.io/badge/Val%20Accuracy-91%25-green)

> PRCP-1001 Capstone Project — Datamites Certified Data Science Program

---

## Overview

This project detects rice leaf diseases using image classification.
Two approaches are compared:

| Approach | Model | Val Accuracy |
|---|---|---|
| Basic | Sequential CNN from scratch | ~48% |
| Advanced | MobileNetV2 Transfer Learning | **91%** |

---

## Dataset

**3 classes — 40 images each (119 total):**
- Bacterial leaf blight
- Brown spot
- Leaf smut

> **Disclaimer:** The dataset is not included in this repository.
> The download link is provided in `PRCP-1001-RiceLeaf.docx` (included in repo).
> Direct download link:
> ```
> https://d3ilbtxij3aepc.cloudfront.net/projects/CDS-Capstone-Projects/PRCP-1001-RiceLeaf.zip
> ```

---

## Setup Instructions

1. Download the dataset from the link above
2. Extract the zip file
3. Upload to your Google Drive
4. Create a folder called `Data` inside `MyDrive`
5. Place the 3 class folders inside `Data/`
6. Open notebook in Google Colab
7. Run the `drive.mount()` cell first before executing anything else

---

## Notebooks

| Notebook | Description |
|---|---|
| `PRCP_1001_RiceLeaf_Basic.ipynb` | Sequential CNN from scratch — EDA, preprocessing, model training, evaluation |
| `PRCP_1001_RiceLeaf_Advanced.ipynb` | MobileNetV2 Transfer Learning — ImageDataGenerator, EarlyStopping, ModelCheckpoint, ReduceLROnPlateau |

---

## Model Comparison

### Basic CNN
- Built from scratch using Keras Sequential API
- Random weight initialization — learns only from 119 images
- Result: overfitting, ~48% val accuracy

### MobileNetV2 Transfer Learning (Feature Extraction)
- Pretrained on ImageNet (1.2M images, 1000 classes)
- Base model frozen — used purely as feature extractor
- Only custom top layers trained (164K / 2.4M params)
- Augmentation via ImageDataGenerator
- Callbacks: EarlyStopping + ModelCheckpoint + ReduceLROnPlateau
- Result: **91% val accuracy in just 8 epochs**

---

## Tech Stack

`Python` `TensorFlow` `Keras` `MobileNetV2` `NumPy` `Matplotlib` `Seaborn` `scikit-learn` `Google Colab`

---

## Results
