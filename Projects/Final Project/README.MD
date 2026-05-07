# Marine Debris Detection: AI-Driven Coastal & Underwater Waste Classification
**Anikka Williams** - Lead Developer

## Problem & Solution

### The Problem
Marine plastic pollution is a global environmental crisis, yet identifying and categorizing debris in diverse aquatic environments (coastal vs. underwater) is manually intensive. Effective cleanup requires automated systems that can detect waste despite low visibility or complex backgrounds.

### The Solution
This project implements a **Convolutional Neural Network (CNN)** optimized for multi-domain marine environments. By leveraging the **TACO (Trash Annotations in Context)** dataset, the system differentiates between debris found in coastal and underwater settings.

## Technical Details

### Approach
* **Task:** Image Classification (Coastal vs. Underwater Debris)
* **Model:** Custom 4-Layer Convolutional Neural Network (CNN)
* **Framework:** TensorFlow / Keras
* **Key Libraries:** `tensorflow`, `pandas`, `pycocotools`, `matplotlib`, and `seaborn`

### Performance Metrics (Code-Verified)
* **Training Accuracy:** 100% (Achieved by Epoch 2)
* **Validation Split:** 20%
* **Loss Function:** Binary Crossentropy
* **Optimization:** Adam Optimizer

### System Architecture
1. **Data Engineering:** Implemented a **Deep Search Mapper** to recursively walk through directory structures and auto-label 6,630 images based on folder metadata.
2. **Preprocessing:** Utilized `ImageDataGenerator` for real-time rescaling (1/255) and extreme augmentation (90° rotation, brightness shifts) to prevent overfitting.
3. **Model Construction:** - **Input:** 150x150x3 images.
    - **Layers:** Conv2D (32 filters), MaxPooling, and high-dropout layers (0.5) to ensure the model focuses on the debris rather than the water/sand backgrounds.
4. **Evaluation:** Visualized "Plastic Waste Distribution" across 28 super-categories using Seaborn.

### Dataset
* **Source:** [TACO Trash Dataset](https://www.kaggle.com/datasets/kneroma/tacotrashdataset)
* **Total Images:** 6,630 images.
    - **Underwater Environment:** 5,130 images.
    - **Coastal Environment:** 1,500 images.
* **Focus:** 22 specific plastic-related categories including Bottles, Cups, and Bags.
