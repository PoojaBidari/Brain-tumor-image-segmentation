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
├── data/brisc2025/ # Dataset
├── results/ # All outputs
│ ├── plot1_mean_comparison.png
│ ├── plot2_best_worst.png
│ ├── plot3_boxplot.png
│ ├── plot4_scatter.png
│ ├── plot5_line_charts.png
│ ├── plot6_gap_analysis.png
│ ├── full_results_with_iou.csv
│ └── methodology_diagram.png
├── main_segmentation.py # Main execution script
└── requirements.txt # Dependencies


## 🚀 How to Run

```bash
# Clone repository
git clone https://github.com/yourusername/brain-tumor-segmentation.git

# Install dependencies
pip install -r requirements.txt

# Run segmentation
python main_segmentation.py
