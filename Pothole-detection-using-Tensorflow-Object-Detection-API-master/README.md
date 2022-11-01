# Pothole-detection-using-Tensorflow-Object-Detection
Custom object detection classifier, detecting Potholes on roads. Used Tensorflow Object Detection API

## Brief Summary
This repository is the application of learned knowledge of 'Object Detection Using Tensorflow'.
This repo is all about detecting Potholes on an image of a road having potholes and the process I followed in doing so.


<p align="center">
  <img src="pothole_testImages/432_out.JPG">
</p>

This model is trained to detect and differentiate 4 different classes,namely
1. Pothole
2. Pothole Group (Having more than 2 potholes on the image or a Big Pothole. PS:Created this caz to escape labelling each and every tiny pothole in the image :P which is extremely a gruelling task)
3. Car
4. Auto

I had labelled and trained the model in such way that detecting Pothole and Pothole group is the main priority.

## Implementation
#### 1. Gather required images and label them.
I had got the Pothole images dataset from [Kaggle](https://www.kaggle.com/sachinpatel21/starter-code-to-view-dataset-images/data)
I had used [LabelImg](https://github.com/tzutalin/labelImg) which is an open tool for labelling your images.
#### 2. Set up TensorFlow Directory and Anaconda Virtual Environment
The TensorFlow Object Detection API requires using the specific directory structure provided in its GitHub repository. It also requires several additional Python packages, specific additions to the PATH and PYTHONPATH variables, and a few extra setup commands to get everything set up to run or train an object detection model.


#### 3. Model used: Faster-RCNN-Inception-V2-COCO model from TensorFlow's model zoo
TensorFlow provides several object detection models (pre-trained classifiers with specific neural network architectures) in its [model zoo](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/detection_model_zoo.md)

#### 4. Install all the required Python Libraries present in requirements.txt
It is better you create a Anaconda virtual environment and do your stuff in there.
#### 5. Training and exporting the Inference graph.

