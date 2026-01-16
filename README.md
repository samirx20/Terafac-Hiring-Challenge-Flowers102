# Computer Vision Hiring Challenge: Flowers-102

**Candidate:** Samrendra Maurya  
**Affiliation:** GGSIPU, EDC  
**Date:** January 16, 2026

## 📂 Project Structure
This repository contains the complete solution for the Multi-Level Assessment. The code is consolidated into a single Jupyter Notebook for reproducibility.

├── Flowers102_Solution.ipynb  # Contains code for Levels 1, 2, 3, 4, and 5
├── models/
│   └── level_5_production.pt  # Final Quantized MobileNetV2 (~9MB)
├── results/
│   ├── level_1_training.png
│   ├── level_2_comparison.png
│   ├── level_3_heatmap.png
│   └── level_4_accuracy.png
└── requirements.txt

## 🚀 Solution Summary

### Level 1: Baseline (ResNet50)
- Implemented Transfer Learning with ResNet50.
- Custom 80/10/10 split on Flowers-102 dataset.
- **Accuracy:** ~95%

### Level 2: Data Augmentation
- Added RandomRotation, Flip, and ColorJitter.
- Demonstrated improved robustness against variations.

### Level 3: Explainability (Grad-CAM)
- Visualized class activation maps to verify feature focus (petals/textures).

### Level 4: Ensemble Learning
- Combined **ResNet50** (Teacher) and **MobileNetV2** (Student).
- **Final Ensemble Accuracy:** 95.61% (Surpassing 93% threshold).

### Level 5: Production Optimization
- Pivoted to **MobileNetV2** for edge deployment.
- Applied **Dynamic Quantization**.
- **Inference Speed:** 29.77 ms (Target <100ms).
- **Compression:** 90.2% reduction (8.8MB).

## 🛠️ How to Run
1. Open `Flowers102_Solution.ipynb` in Google Colab or Jupyter Lab.
2. Install requirements: `pip install -r requirements.txt`.
3. Run all cells sequentially.
