# Strategy to improve the accuracy of convolutional neural network architectures applied to digital image steganalysis in the spatial domain

<p align="justify"> In recent years, Deep Learning (DL) techniques applied to steganalysis have surpassed the traditional two-stage approach by unifying feature extraction and classification in a single model, the Convolutional Neural Network (CNN). Several CNN architectures have been proposed to solve this task, improving the detection accuracy of steganographic images, but it is not clear which computational elements are relevant. Here we present a strategy to improve accuracy, convergence, and stability during training. The strategy involves a preprocessing stage with Spatial Rich Models (SRM) filters, Spatial Dropout, Absolute Value layer, and Batch Normalization. Using the strategy improves the performance of three steganalysis and two image classification CNN's, by enhancing the accuracy from 2% up to 10% while reducing the training time to less than 6 hours and improving the networks' stability. </p>

![Ye-Net](YeNet.jpg)

<p align="center">The architecture in the top represents original Ye-Net, the one in the bottom </br> represents the architecture using the strategy </p>

## Folders

- **CNNs and SRM filters** This folder contains the notebooks Xu-Net, Ye-Net, Yedroudj-Net, Vgg16Stego, and Vgg19Stego architectures for steganographic images in the spatial domain. Also, it contains the SRMfilters.npy, which are used in the feature extraction stage of CNNs.

## Files

 - **YeNet.jpg** Comparison of Ye-Net architecture with and without the strategy.
 
## Requirements
This repository requires the following libraries and frameworks:

- TensorFlow 
- numPy 
- OpenCV 
- Matplotlib
- Time
- random
- os

This repository was developed in the Python3 (3.8) programming language.

## Package installation

if you don't use google colab, We highly recommend to use and install Python packages within an Anaconda enviroment. To create, execute the command below:
```
conda create --name Strategy python=3.8
```
So, activate it
```
conda activate Strategy 
```
installed the framework
```
conda install -c anaconda keras-gpu==2.4.3
```
Now, install the libraries.
```
pip install opencv-python
conda install -c conda-forge matplotlib
conda install -c jmcmurray os
conda install -c conda-forge time
```
## Execution
After installing all the Requirements, you must clone the repository of the current version of GBRAS_SW using.
```
git clone https://github.com/BioAITeam/
Strategy-to-improve-CNN-applied-to-digital-image-steganalysis-in-the-spatial-domain.git
```
If you will use colab, upload the cloned folder to drive, then open the folder "CNNs and SRM filters" and run the notebook of your choice.

if you are going to use your computer, install:
```
conda install jupyter 
```
Enter the cloned folder, then enter the "CNNs and SRM filters" folder and run the choice notebook.
 


## Databases

The data set used to reproduce the results can be downloaded from this <a href="https://drive.google.com/drive/folders/1G5vdhW11_qKfVC6W8_pfJpstVkXUk1QQ?usp=sharing">link</a>. Images taken from: <a href="http://agents.fel.cvut.cz/boss/index.php?mode=VIEW&tmpl=materials">BOSS competition</a> and <a href="http://bows2.ec-lille.fr/index.php?mode=VIEW&tmpl=index1">BOWS2</a>.
