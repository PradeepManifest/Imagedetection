# Emotion-detection

## Introduction

This project aims to classify the emotion on a person's face into one of **seven categories**, using deep convolutional neural networks. 
## Dependencies: 

* Python 3.5+, [OpenCV 3.0](http://opencv.org/opencv-3-0.html), [TFlearn](http://tflearn.org/). 

## Usage


* To run the program to detect emotions only in one face, type `python em_model.py singleface`.

* To run the program to detect emotions on all faces close to camera, type `python em_model.py multiface`.

## Algorithm

* First, we use **haar cascade** to detect faces in each frame of the webcam feed.

* The region of image containing the face is resized to **48x48** and is passed as input to the ConvNet.

* The network outputs a list of **softmax scores** for the seven classes.

* The emotion with maximum score is displayed.

## Example Output

![Happy](examples/happy.png)
