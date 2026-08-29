# Neural Network Problem Solver — Fashion Item Classification

## 1. Project Overview & Introduction
This project builds a Deep Feedforward Neural Network using TensorFlow / Keras to classify 28x28 grayscale images of clothing into 10 categories.

## 2. Dataset & Features
- **Dataset**: Fashion-MNIST (60,000 train, 10,000 test images).
- **Classes (10)**: T-shirt/top, Trouser, Pullover, Dress, Coat, Sandal, Shirt, Sneaker, Bag, Ankle boot.

## 3. Neural Network Architecture
- **Flatten Layer**: Reshapes 28x28 images into a 784-element vector.
- **Dense Layers**: 128 & 64 hidden units with ReLU activation.
- **Dropout (20%)**: Prevents overfitting.
- **Output Layer**: 10 units with Softmax activation.

## 4. Model Results & Accuracy
- **Test Accuracy**: ~88%
- **Optimizer**: Adam | **Loss**: Sparse Categorical Crossentropy

## 5. How to Run
```bash
jupyter notebook solution.ipynb
```

## Submission Status
Feature branch ready for Pull Request.
