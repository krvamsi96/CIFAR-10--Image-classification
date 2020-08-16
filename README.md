# CIFAR-10--Image-classification

##In neural networks, Convolutional neural network (ConvNets or CNNs) is one of the main categories to do images recognition, images classifications.
Objects detections, recognition faces etc., are some of the areas where CNNs are widely used.

##CNN image classifications takes an input image, process it and classify it under certain categories (Eg., Dog, Cat, Tiger, Lion). Computers sees an 
input image as array of pixels and it depends on the image resolution. Based on the image resolution, it will see h x w x d( h = Height, w = Width, d = Dimension ).
Eg., An image of 6 x 6 x 3 array of matrix of RGB (3 refers to RGB values) and an image of 4 x 4 x 1 array of matrix of grayscale image.

* The class labels and their standard associated integer values are listed below.

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

##### In this project, i have create Image classification using  Convolution Neural Network on CIFAR-10 dataset.I have made CNN using Tensorflow library for GPU (Tensorflow is used on CPU but it will take more Time to train Network)by changing Hyperparameters of CNN atlast I have got 81% accuracy on training set..
