# Semantic Segmentation of Aerial Imagery using U-Net with ResNet Backbone
![Image](https://github.com/user-attachments/assets/4940fe5d-30ee-46ea-a1d0-acc2e877ce8a)

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

## 📊 Results
- **Accuracy**: 0.87
- **Jacard coefficient**: 0.75
- **MeanIOU**: 0.61


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
