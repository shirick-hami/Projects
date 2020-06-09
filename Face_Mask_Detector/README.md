# Face Mask Detector

Face Mask Detector with OpenCV, Keras/TensorFlow, and Deep Learning

## Overview

In order to train a custom face mask detector, we need to break our project into two distinct phases:

1) Training: Here we’ll focus on loading our face mask detection dataset from disk, training a model (using Keras/TensorFlow) on this dataset, and then serializing the face mask detector to disk
2) Deployment: Once the face mask detector is trained, we can then move on to loading the mask detector, performing face detection, and then classifying each face as with_mask or without_mask

## Python Scripts 

1) train_mask_detector.py: Accepts our input dataset and fine-tunes MobileNetV2 upon it to create our mask_detector.model. A training history plot.png containing accuracy/loss curves is also produced
2) detect_mask_image.py: Performs face mask detection in static images
3) detect_mask_video.py: Using your webcam, this script applies face mask detection to every frame in the stream

