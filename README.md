# Handwritten Digit Recognition ✍️

A Deep Learning project built with **PyTorch** to recognize handwritten digits (0–9) using the MNIST dataset. The model is a Multi-Layer Perceptron (MLP) trained to classify 28×28 grayscale images.

The project is implemented in **Google Colab**, making it easy to run without setting up a local Python environment.

## 🚀 Project Overview

The goal is to build and train a neural network that can recognize handwritten digits from images.

The notebook covers the complete Deep Learning workflow, from loading and preprocessing the dataset to training, evaluation, and making predictions on custom images.

## 🧠 Model Architecture

The project uses a Multi-Layer Perceptron (MLP) with the following architecture:

```text
Input Image (28 × 28)
        |
     Flatten
        |
   Linear (784 → 128)
        |
      ReLU
        |
    Dropout (0.2)
        |
   Linear (128 → 64)
        |
      ReLU
        |
    Dropout (0.2)
        |
   Linear (64 → 10)
        |
   Digit Prediction (0–9)
```

**Training configuration:**
- Optimizer: Adam
- Loss Function: Cross-Entropy Loss
- Learning Rate: 0.001
- Batch Size: 64
- Maximum Epochs: 15
- Early Stopping: Patience of 4 epochs

## 📊 Dataset

The project uses the [MNIST dataset](https://yann.lecun.com/exdb/mnist/), which contains 70,000 grayscale images of handwritten digits.

- 55,000 training images
- 5,000 validation images
- 10,000 test images
- Image size: 28 × 28 pixels
- Number of classes: 10 (digits 0–9)

The dataset is automatically downloaded through `torchvision`.

## 🛠️ Technologies Used

- Python
- PyTorch
- Torchvision
- NumPy
- Matplotlib
- Pillow
- Google Colab


## 🔍 Custom Image Prediction

You can test the trained model with your own handwritten digit images.

1. Run the prediction section in the notebook.
2. Upload an image containing a single handwritten digit.
3. The image is converted to grayscale, resized to 28×28, and normalized.
4. The model predicts the digit and displays its confidence score.

**Tip:** For better predictions, use clear, centered digits with good contrast.

## 📈 Evaluation

The model is evaluated using:
- Training and validation loss.
- Training and validation accuracy.
- Test loss.
- Test accuracy.

The notebook also generates training curves to visualize the model's learning progress.

## 💡 Possible Improvements

- Implement a Convolutional Neural Network (CNN).
- Add a confusion matrix.
- Experiment with different optimizers and hyperparameters.
- Improve image preprocessing for custom handwritten digits.

## 🎯 Learning Objectives

Through this project, I explored:
- Building neural networks using PyTorch.
- Loading and preprocessing image datasets.
- Understanding training and validation loops.
- Using loss functions and optimizers.
- Evaluating classification models.
- Making predictions on unseen images.

---

**Author:** [GitHub Profile](https://github.com/kkifouche-ctrl)
