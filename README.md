# Liveliness_Detection
<h3>1. Overview</h3>

I have done it on the local machine in 3 python scripts. Computer vision and Deep Leaning techniques are used for this purpose.

<h3>2.Data</h3>

In the folder “dataset” there are 2 subfolders :
Fake: Contains face ROIs from the fake.mp4 file
Real: Holds face ROIs from thereal.mov file

<h3>3.Other Folders and files:</h3>

Face_detector: Consists of our pretrained Caffe face detector to locate face ROIs.
Model:   This module contains our LivenessNet class.
Videos:  I’ve provided two input videos for training our LivenessNet classifier.
Results:  It contains my final results and a video.
Requirement.txt: It contains all the required packages to run this project.

<h3>3.My Approach</h3>

I decided to use resnet caffe model to detect the face from the video and over that i trained a deep neural network that was capable of distinguishing between fake or real faces. For this I used a simple Convolutional Neural Networks.
Bounding Boxes are made over the detected faces in the colour green for real time face and red for spoofed faces . Respective probablities are also displayed alongwith.
Input Footage could be taken from the webcam directly or through RTSP. Through Webcam images are usually unclear so model could get confused so i used RTSP and taken input from my mobile phone camera.

<h3>Results</h3>
The model sucessfully detects spoofed and real faces.
