# Lung Disease Classification Using X-Ray Images

## Overview
This project aims to classify lung X-ray images into four categories: 
- **Covid-19**
- **Normal**
- **Viral Pneumonia**
- **Bacterial Pneumonia**

Using transfer learning with a pre-trained **ResNet50** model, the system processes and analyzes chest X-ray images to provide accurate classifications.

## Features
- Loads and preprocesses lung X-ray images.
- Uses **TensorFlow's ImageDataGenerator** for data augmentation and normalization.
- Implements **ResNet50** with transfer learning for improved accuracy.
- Includes early stopping and model checkpointing for optimal performance.
- Evaluates model performance using a confusion matrix and classification report.
- Generates visualizations of predictions against ground truth labels.

## Requirements
Install the necessary dependencies using:
```bash
pip install numpy pandas seaborn matplotlib tensorflow keras opencv-python
```

## Dataset
- The dataset is stored in a Google Drive directory.
- Images are categorized into four classes and loaded using **ImageDataGenerator**.
- Training and validation data are split with an 80-20 ratio.

## How to Run
1. Mount Google Drive and set the dataset path.
2. Load and preprocess X-ray images.
3. Train the ResNet50-based model with early stopping and checkpointing.
4. Evaluate the model using a test set.
5. Visualize predictions and model performance metrics.

## Model Training
- Uses **ResNet50** as a base model, freezing layers up to stage 4.
- Adds custom dense layers for classification.
- Trains using **Adam optimizer** with categorical cross-entropy loss.
- Saves the best model based on validation loss.

## Evaluation
- Computes accuracy on the test dataset.
- Generates a confusion matrix for classification analysis.
- Produces a classification report with precision, recall, and F1-score.
- Displays sample predictions comparing model output with ground truth labels.

## Output
- Trained model for lung disease classification.
- Performance plots for accuracy and loss during training.
- Visualizations of test images with predicted vs. actual labels.

## License
This project is open-source and can be used for educational and research purposes.

