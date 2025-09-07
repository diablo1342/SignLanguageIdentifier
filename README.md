<h1> SignLanguageIdentifier </h1>

## 📝 Overview 📝

Sign Language Identifier is a computer vision application that uses deep learning to classify sign language gestures from images. The model is trained on a labeled dataset and predicts the corresponding letter or symbol with high accuracy.

What makes this project special is its use of VGG16 transfer learning in PyTorch, achieving strong performance on a relatively small dataset and enabling real-time image classification for sign language recognition.

Training data was too big to fit on github, you can download it here: https://drive.google.com/drive/folders/1o-pAHnYPnEJtLkjYeFCZfORLmrIJLsY4?usp=sharing

## How I built it
Model: Pre-trained VGG16 (ImageNet weights) modified for our number of classes.

Framework: PyTorch for model training, evaluation, and inference.

Dataset: Loaded using torchvision.datasets.ImageFolder with train/test split (80/20).

Training:

Image preprocessing (resize to 224×224, normalization).

SGD optimizer and CrossEntropyLoss for classification.

Trained for 10 epochs, achieving 94.84% test accuracy.


## Built with

-Python

-PyTorch

-Torchvision

-OpenCV

-Scikit-learn

## Results

- 94% accuracy in determining gestures from images.

## Future
- Will look to incorporate this into live video recordings to allow for live translation.
