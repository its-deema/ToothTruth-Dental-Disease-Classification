##  Implemented Models

We implemented and fine-tuned the following convolutional neural network (CNN) architectures:

### 1. **EfficientNetV2**
- ✅ **Main pipeline**
- Includes **data preprocessing**, **augmentation**, **cropping**, and **training scripts**.
- Used as the starting point of the project.
- Achieved **97.04% accuracy**.
- Key augmentations:
  - Random flipping
  - Rotation
  - Brightness variation
  - Gaussian noise
- Pretrained on ImageNet, then fine-tuned on the dental dataset.


### 2. **InceptionV3**
- Implemented for its multi-scale feature extraction.
- Achieved the **highest classification accuracy (97.51%)** among all models.

### 3. **DenseNet121**
- Strong performance on medical images due to dense connections and feature reuse.
- Fine-tuned using the same preprocessed dataset.
- Achieved **96.70% accuracy**.
- Benefited from transfer learning and consistent convergence.

### 4. **ResNet50**
- Known for its residual learning capabilities.
- Applied with the same training pipeline (excluding preprocessing).
- Achieved solid performance with good generalization.

### 5. **VGG16**
- Simple and reliable baseline architecture.
- Used for comparison; slower training and larger model size.
- Still achieved competitive accuracy with proper fine-tuning.


---

## ⚙️ Preprocessing & Augmentation

> ⚠️ All preprocessing and augmentation scripts are included in the **EfficientNetV2 implementation code** (`efficientnetv2_model`), since this model was developed first and served as the base pipeline.

- **Augmentation Techniques**:
  - Random horizontal/vertical flipping
  - Rotation between -20 to +20 degrees
  - Brightness/contrast adjustments
  - Gaussian noise injection

---

## 🔬 Evaluation Metrics

For each model, we used the following metrics to compare performance:

- Accuracy  
- Precision  
- Recall  
- F1-Score  
- AUC-ROC  
- mAP (mean average precision)
