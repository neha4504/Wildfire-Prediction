# Wildfire Prediction Using CNN & Transfer Learning

## Overview
This project implements a wildfire image classification pipeline using a **proprietary satellite image dataset** provided by a major tech company for academic purposes. The dataset contains 92,800 images organized into **wildfire** and **non-wildfire** categories, split into train, validation, and test sets.  
The goal: **Accurately classify satellite images to detect wildfire presence** using both a custom CNN and a pretrained ResNet50 model.

---

## Project Workflow
1. **Data Cleaning**  
   - Verified dataset integrity and removed corrupt images.  
   - Checked class distribution to identify imbalances.  

2. **Data Preprocessing**  
   - Resized images for model compatibility (224×224 for ResNet50).  
   - Normalized pixel values to [0, 1].  
   - Applied data augmentation (rotation, flipping, zoom) to improve generalization.  

3. **Modeling Approaches**  
   - **Custom CNN**: Designed and trained from scratch.  
   - **Transfer Learning**: Fine-tuned pretrained ResNet50 for improved accuracy.  

4. **Evaluation Metrics**  
   - Accuracy, Precision, Recall, F1-score  
   - Confusion Matrix  
   - ROC-AUC Curve  

---

## Results
- **ResNet50 with Transfer Learning** outperformed the custom CNN in both accuracy and generalization.
- Data augmentation significantly reduced overfitting in both models.

---

## Key Technologies
- **Python**  
- **TensorFlow / Keras**  
- **Matplotlib & Seaborn** for visualization  
- **Scikit-learn** for metrics  

---

## Dataset
Due to licensing restrictions, the dataset **cannot be shared publicly**.  
If you wish to reproduce the results:  
```
dataset/
  train/
    wildfire/
    nowildfire/
  valid/
    wildfire/
    nowildfire/
  test/
    wildfire/
    nowildfire/
```
- Images should be satellite photos resized to 224×224 pixels.

---

## Acknowledgement
Dataset provided by a **major tech company** for academic research purposes.

