﻿# Broken_Wrist_Detection_CNN_Pytorch-and-Keras

### Data: X-ray images from https://www.kaggle.com/datasets/vuppalaadithyasairam/bone-fracture-detection-using-xrays dataset.
- Has multiple images nd pespectives of patients who have a fractured wrist. The images are 224x224

## Models in PyTorch and Keras are both Convolutional Neural Networks
- Keras model has 4 convolutional layers and 2 fully connected layers. Using basic data augmentation using keras libraries, accuracy came to about 75%
  due to running on cpu and less epochs and the fac that the images have the patient ID on them which may throw things off. It uses a binary
  crossentropy loss function because this is a binary classification case.
  
- PyTorch Model has 4 convolutional and 2 fully connected layers as well, but it uses a ReLU activation instead of a sigmoid and has more hidden layers.
  The model architecture is based on the TinyVgg CNN which performs well on simple image classification tasks.
  *Note if image is NOT colored, output shape should 2, otherwise, use your data.shape() to find the necessary output shape of model
  
