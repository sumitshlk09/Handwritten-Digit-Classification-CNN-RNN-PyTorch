# Handwritten Digit Classification using CNN & LSTM

## 📌 Project Overview

This project implements and compares two deep learning approaches for handwritten digit classification using the MNIST dataset:

- Convolutional Neural Network (CNN)
- Long Short-Term Memory (LSTM) based Recurrent Neural Network (RNN)

The models were developed using PyTorch and evaluated using accuracy, precision, recall, F1-score, confusion matrices, and training/validation performance curves.

---

## 🎯 Objective

The main objective of this project is to build deep learning models capable of recognizing handwritten digits from 0 to 9 and compare the performance of CNN and LSTM-based RNN architectures.

---

## 📊 Dataset

The project uses the MNIST handwritten digit dataset available through `torchvision.datasets.MNIST`.

### Dataset Details

- Training images: 60,000
- Test images: 10,000
- Image size: 28 × 28 pixels
- Number of classes: 10
- Classes: 0–9
- Image type: Grayscale

The dataset is automatically downloaded when the notebook is executed.

---

## 🛠️ Technologies Used

- Python
- PyTorch
- Torchvision
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 🧠 Models Implemented

### 1. Convolutional Neural Network (CNN)

The CNN model consists of:

- Convolutional layers
- Batch Normalization
- ReLU activation
- Max Pooling
- Fully Connected layers
- Dropout

The CNN is designed to extract spatial features from handwritten digit images.

### 2. LSTM-based Recurrent Neural Network

The LSTM model treats each 28 × 28 image as a sequence of 28 rows, where each row contains 28 pixel values.

The sequence is processed by an LSTM network followed by fully connected layers for classification.

---

## ⚙️ Data Preprocessing

The following preprocessing steps were performed:

1. Convert images to PyTorch tensors.
2. Normalize image pixel values.
3. Split the training data into training and validation sets.
4. Create DataLoaders for batch-based training.

---

## 🔬 Training Techniques

The following techniques were used:

- Adam optimizer
- Cross-Entropy Loss
- Batch Normalization
- Dropout regularization
- Learning Rate Scheduler
- Early Stopping
- GPU acceleration when available

---

## 📈 Results

| Model | Test Accuracy |
|---|---:|
| CNN | **99.33%** |
| LSTM (RNN) | **98.82%** |

Both models achieved significantly higher than the required 95% accuracy.

---

## 📊 Model Evaluation

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- Training Loss
- Validation Loss
- Training Accuracy
- Validation Accuracy


## 🚀 How to Run

### 1. Clone or download the repository

Download the repository as a ZIP file from GitHub.

### 2. Install the required libraries

```bash
pip install -r requirements.txt
