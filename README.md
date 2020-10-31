# Strategy to improve the accuracy of CNN architectures applied to digital image steganalysis in the spatial domain

In recent years, Deep Learning (DL) techniques applied to steganalysis have surpassed the traditional two-stage approach by unifying feature extraction and classification in a single model, the Convolutional Neural Network (CNN). Several CNN architectures have been proposed to solve this task, improving the detection accuracy of steganographic images, but it is not clear which computational elements are relevant. Here we present a strategy to improve accuracy, convergence, and stability during training. The strategy involves a preprocessing stage with Spatial Rich Models (SRM) filters, Spatial Dropout, Absolute Value layer, Batch Normalization, and fully connected layers. Using the strategy improves the performance of three steganalysis and two image classification CNN’s, by enhancing the accuracy from 2% up to 10% while reducing the training time to less than 6 hours and improving the networks’ stability.

## Files

 - "Entrenamiento_redes.ipynb" contains the CNN implementations in TensorFlow.
 - "SRM_Kernels.npy" is the NumPy Array file containing the 30 filters used in the preprocessing stage.
 - Folder "Databases"
