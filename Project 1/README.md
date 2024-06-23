# Project 1 : Gender Classification
Face recognition is an algorithm to identify and differentiate human faces based on an image (or videos, a collection of images). One subpart of the face recognition algorithm is gender classification, used to determine whether a subject is male or female. This project explores the use 3 convolutional neural networks (VGG, ResNet, GoogLeNet) for gender classification. 

## Links :
1. Presentation Slides : https://www.canva.com/design/DAGIXLt-BeA/9t1ztxUv5TCdiBzK6QeSFQ/edit?utm_content=DAGIXLt-BeA&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton
2. Project timeline and results sheet : https://docs.google.com/spreadsheets/d/1_9GufGzPxtFupQge11p2blhVwx8wQ4Gw6InpppjLgys/edit?usp=sharing

## File Decriptions :
1. notebooks : contains jupyter notebooks divided into different folders based on the 3 variations done in our project. Each model folder contains 10 files, each one being a different model or its sub-variation. All notebooks were run on Kaggle using the GPU T4 x2 accelerator.
2. Images : is a folder containing 5017 images of various artists but containing a few duplicates, which will be filtered in all notebooks. The image dataset is a subset of the 'CelebA' dataset.
3. list_attribute.txt : contains the attributes of all approximately 200,000 images. This will be filtered to only contain those available in the 'Images' folder in all notebooks. Also, only the ['Male'] column will be utilized for this project. 
4. validation_images : contains 10 random face images (5 male and 5 female) to validate each model after training.
