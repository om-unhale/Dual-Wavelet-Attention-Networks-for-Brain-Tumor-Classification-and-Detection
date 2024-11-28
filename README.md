# Dual-Wavelet-Attention-Networks-for-Brain-Tumor-Classification-and-Detection
Introduction:
There have been advancements in image processing tasks such as object de-
tection, image classification due to Convolutional Neural Network (CNN)
models. Current models employ the use of spatial domain relying on pixel
values. Spectral analysis of images is an aspect where the model can be fur-
ther improved upon fulfilling the objectives of noise frequency removal and
identifying the unclear edges among others. This type of CNN architecture,
combines the normal model with the multi-resolution analysis using the 2-D
Wavelet Transform (WT) for feature extraction. 2D WT helps in capturing
the approximate and detailed information of the image. Attention mecha-
nisms are also used in CNN to learn critical information and reduce redun-
dancy. Attention based models are know to provide better interpretability/
explainability and accuracy. In this work, a Dual Wavelet Attention network
(DWAN) is proposed for brain tumor detection and classification. It consists
of a wavelet channel attention and a wavelet spatial attention. [1] served as
the primary source for most of the work in this study. .We used an aug-
mented dataset from Kaggle for our experiments : https://github.com/sartajbhuvaji/brain-tumor-classification-dataset

The base architecture used in the experiment is ResNet18. A wavelet
channel attention module was added, followed by a wavelet spatial attention
module after each ResNet layer. Since this model is originally designed for
training on CIFAR datasets, The model was trained over 20 epochs with a learning
rate of 0.001, and the batch size was set to 32. Upon evaluation
on the test set, the model achieved a test accuracy of 90.05%.For comparison, a standard ResNet18 model (without any attention mech-
anisms) was trained on the same dataset with identical hyperparameters: a
batch size of 32 and a learning rate of 0.001. This model achieved an accu-
racy of 82.58%. These results demonstrate that the dual wavelet attention
model outperforms the standard ResNet18 model in terms of accuracy.
