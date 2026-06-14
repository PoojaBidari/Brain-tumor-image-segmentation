# 🧠 Brain Tumor Detection: Otsu vs Watershed Segmentation

## 📌 Overview

This project implements and compares two classical image segmentation methods—**Otsu Thresholding** and **Watershed Segmentation**—for brain tumor detection in MRI images. The BRISC 2025 dataset containing expert-annotated brain tumor masks is used for evaluation. Performance is measured using **Dice Coefficient** and **Intersection over Union (IoU)** metrics.

## 🎯 Key Findings

| Method | Mean Dice | Mean IoU | Best Dice |
| :--- | :--- | :--- | :--- |
| Otsu Thresholding | 0.1019 | 0.0549 | 0.2856 |
| Watershed Segmentation | **0.1082** | **0.0592** | **0.3084** |

- ✅ **Watershed outperforms Otsu on 80% of test images**
- ✅ 6.2% higher mean Dice score
- ✅ 7.8% higher mean IoU score

## 📊 Dataset

- **Name:** BRISC 2025 (Brain MRI Image Segmentation Challenge)
- **Images:** 3,933 training / 1,000 testing
- **Modality:** T1-weighted contrast-enhanced MRI
- **Tumor Types:** Glioma, Meningioma, Pituitary tumor

## ⚙️ Methods Implemented

1. **Otsu Thresholding** - Automatic threshold selection using histogram analysis
2. **Watershed Segmentation** - Marker-based region growing with distance transform

## 📈 Evaluation Metrics

- Dice Similarity Coefficient
- Intersection over Union (IoU / Jaccard Index)

## 📁 Project Structure
