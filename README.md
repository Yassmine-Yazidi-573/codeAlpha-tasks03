# codeAlpha-tasks03
# Handwritten Character Recognition (A–Z)

This project implements a Convolutional Neural Network (CNN) model to recognize handwritten English alphabets (A–Z) from images. The model is trained on a labeled dataset of characters and can be used to classify new handwritten letter images provided by the user.

## Project Overview

* **Goal**: Recognize handwritten characters (A–Z)
* **Input**: 28x28 grayscale images of individual letters
* **Output**: Predicted character (A to Z)
* **Model**: Convolutional Neural Network (CNN)
* **Dataset**: A–Z Handwritten Data (CSV format)

## Dataset

The dataset used consists of 372,450 labeled images of size 28x28 pixels, each representing a letter from A to Z.

* Format: CSV file
* Each row contains 784 pixel values + label
* Labels: 0 (A) to 25 (Z)

## How to Run

1. **Load the dataset** and preprocess the pixel values.
2. **Split** the data into training and testing sets.
3. **Build the CNN model** using Keras.
4. **Train the model** on the training data.
5. **Evaluate** the model on the test data.

## Model Architecture

* Conv2D → ReLU → MaxPooling → Dropout
* Conv2D → ReLU → MaxPooling → Dropout
* Flatten → Dense → Dense (Softmax)

## Example: Predicting a New Image

To predict a new letter image:

1. Upload an image file to Colab (`my_letter.png`)
2. Convert to grayscale, resize to 28x28, normalize
3. Run the model to predict the character
