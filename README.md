# Strategy to improve the accuracy of CNN architectures applied to digital image steganalysis in the spatial domain

<p align="justify"> In recent years, Deep Learning (DL) techniques applied to steganalysis have surpassed the traditional two-stage approach by unifying feature extraction and classification in a single model, the Convolutional Neural Network (CNN). Several CNN architectures have been proposed to solve this task, improving the detection accuracy of steganographic images, but it is not clear which computational elements are relevant. Here we present a strategy to improve accuracy, convergence, and stability during training. The strategy involves a preprocessing stage with Spatial RichModels (SRM) filters, Spatial Dropout, Absolute Value layer, and Batch Normalization. Using the strategy improves the performance of three steganalysis and two image classification CNN's, by enhancing the accuracy from 2% up to 10% while reducing the training time to less than 6 hours and improving the networks' stability. </p>

![Ye-Net](YeNet.jpg)

<p align="center">The architecture in the top represents original Ye-Net, the one in the bottom </br> represents the architecture using the strategy </p>

## Files

 - **CNN_Implementation_evaluation.ipynb** CNN implementations in TensorFlow.
 - **SRM_Kernels.npy** NumPy Array file containing the 30 filters used in the preprocessing stage.
 - **Ye-Net.jpg** Comparison of Ye-Net architecture with and without the strategy.
 - **Trained Models** Folder that contains the best trained model for each architecture in *hdf5* format.
 - **requirements**

## Databases

The data set used to reproduce the results can be downloaded from this <a href="https://drive.google.com/drive/folders/1G5vdhW11_qKfVC6W8_pfJpstVkXUk1QQ?usp=sharing">link</a>. Images taken from: <a href="http://agents.fel.cvut.cz/boss/index.php?mode=VIEW&tmpl=materials">BOSS competition</a> and <a href="http://bows2.ec-lille.fr/index.php?mode=VIEW&tmpl=index1">BOWS2</a>.
