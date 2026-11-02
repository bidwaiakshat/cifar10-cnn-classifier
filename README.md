# CIFAR-10 Image Classification using CNN

A deep learning project that uses a Convolutional Neural Network (CNN) to classify images into 10 categories using the CIFAR-10 dataset.

## Overview

This project implements an image classification workflow using TensorFlow and Keras. The model learns visual features from small RGB images and predicts the category of each image.

The project covers dataset exploration, preprocessing, CNN construction, model training, performance evaluation, and analysis of classification errors.

## Dataset

The project uses the CIFAR-10 dataset.

- **Training images:** 50,000
- **Test images:** 10,000
- **Image dimensions:** 32 × 32 pixels
- **Channels:** 3 (RGB)
- **Number of classes:** 10

### Classes

1. Airplane
2. Automobile
3. Bird
4. Cat
5. Deer
6. Dog
7. Frog
8. Horse
9. Ship
10. Truck

The dataset is loaded using TensorFlow/Keras.

## Model Architecture

The CNN contains:

- Convolutional layers with ReLU activation
- Max-pooling layers
- A flattening layer
- A fully connected dense layer
- A softmax output layer for 10-class classification

The model is trained using the Adam optimizer and sparse categorical cross-entropy loss.

## Preprocessing

- Pixel values are normalized from the range 0–255 to 0–1.
- Class labels are retained as integer class IDs.
- A validation split is used to monitor training and help identify overfitting.

## Results

The supplied notebook reports approximately **70.36% test accuracy** across the 10,000 CIFAR-10 test images.

The evaluation includes:

- Training and validation accuracy
- Training and validation loss
- Final test performance
- Sample predictions
- Correct and incorrect classification examples
- Confusion matrix
- Per-class accuracy and common classification errors

The results show that the model learns useful visual features, but it can struggle with visually similar categories.

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Google Colab

## How to Run

### Option 1: Google Colab

1. Download the `.ipynb` notebook from this repository.
2. Open [Google Colab](https://colab.research.google.com/).
3. Upload the notebook.
4. Select a suitable runtime.
5. Run the cells in order.

TensorFlow downloads the CIFAR-10 dataset when required.

### Option 2: Local Environment

Install the dependencies:

```bash
pip install -r requirements.txt
```

Open the notebook in Jupyter Notebook or JupyterLab and execute its cells.

## Possible Improvements

Potential future improvements include:

- Data augmentation
- Dropout and batch normalization
- Hyperparameter tuning
- Comparing different CNN architectures
- Improving generalization and reducing overfitting

## Author

**Akshat Shankar Bidwai**
