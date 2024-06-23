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

## Getting started : 
1. If the user decides to use Kaggle, creation of an account and identity verification in the settings are required to run the notebooks using accelerators. 
2. Uploading the dataset and validation images:
    a. Select 'Datasets' from the Kaggle menu and select 'New Dataset'.
    b. upload all the files ('Images' folder, list_attribute.txt, and validation_images).
    c. configure the dataset title and visibility.
    d. check the files and configurations, then select 'Create' to finish creating the new dataset. After that, it can be called from the 'Input' menu of a notebook. 
3. The steps to open and run the notebooks on Kaggle will be explained below.
    a. Select the large '+' sign in the Kaggle menu and select 'New Notebook'.
    b. select 'File' in the toolbar and select 'Import Notebook'. a prompt to upload a file will then be shown.
    c. upload a single desired notebook from the 'notebooks/Models..' folders.
    d. select the little arrow at the bottom right corner to reveal the notebook configurations. In the 'Input' section, add the previously created dataset. Also, configure the 'Session options' to the desired accelerator, and activate the 'Internet' option to allow downloads from the internet.
    e. depending on the user's dataset path, one will need to change the data_path (first cell in 'Data Preparation') and val_images_list (fourth cell in 'Validation').
