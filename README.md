# Protein Organelle Localization Classifier using 3D Convolutional Neural Network



This repository contains code and data for training a neural network model to classify protein organelle localization labels using a 3D Convolutional Neural Network architecture. The model can accurately classify protein organelle localization labels with a test and training accuracy of 95 percent.

Getting Datasets
The dataset used in this project is the Human Protein Atlas Image Classification challenge dataset from Kaggle. In order to use this dataset, you need to have a Kaggle account and install the Kaggle API. You can do this by running the following commands:import os

if os.path.isfile('/root/.kaggle/kaggle.json'):
    print('kaggle.json file exists in /root/.kaggle directory')
else:
    print('kaggle.json file does not exist in /root/.kaggle directory')

!pip install -q kaggle

os.makedirs(os.path.expanduser('~/.kaggle'), exist_ok=True)

!cp kaggle.json ~/.kaggle/

!kaggle competitions download -c human-protein-atlas-image-classification


In conclusion, this GitHub repository presents a neural network architecture for accurate classification of protein organelle localization labels with a high accuracy rate of 95 percent. The model processes input data as three-dimensional data, with each dimension representing a color filter (red, blue, yellow, and green). The input to the neural network is represented as (samples, 2, 90, 90, 3), where the number 2 corresponds to the two types of input data used in the proposed structure - RGB images and images captured using a yellow filter. The code provides steps for obtaining the dataset, preprocessing the images, and building the model using the DenseNet201 architecture. The repository serves as a valuable resource for researchers and machine learning enthusiasts interested in developing image classification models for protein organelle localization labels.
