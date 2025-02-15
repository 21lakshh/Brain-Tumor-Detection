# Brain Tumor Detection using EfficientNetB1

## Overview
This project aims to classify brain MRI images into four categories:
- **Glioma**
- **Meningioma**
- **No Tumor**
- **Pituitary**

We utilize deep learning with a pre-trained EfficientNetB1 model to achieve high accuracy in detecting brain tumors from MRI images.

## Dataset
- All images are stored in a **DataFrame** for efficient handling.
- Visualized the class distribution using a **pie chart**.
- Displayed sample images from each class.
- Cropped the outer section of all images to focus on the tumor region.

## Data Preprocessing
- Applied **ImageDataGenerator** for data augmentation on **training** and **validation** sets.
- **No augmentation** was applied to the **test set**.

## Model Architecture
- Used **EfficientNetB1** as the backbone for feature extraction.
- Fine-tuned the model to optimize classification performance.

## Model Performance
- **Training Accuracy:** 99.44%
- **Validation Accuracy:** 98.34%
- **Test Accuracy:** 98.55%

### Confusion Matrix & Metrics
- Constructed a **confusion matrix** to analyze model predictions.
- Evaluated key metrics:
  - **Precision:** 0.99
  - **Recall:** 0.99
  - **F1-score:** 0.99

## Explainability with Grad-CAM
- Implemented **Grad-CAM** to highlight tumor regions in MRI images.
- Visualized the most influential areas for each classification.

## Results
Below are some Grad-CAM visualizations highlighting the tumor areas in the MRI scans:

![Grad-CAM Example](/GradCAM/image1.png)

## Future Improvements
- Experiment with other architectures (e.g., Vision Transformers, ResNet variants).
- Deploy the model as a web application.
- Enhance dataset quality with more preprocessing techniques.
