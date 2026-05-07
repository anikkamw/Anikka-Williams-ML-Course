# MangeVision: AI-Driven Canine Mange Classifier
**Anikka Williams** - Lead Developer & Domain Expert (Veterinary Technician Background)

## Problem & Solution

### The Problem
Traditional diagnosis of canine mange requires invasive skin scrapings, which can be stressful for the animal and time-consuming for clinical staff. There is a need for a rapid, non-invasive triage tool to assist in early detection.

### Impact
This tool reduces diagnostic wait times and improves animal welfare by providing a non-contact preliminary screening method.

## Technical Details

### Approach
* **Task:** Multi-class Image Classification
* **Model:** Vision Transformer (ViT)
* **Framework:** PyTorch
* **Key Libraries:** `torch`, `torchvision`, `timm`, `matplotlib`, and `seaborn`

### Performance Metrics (ViT Evaluation)
* **Demodicosis:** 0.96 (F1-Score)
* **Healthy:** 0.88 (F1-Score)
* **Scabies:** 0.93 (F1-Score)
* **Overall Accuracy:** 92%

### System Architecture
1. **Data Acquisition:** Automated retrieval of canine and human skin disease datasets via `kagglehub`.
2. **Preprocessing:** Images resized to **224x224** for ViT compatibility; normalization applied to align with ImageNet standards.
3. **Model Construction:** Implementation of a custom **ViT class** featuring Patch Embedding, Transformer Encoder blocks (Multi-head Attention), and a MLP Head for 3-class classification.
4. **Optimization:** Trained for 20 epochs using **AdamW** with a `ReduceLROnPlateau` scheduler to refine the learning rate during plateaus.

### Dataset
* **Source:** Combined datasets from [Kaggle](https://www.kaggle.com/datasets/youssefmohmmed/dogs-skin-diseases-image-dataset) and [Roboflow](https://roboflow.com).
* **Total Images:** 1,350 images across 3 classes.
* **Classes:** Demodicosis, Scabies, Healthy.
* **Split:** 80% Training | 10% Validation | 10% Testing
