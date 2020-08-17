# CIFAR-10--Image-classification


#### In this notebook, I am going to classify images from the CIFAR-10 dataset. The dataset consists of airplanes, dogs, cats, and other objects. You'll preprocess the images, then train a convolutional neural network on all the samples. The images need to be normalized and the labels need to be one-hot encoded. 

## Contents
1. Get the Data
2. Understanding the dataset
3. Hands-on experience implementing normalize and one-hot encoding function
4. Tensorflow Basics
5. Model Architecture and construction (Using different types of APIs (tf.nn, tf.layers, tf.contrib))
6. Training the model (how to feed and evaluate Tensorflow graph?)
7. Prediction

## Understanding the dataset

The original a batch data is (10000 x 3072) dimensional tensor expressed in numpy array, where the number of columns, (10000), indicates the number of sample data. As stated in the CIFAR-10/CIFAR-100 dataset, the row vector, (3072) represents an color image of 32x32 pixels.

Since this project is going to use CNN for the classification tasks, the row vector, (3072), is not an appropriate form of image data to feed. In order to feed an image data into a CNN model, the dimension of the tensor representing an image data should be either (width x height x num_channel) or (num_channel x width x height).

It depends on your choice (check out the tensorflow conv2d). In this particular project, I am going to use the dimension of the first choice because the default choice in tensorflow's CNN operation is so.

The row vector (3072) has the exact same number of elements if you calculate 32*32*3==3072. In order to reshape the row vector, (3072), there are two steps required. The first step is involved with using reshape function in numpy, and the second step is involved with using transpose function in numpy as well.

## build the model.
 1. Convolution with 32 different filters in size of (3x3)
 2. Max Pooling by 2
 * ReLU activation function
 * Batch Normalization
 
 3.Convolution with 64 different filters in size of (3x3)
 
 4.Max Pooling by 2
 * ReLU activation function
 * Batch Normalization
 
 5.Fully Connected Layer with 512 units
 * Dropout
 * Batch Normalization
 6.Fully Connected Layer with 1024 units
 * Dropout
 * Batch Normalization
 
 
 

## The class labels and their standard associated integer values are listed below.

* 0: airplane
* 1: automobile
* 2: bird
* 3: cat
* 4: deer
* 5: dog
* 6: frog
* 7: horse
* 8: ship
* 9: truck























