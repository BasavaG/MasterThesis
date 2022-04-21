# MasterThesis : Frankfurt University of Applied Scieces Author: Basavaraj Prakash Gangadhar.
This repository contains the codes and notebooks used for master thesis. 

# Hardware : 
1) Raspberry Pi.
2) Google Coral USB Accelerator. 
3) Luxonis OAK-1 (OpenCV AI Kit-1).

# Object Detection Algorithm: 
1) YOLOv4 and TINYYOLOv4
# Software: 
![image](https://user-images.githubusercontent.com/34217063/164266810-82fa852a-666a-43f4-8fed-5aaeffcf06fc.png)

# Steps: 
# I) Implementation of base YOLOv4: 

# 1): Gathering and Labeling a Custom Dataset
In order to create a custom object detector you need a good dataset of images and labels so that the detector can be efficiently trained to detect objects.
This can be done using Google images or creating your own dataset and using an annotation tool to manually draw labels.

This method is the method I recommend as you can gather thousands of images and auto-generate their labels within minutes! Gathering a dataset from Google's Open Images Dataset and using OIDv4 toolkit to generate labels is easy and time efficient. The dataset contains labeled images for over 600 classes! Explore the Dataset Here!

Here is a link to github repository for the OIDv4 toolkit! Github Repo:https://github.com/theAIGuysCode/OIDv4_ToolKit

# 2) Start Training YOLOv4 on the prepared dataset from step1
Refer to "YOLOv4_Custom_Training Notebook" from my repository. 

# 3) Conversion of YOLOv4 to tflite Edge tpu compatable version(Quantized). 
The "baseyolov4_to_edgetpu" notebook under "edgetpu" folder contains a code and description of converting YOLOv4 trained model to edge tpu compatable tflite version. 

# 4) Conversion of YOLOv4 to OAK-1 edge device compatable version. 
The "baseyolov4_to_oak-1" notebook under "oak-1" folder contains a code and description of converting YOLOv4 trained model to OpenVINO and then to OAK-1 compatable  .blob version. 

# 5) Implementation of YOLOv4 Object detection on vehicle dataset on Raspberry Pi.
"Pi-YOLOv4" folder contains a code to execute YOLOv4 model on Raspberry Pi. 
Prerequsite: Setup Raspberry Pi.

# 6) Implementation of YOLOv4 Object Detection on vehicle dataset using Google Coral Stick on PI.
"edgetpuyolo4" folder contains a code for delegating "quantized_yolov4" model to USB accelerator which is attached to PI's 3.0 USB port and execute it. 

# 7) Implementation of YOLOv4 Object Detection on vehicle dataset using OAK-1.
"oak-1" folder contains a code for delegating YOLOv4's .blob model to OAK-1 device which is attached to Windows machine 3.0 USB port and execute it.




