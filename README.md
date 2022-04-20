# MasterThesis : Investigation of Object Detection in Urban Traffic using Edge Computing
This repository contains the codes and notebooks used for master thesis. 
# Abstract:
Many hardware companies are driving towards building smart cameras with alternative
edge devices. The core business impact is to manufacture cost-effective state-of-the-art
(SOTA) vision systems. The concept of SOTA vision systems are versatility, dependability,
compact in size, cost-effective and consumes minimal power. The players in this
technological drift are devices such as; Google’s Coral Edge TPU and OpenCV AI KIT.
The devices have proved to deliver a favourable quality to inference neural networks models
efficiently. The current research in the domain has many cumbersome tasks and unsolved
questions. Combining the latest neural network topologies with the hardware is one of the
open research questions.

# Hardware : 
1) Raspberry Pi.
2) Google Coral USB Accelerator. 
3) Luxonis OAK-1 (OpenCV AI Kit-1).

# Object Detection Algorithm: 
1) YOLOv4 and TINYYOLOv4
# Software: 
![image](https://user-images.githubusercontent.com/34217063/164266810-82fa852a-666a-43f4-8fed-5aaeffcf06fc.png)

# Steps: 
# 1) Implementation of base YOLOv4: 

Step 1: Gathering and Labeling a Custom Dataset
In order to create a custom object detector you need a good dataset of images and labels so that the detector can be efficiently trained to detect objects.
This can be done using Google images or creating your own dataset and using an annotation tool to manually draw labels.

This method is the method I recommend as you can gather thousands of images and auto-generate their labels within minutes! Gathering a dataset from Google's Open Images Dataset and using OIDv4 toolkit to generate labels is easy and time efficient. The dataset contains labeled images for over 600 classes! Explore the Dataset Here!

Here is a link to github repository for the OIDv4 toolkit! Github Repo:https://github.com/theAIGuysCode/OIDv4_ToolKit

# 2) Start Training YOLOv4 on the prepared dataset from step1

