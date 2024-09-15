# Project 3 : Self-Driving Car
The self-driving car model is used for autonomous driving in which its main use is to detect, identify, and calculate the distance of objects commonly encountered on the road with respect to the driver's vehicle. The objects include the road itself, people, and other vehicles. This project first experimented with 3 base models (Vanilla CNN, VGG16, and ResNet50) and 3 segmentation heads (FCN8, U-Net, and SegNet) to obtain the combination with highest performance potential. The decision is based on the value of validation dice loss. The best model, being the ResNet50_U-Net model was then finetuned, mainly from augmentation of training images.

## image-segmentation-keras library
the completion of this project was eased through the availability and publicly allowed use of the [image-segmentation-keras](https://github.com/divamgupta/image-segmentation-keras) library by divam gupta.

## Links :
1. [Presentation Slides](https://www.canva.com/design/DAGMnc-UYDY/rh_0MRh2Wvog_BYK2Fgc5w/edit)
2. [Project timeline and results sheet](https://docs.google.com/spreadsheets/d/19r60rSKzbD9wwQJAUAhbfaILK345ghxz2j73iuzR9q8/edit?usp=sharing)
3. [Hugging Face Interface](https://huggingface.co/spaces/eurekalabdawara/computervision-keras-segmentation)

## File Decriptions :
1. Model Test notebooks : contains jupyter notebooks of the initial 9 models that were the combination of the 3 base models and 3 segmentation heads. It is divided into different folders based on the segmentation heads. All notebooks were run on Kaggle using the GPU T4 x2 accelerator.
2. Resnet50-Unet Finetuning Notebooks : contains 4 jupyter notebooks with different finetuning parameters (mainly training image augmentation).
3. dataset : contains the training-and-validation images-and-annotations for model training. this dataset is a prepped subset of the "Cityscapes" dataset.
4. Gradio_inference (Gcolab).ipynb : is a notebook to run a gradio inference in google colaboratory (Gcolab) that utilizes the best finetuned ResNet50_U-Net model from our study to analyze images or videos.

## Getting started : 
1. If the user decides to use Kaggle, creation of an account and identity verification in the settings are required to run the notebooks using accelerators. 
2. Uploading the dataset on Kaggle:
    - Select 'Datasets' from the Kaggle menu and select 'New Dataset'.
    - upload all the files ('dataset' folder).
    - configure the dataset title and visibility.
    - check the files and configurations, then select 'Create' to finish creating the new dataset. After that, it can be called from the 'Input' menu of a notebook.
3. The steps to open and run the notebooks on Kaggle:
    - Select the large '+' sign in the Kaggle menu and select 'New Notebook'.
    - select 'File' in the toolbar and select 'Import Notebook'. a prompt to upload a file will then be shown.
    - upload a single desired notebook from either notebook folders.
    - select the little arrow at the bottom right corner to reveal the notebook configurations. In the 'Input' section, add the previously created dataset. Also, configure the 'Session options' to the desired accelerator, and activate the 'Internet' option to allow downloads from the internet.
    - depending on the user's dataset path, one will need to adjust the data path regarding the dataset location.
