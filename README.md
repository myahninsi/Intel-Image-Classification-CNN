# Intel Image Classification - CNN

## Overview
This project implements a **Convolutional Neural Network (CNN)** for **multi-class image classification** using the **Intel Image Classification dataset**. The model classifies images into six categories: **buildings, forest, glacier, mountain, sea, and street**.

## Dataset
- **Source**: [Intel Image Classification - Kaggle](https://www.kaggle.com/datasets/puneet6060/intel-image-classification)
- **Size**: 25,000 images
- **Classes**: 6
- **Preprocessing**: Images are resized, normalized, and augmented.

## Approach
### 1️⃣ Data Loading and Preparation
- Load dataset using `ImageDataGenerator`.
- Resize images to `(150,150,3)`.
- Normalize pixel values to `[0,1]`.
- Split into training (80%) and testing (20%).

### 2️⃣ Model Building
- **Conv Layers**: 2+ convolution layers with ReLU activation.
- **Pooling**: MaxPooling for downsampling.
- **Dropout**: Prevents overfitting.
- **Flatten & Dense Layers**: Fully connected network.
- **Output**: Softmax for classification.

### 3️⃣ Training & Evaluation
- **Optimizer**: Adam / SGD
- **Loss Function**: Categorical Crossentropy
- **Metrics**: Accuracy, Precision, Recall, F1-score
- **Visualization**: Accuracy/Loss graphs, Confusion Matrix, Feature Maps

## Results
- Model performance metrics: Accuracy, Precision, Recall, F1-score.
- Confusion Matrix and misclassified images analysis.
- Feature map visualization to understand CNN feature extraction.

## Repository Structure
```
├── dataset/             # Dataset directory
├── notebook/            # Jupyter notebook for EDA, training and evaluation
├── README.md            # Project documentation
└── requirements.txt     # Dependencies
```

## Credits
- Dataset: Intel Image Classification - Kaggle
- Frameworks: TensorFlow/Keras, Matplotlib, scikit-learn

## License
MIT License
