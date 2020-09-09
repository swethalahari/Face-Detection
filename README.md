# Face-Detection-using-mobilenet
Face detection using mobilenet using keras
The goal is to build a face recognition system, which includes building a face detector to locate the position of a face in an image and a face identification model to recognize whose face it is by matching it to the existing database of faces.   This Repository aims at face detection, face recognition repository is built on this model.
# Face Detector
We will be using transfer learning on an already trained model to build our detector. We will perform transfer learning on Mobile Net model which is already trained to perform object detection. We will need to train the last 6-7 layers and freeze the remaining layers to train the model for face detection. To be able to train the Mobile Net model for face detection, we will be using WIDER FACE dataset which already has the bounding box data for various images with single face and multiple faces. The output of the model is the bounding box data which gives the location of the face in an image. We learn to build a face detection model using Keras supported by Tensorflow 
# Overview
In this problem we use "Transfer Learning" of an Object Detector model to detect any object according to the problem in hand. 
Here, we are particularly interested in detecting faces in a given image. 
# Below are the steps involved in the project. 
1. To use already trained model, we will import the model and its supporting files for the model to function.   
2.Set the parameters for the model  
3.Import the dataset for the model to train on. For this, we are using the WIDER FACE dataset.   
4.Get the labels for these images, so that we can use this information while training for detecting faces with the given model using transfer learning.
5.Making the model ready for training by freezing some layers in which we are not updating the weightswhile training. We need to train the top 6-7 layers. 
6.load the weights of the Mobile Netmodel given in file ''`mobilenet_1_0_224_tf.h5`''  
7.Set the optimizers, loss functions, epochs, learning rate, batch size, check pointing, early stopping etc.
8.Train the model  
9.Load the best saved weights 
10.Predict using test images
