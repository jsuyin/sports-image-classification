# 🏀 Sports Image Classification (ConvNeXt)

**Authors:** Justin Mundell, Ronan M., Thu N.

---

## Overview
Built a deep learning model to classify sports gameplay images into 10 categories using a dataset of 100K+ images from 175 video games. The model handles significant variation in visual styles, including retro, modern, and photorealistic graphics.

---

## Approach
- **Model:** ConvNeXt-Tiny (pre-trained on ImageNet, fine-tuned)  
- **Input:** Images resized to 224×224  
- **Data Split:** Train (68%) / Val (8%) / Test (24%), grouped by game to prevent leakage  
- **Augmentation:** Random crops, flips, rotations, and color jitter  

---

## Results
- **Validation Accuracy:** ~80–83%  
- Training loss decreased steadily, while validation loss increased over time, indicating overfitting  

---

## Key Takeaways
- Transfer learning was effective for large-scale image classification  
- Splitting data by **game (not image)** was critical to avoid leakage  
- Model performance was limited by generalization across diverse visual styles  

---

## Tech Stack
- Python  
- PyTorch  
- NumPy / pandas  

---

## Next Steps
- Improve generalization with regularization and tuning  
- Explore larger architectures or ensemble methods  
