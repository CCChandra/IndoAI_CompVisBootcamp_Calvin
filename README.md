# IndoAI_CompVisBootcamp_Calvin
This is a repository store projects completed in the Indonesia AI Computer Vision bootcamp.
below are subheadings that provides the names of the project along with a brief description of the project.

## Project 1 : Gender Classification
this project encourages us to use and compare 3 Convolutional Neural Networks (CNNs) to make predictions on whether an image of a human face is a male or female subject. the 3 CNNs are Visual Group Geometry (VGG), Residual Network (ResNet), and GoogLeNet (or otherwise known as Inception).

## Project 2 : Person Tracking
this project requires us to use an object detection algorithm to detect people in an image or video frame. During our attempt, the only successfully implemented model was the YOLO model.

## Project 3 : Self-Driving Car
this project is aimed to obtain an object segmentation model that can be implemented for self-driving car purposes. Therefore, detection of bicyclists, pedestrians, roads, signs, other vehicles, etc. are the main objects to be identified. for this project, we studied the combination of 3 base models (vanilla CNN, VGG16, and ResNet50) and 3 segmentation heads (FCN8, U-Net, and SegNet), resulting in 9 different models for initial experimentation. The model with highest performance (decided with validation dice loss), being the ResNet50_U-Net model was finetuned to further increase its performance.
