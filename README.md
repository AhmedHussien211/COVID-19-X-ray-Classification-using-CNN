🩺 COVID-19 X-ray Classification using CNN
📌 Project Overview

This project focuses on building a Convolutional Neural Network (CNN) to automatically classify chest X-ray images into three categories:

Normal

COVID-19

Viral Pneumonia

The model learns visual patterns from medical X-ray images and predicts the disease category. This project demonstrates a full deep learning pipeline, including data preprocessing, model building, training, validation, and performance visualization.

The project was implemented using Python and TensorFlow/Keras and trained on Google Colab.

📂 Dataset Structure

The dataset is divided into training and testing sets.
            dataset/
            │
            ├── train/
            │   ├── Normal/
            │   ├── Covid/
            │   └── Viral Pneumonia/
            │
            └── test/
                ├── Normal/
                ├── Covid/
                └── Viral Pneumonia/

⚙️ Data Preprocessing

Before training the model, several preprocessing steps were applied:

Directory Handling

Used the Python os library to organize dataset paths.

Image Resizing

All images were resized to a fixed size suitable for CNN input.

Normalization

Pixel values were scaled to improve model training.

Train / Validation Split

Training data was further split into:

Training set

Validation set

Data Augmentation

Implemented using ImageDataGenerator from TensorFlow to improve model generalization.

Example augmentations:

Rotation

Horizontal flip

Zoom

Width/height shift

🧠 Model Architecture

A Convolutional Neural Network (CNN) was built to extract spatial features from X-ray images.

Typical architecture components:

Convolution Layers

Activation Functions (ReLU)

MaxPooling Layers

Flatten Layer

Fully Connected Layers

Softmax Output Layer (3 classes)

👨‍💻 Author

Ahmed Hussien

Computer Vision & Deep Learning Enthusiast
