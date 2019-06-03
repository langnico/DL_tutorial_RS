# Tutorial: Introduction to convolutional neural networks (CNNs)

This tutorial introduces a simple CNN with keras and tensorflow to classify remote sensing images from the [UC Merced dataset](http://weegee.vision.ucmerced.edu/datasets/landuse.html).


## Getting Started

1. Clone this repository to your local machine. In your terminal type:

```
git clone https://github.com/langnico/DL_tutorial_RS.git
```

2. Download the data and pre-trained models from this link:

[Google Drive](https://drive.google.com/drive/folders/1GyuSRVqXoMK9DuLWB-0XMS5-vnIVE5as?usp=sharing)

Move the directories into the code directory `DL_tutorial_RS/`. The directory tree should look like this:

* DL_tutorial_RS/
	* data/
	* pretrained_model_simpleCNN/


## Prerequisites

We are going to execute the code in a jupyter notebook and use keras with a tensorflow backend. 

Therefore, we need to install:

* python3
* jupyter
* tensorflow

Further we will need the python packages/modules:

* sklearn
* numpy
* matplotlib
* keras


## Installing
We propose to install python via anaconda.
1) [Install Anaconda](https://docs.anaconda.com/anaconda/install/) and read the [Anaconda tutorial (20min)](https://conda.io/docs/user-guide/getting-started.html)

2) Create a new environment: ```conda create --name DLenv python=3.6```
3) Activate the new environment
    * Windows: ```activate DLenv```
    * Linux and macOS: ```source activate DLenv```
    
    --> now your terminal prompt should start with ***(DLenv)*** 
4) Install the following packages in your activated DLenv:
    
    ```
    conda install jupyter
    conda install scikit-learn
    conda install matplotlib
    conda install keras
    ```
    
5) Install tensorflow with pip in the activated anaconda environment (DLenv).

For example install the current stable release for *CPU-only*:
```
pip install tensorflow
```

Alternatively, install tensorflow with *GPU support* using: `tensorflow-gpu`. For the GPU version you might have to follow the [official tensorflow installation instructions](https://www.tensorflow.org/install/pip)
or check the [anaconda installation instructions](https://tensorflow-object-detection-api-tutorial.readthedocs.io/en/latest/install.html).


## Verify your installation
1. In the activated DLenv type ```which jupyter```. This should point to the python installation in your conda env e.g. ```/username/anaconda3/envs/DL_tutorial/bin/jupyter```

2. Open a terminal and go to the location of the file: `installation_check.ipynb`

    Then open this jupyter notebook with: ```jupyter notebook installation_check.ipynb```

    NOTE: If this does not automatically open a browser showing the notebook, then open a browser (Firefox, Chrome) and type: `http://localhost:8888/notebooks/installation_check.ipynb`
    
    Then select the first cell containing the imports and click on the `> Run` Button.
    If your installation was successful, the output should be something like this:
    
    ```
    Using TensorFlow backend.
    successfully imported
    keras version:  2.2.4
    ```

## Code inspirations

* https://github.com/tgjeon/Keras-Tutorials
* https://github.com/flyyufelix/cnn_finetune

## Authors
* Nico Lang 







