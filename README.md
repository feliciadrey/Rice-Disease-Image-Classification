# Sehatin Padi - Rice Leaf Disease Classification
This repository contains a Jupyter notebook (`Rice_Disease_Img_Classification.ipynb`) that implements a CNN-based model for automatic detection of rice leaf diseases using transfer learning. Multiple ImageNet-pretrained backbones were compared (EfficientNetB0, ResNet50, InceptionV3, MobileNetV2, DenseNet121).

---
## Dataset & Quick stats
- Dataset: **3,829** images across **6** classes  
  `['Bacterial Leaf Blight', 'Brown Spot', 'Healthy Rice Leaf', 'Leaf Blast', 'Leaf scald', 'Sheath Blight']`
- Train/Val/Test split used in the notebook: **~70% train (2,681)** and remaining 30% split equally for validation and test (~574 each).
- Image size: **224 × 224**
- Batch size: **32**
- Optimizer: **Adam** (learning rate **1e-4**)
- Loss: **sparse_categorical_crossentropy**

---

## Models evaluated & results (test set)
| Model | Test Accuracy | Test Loss |
|---|---:|---:|
| EfficientNet-B0 | **0.9458** | 0.1915 |
| ResNet50 | 0.9108 | 0.2485 |
| InceptionV3 | 0.6329 | 1.2074 |
| MobileNetV2 | 0.7045 | 0.8206 |
| DenseNet121 | 0.8112 | 0.5382 |

> EfficientNet-B0 showed the best performance in these experiments.

---

## Acknowledgments
This work was completed as part of a team project for a Statistic Competition.  
Special thanks to my teammates for their contributions in dataset preparation, experiments, and analysis.


