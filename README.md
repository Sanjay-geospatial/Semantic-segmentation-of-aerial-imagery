# Semantic Segmentation of Aerial Imagery using U-Net with ResNet Backbone
![Semantic Segmentation Banner](https://www.google.com/search?q=lulc+esri&sca_esv=126bc4ae6ee860b7&rlz=1C1GCEU_enIN1103IN1111&udm=2&biw=1366&bih=641&sxsrf=AE3TifMP4f5sb_XALg2HYG1cGDoEqSFltQ%3A1749618171267&ei=-w1JaPmFEMa3vr0PkreawQI&oq=lulc+&gs_lp=EgNpbWciBWx1bGMgKgIIBTIHECMYJxjJAjIHECMYJxjJAjIKEAAYgAQYQxiKBTIFEAAYgAQyChAAGIAEGEMYigUyBRAAGIAEMgUQABiABDIKEAAYgAQYQxiKBTIFEAAYgAQyBRAAGIAESIEbUKkBWKkBcAF4AJABAJgBtwGgAbcBqgEDMC4xuAEByAEA-AEBmAICoALCAcICBhAAGAcYHpgDAIgGAZIHAzEuMaAHlweyBwMwLjG4B7wBwgcDMi0yyAcK&sclient=img#imgrc=m4TnRdB4aFbF7M&imgdii=mYLhYz40pmjhvM)

This project focuses on semantic segmentation of aerial imagery into six land cover classes using a U-Net architecture with a ResNet encoder backbone.

## 🛰️ Project Overview

Land use land cover (LULC) classification plays a vital role in environmental monitoring, urban planning, and resource management. In this project, we employ deep learning techniques to segment aerial images into the following six classes:

1. Water  
2. Building
3. Vegetation  
4. Land 
5. Road 
6. Unlabelled

We use a U-Net model with a ResNet-based encoder to achieve high accuracy and spatial precision.

## 🧠 Model Architecture

- **Base Architecture**: U-Net  
- **Encoder Backbone**: ResNet-34 (pretrained on ImageNet)  
- **Loss Function**: Categorical Cross-Entropy 
- **Metrics**: IoU (Intersection over Union) and Accuracy

## 📁 Dataset

- **Source**: https://www.kaggle.com/datasets/humansintheloop/semantic-segmentation-of-aerial-imagery
- **Format**: RGB aerial imagery with corresponding pixel-wise masks
- **Classes**: 6 (as listed above)

## 🛠️ Setup

### Requirements

```bash
python>=3.8
tensorflow>=2.x
numpy
rioxarray
matplotlib
scikit-learn
opencv-python
segmentation_models
