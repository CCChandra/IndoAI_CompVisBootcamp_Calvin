# Project 2 : Person Tracking
Object tracking is an algorithm used to detect the presence of objects and mark their location on an image or video frame. Here, the object in question are people and will implement the YOLO v8m model.

## Links :
1. [Presentation Slides](https://www.canva.com/design/DAGKjWVZ7L8/NHLMkKCIaor025SGX0J2qQ/edit?utm_content=DAGKjWVZ7L8&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)
2. [Project timeline sheet](https://docs.google.com/spreadsheets/d/1T0lfrETqY3BVNpQJ01RyxGfxmGwZvJxj6KMXCe48Tec/edit?usp=sharing)
3. [COCO 2017 kaggle dataset](https://www.kaggle.com/datasets/awsaf49/coco-2017-dataset)

## File Decriptions :
1. notebooks : contains jupyter notebooks to run the training of a YOLO v8m model (YOLO_train) and predict using said model (YOLO_predict). If a user wants to change the model, one can refer to the [ultralytics documentation](https://docs.ultralytics.com/models/yolov8/) for the sought model and change the defined model in the notebook. All notebooks were run on Kaggle using the GPU T4 x2 accelerator. Also, while the Faster-RCNN notebook is present in the folder, as it wasn't pursued due to long training time, it won't be much explained.
2. Implementation : contains a jupyter notebook to run gradio and enables the user to provide a link that can be used to detect people on an image or video. Also, the local version is also provided in a folder but will need cuda to run.

## Getting started : 
1. If the user decides to use Kaggle, creation of an account and identity verification in the settings are required to run the notebooks using accelerators. 
2. Selecting the COCO 2017 dataset from Kaggle:
    - after clicking the kaggle dataset link provided, navigate to the top right corner, then click on the 3 vertical dots.
    - select 'new notebook' to automatically open a notebook with the COCO 2017 dataset as an input.
    - in the notebook configuration (select the little arrow at the bottom right corner), don't forget to turn on 'internet'.
3. The steps to run the notebooks on Kaggle:
    - from the previously created notebook, select 'File' in the toolbar and select 'Import Notebook'. a prompt to upload a file will then be shown.
    - upload either one of the YOLO notebooks depending on the users desire.
    - in the notebook configurations, configure the 'Session options' to the desired accelerator.
    - if using the COCO 2017 dataset, a simple 'run all' will start the process. The user can then edit the notebook to configure the desired model, images, etc.
