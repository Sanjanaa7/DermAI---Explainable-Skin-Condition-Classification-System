# DermAI – Skin Condition Classification System

## Overview

DermAI is an AI-based skin condition classification system that uses **Deep Learning and Transfer Learning** to identify common skin conditions from images.

The system uses **MobileNetV2** for image classification and **Grad-CAM** to provide visual explanations for the model's prediction.

## Features

* Skin condition classification
* MobileNetV2 transfer learning
* AI confidence score
* Prediction probability chart
* Top 3 predictions
* Grad-CAM explainability
* Original and processed image comparison
* Simple Gradio web interface

## Skin Conditions

The model classifies images into six categories:

* Acne
* Dark Spots
* Eczema
* Normal Skin
* Rosacea
* Wrinkles

## Dataset

The dataset used in this project is the **Multi-Class Skin Condition Image Dataset (MSC-6)** from **Kaggle**.

**Dataset:** Multi-Class Skin Condition Image Dataset (MSC-6)
**Source:** Kaggle
**Dataset ID:** `harishnivasagam/multi-class-skin-condition-image-dataset-msc-6`

The dataset is downloaded automatically in Google Colab using `kagglehub`.

## Technologies Used

* Python
* TensorFlow
* Keras
* MobileNetV2
* Grad-CAM
* Gradio
* NumPy
* Matplotlib
* Pillow
* KaggleHub

## Model

The project uses **MobileNetV2**, a pre-trained convolutional neural network with ImageNet weights.

The MobileNetV2 base model is used for feature extraction, followed by:

**Global Average Pooling → Dropout → Dense Layer → Dropout → Softmax**

## Explainability

**Grad-CAM (Gradient-weighted Class Activation Mapping)** is used to highlight the important regions of the input image that influenced the model's prediction.

## How to Run

1. Open the notebook in Google Colab.
2. Install the required libraries.
3. Run the notebook cells.
4. The dataset will be downloaded automatically from Kaggle.
5. Train the model.
6. Launch the Gradio interface.
7. Upload a skin image to get the prediction.

## Project Structure

```text
DermAI/
│
├── DermAI_Skin_Condition_Classification.ipynb
├── README.md
└── models/
    └── dermAI_model.keras
```

## Note

DermAI is developed as an **academic project** for educational and research purposes. It is not intended to replace professional medical diagnosis.
