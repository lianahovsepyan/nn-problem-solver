# Neural Network Problem Solver - Fashion MNIST

## Introduction
This project builds, trains, and evaluates a TensorFlow/Keras **Sequential Neural Network** to solve an image classification problem using the **Fashion MNIST** dataset (10 clothing categories).

## How to Run
1. Open `fashion_mnist_nn.ipynb` in Jupyter Notebook or VS Code.
2. Execute cells sequentially to inspect data loading, model architecture, training curves, and final test evaluations.

## Libraries & Functions Used
- **TensorFlow / Keras**: `Sequential`, `Flatten`, `Dense`, `Dropout` layers.
- **NumPy**: Data manipulation and array transformations.
- **Matplotlib & Seaborn**: Visualizing sample images, training curves (Loss vs Accuracy), and Confusion Matrix.
- **Scikit-Learn**: `classification_report` and `confusion_matrix` for in-depth metric analysis.

## Model Architecture (`model.summary()`)
- **Input Layer:** `Flatten(input_shape=(28, 28))` - converts 2D images to 784 1D vectors.
- **Hidden Layer:** `Dense(128, activation='relu')` with `Dropout(0.2)` to prevent overfitting.
- **Output Layer:** `Dense(10, activation='softmax')` for multi-class classification.

## Results & Observations
- **Test Accuracy:** ~88% on unseen test images.
- **Loss vs Accuracy Plots:** Plotted using `history.history` for training and validation splits across epochs.
- **Key Observations & Confusion Analysis:**
  - The model performs exceptionally well on distinct categories like *Trouser* and *Ankle boot*.
  - The most common confusion occurs between visually similar classes, specifically **Shirt vs. T-shirt/top** and **Pullover vs. Coat**.
  - The `Dropout(0.2)` layer effectively stabilized training and minimized overfitting between training and validation accuracy.
