# Project 4 : Beach Litter Segmentation
The beach litter segmentation model is used for detecting and marking natural and artificial (man-made) beach litter. This project first experimented with 2 segmentation models, which are ResNet50_U-Net and YOLOv8-seg. Through qualitative assessment, the YOLOv8x-seg model is the one that provided good predictions for our objective.

## Beach Litter Dataset
the [dataset](https://www.seanoe.org/data/00743/85472/) used in this project is an openly-available dataset provided by Sugiyama, D., et al. (2022). The dataset contains 3500 images and masks, and has 8 classes. A more detailed explanation regarding the dataset is provided in the form of a [journal article](https://www.sciencedirect.com/science/article/pii/S2352340922002839) by the authors.

## image-segmentation-keras Library
the completion of this project was eased through the availability and publicly allowed use of the [image-segmentation-keras](https://github.com/divamgupta/image-segmentation-keras) library by divam gupta.

## Links :
1. [Presentation Slides](https://www.canva.com/design/DAGQGo2w1VY/dxAXfBKHrBVpZF4kF-vXUg/view?utm_content=DAGQGo2w1VY&utm_campaign=designshare&utm_medium=link&utm_source=editor)
2. [Project timeline and results sheet](https://docs.google.com/spreadsheets/d/1adIJcgWbDG36tMfm9UOGmAXjsSNw-R6rneAdyVGLLpA/edit?usp=sharing)
3. [Hugging Face Interface](https://huggingface.co/spaces/eurekalabdawara/beach-litter-segmentation-YOLOv8x)

## File Decriptions :
1. Dataset Format Examples : contains pictures of how the structure of the dataset should be. The ResNet50-Unet dataset structure is more flexible and hence the structure and folder names can safely be changed without any problems. Meanwhile, the YOLOv8-seg is more rigid when it comes to its dataset structure, hence the structure and folder names should be followed as to avoid unnecessary problems when training.
2. Notebooks : contains the notebook for training the ResNet50-Unet and YOLOv8-seg models. Other than that, the mask pallete changer notebook to change the colorful palette of the original masks to grayscale, and the notebook to automatically create YOLOv8 annotations from masks are also provided. Users can freely change the parameters as they see fit. 
3. Processed Masks : Contains the prepped masks already divided into train, validation, and test folders that was implemented in this project. Folders ending in '8classes' refer to the original beach litter dataset masks convertedd to grayscale. Meanwhile, folders ending in '3classes' refer to masks that focus only on the litters, resulting in (background, artificial litter, natural litter) class indexing.
4. YOLOv8 Annotations : contains the prepped YOLOv8 annotations already divided into train, validation, and test folders.

## Getting started : 
1. If the user decides to use Kaggle, creation of an account and identity verification in the settings are required to run the notebooks using accelerators. 
2. Uploading the dataset on Kaggle:
    - Configure the structure and folder names in the user's local file manager. Then compress the file before uploading to avoid kaggle upload file amount limitations. 
    - Select 'Datasets' from the Kaggle menu and select 'New Dataset'.
    - Upload the zip file.
    - Configure the dataset title and visibility.
    - Check the files and configurations, then select 'Create' to finish creating the new dataset. After that, it can be called from the 'Input' menu of a notebook.
3. The steps to open and run the notebooks on Kaggle:
    - Select the large '+' sign in the Kaggle menu and select 'New Notebook'.
    - Select 'File' in the toolbar and select 'Import Notebook'. a prompt to upload a file will then be shown.
    - Upload a single desired notebook from either notebook folders.
    - Select the little arrow at the bottom right corner to reveal the notebook configurations. In the 'Input' section, add the previously created dataset. Also, configure the 'Session options' to the desired accelerator, and activate the 'Internet' option to allow downloads from the internet.
    - depending on the user's dataset path, one will need to adjust the data path regarding the dataset location.
