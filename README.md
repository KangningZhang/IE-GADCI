# GDCI and IE-GADCI
## Introduction
#### Compressive sensing (CS) is a powerful technique to sample far below Nyquist rate and yet recover the information with little loss by exploiting the sparse latent representation of the information. Conventionally, the sparse latent representation is determined empirically; the recent advances of deep neural network enable learning this latent representation from the data, which is often more effective compared with those set empirically. We propose an incoherence-enhanced generative CS-inspired deep neural network called IE-GADCI (Incoherence-Enhanced Generative Adversarial Deep Compressed Imaging) for single image super-resolution (SISR) application. IE-GADCI jointly optimizes the imaging hardware and reconstruction algorithm for a high-speed single-pixel imaging modality, where a learnable point-spread-function (PSF) is used to obtain a low-resolution measurement of the image, and a neural network with a generative latent bank learns the sparse latent representation domain and recovers the super-resolution image. The super-resolution performance is further boosted by an adversarial framework to maximize the incoherence between the sensing representation and sparse latent representation. We verified the performance of IE-GADCI in nature scene and biomedical dataset through numerical simulation.
![alt text](https://github.com/KangningZhang/IE-GADCI/blob/main/Figures/Picture1.png)
![alt text](https://github.com/KangningZhang/IE-GADCI/blob/main/Figures/Picture2.png)

## System Requirements
#### 1. Quadro RTX8000 48GB is used in this project, but any GPU processor better than GTX960 6GB is acceptable. A CUDA compatible GPU is preferred.
#### 2. Tensorflow 2.9.0
#### 3. Anaconda

## Demo and installation
#### 1) Install Anaconda.
#### 2) Launch Anaconda prompt and install Tensorflow 2.9.0 as the virtual environment.
#### 3) Open the virtual environment, and then  pip install mat73, opencv-python, python-time and scipy.
#### 4) Download the "GDCI.ipynb" or "IE-GADCI.ipynb"in folder "Demo" and the simulated dataset via the google drive link. Then, create and put the training dataset in the path "./data_train1/" and "./data_test/".
#### 5) Run: Use Anaconda to launch the virtual environment and open ipynb documents. Then, please check and follow the guide of ipynb documents for training and testing.
#### Note: Every package can be installed in a few minutes.

## Simulated Dataset
#### 1.Nature Scene Data
#### data_train1: https://drive.google.com/drive/folders/1miozQb2WSwqS1NMSiPoqYs84DO5SWTvY?usp=drive_link
#### data_train2: https://drive.google.com/drive/folders/18nv5QNkpdXR2c44xCBPz4qjitUH-cFpD?usp=drive_link
#### data_train3: https://drive.google.com/drive/folders/17_17dcUV5yh4rHqzr1NnNEsUJ2cG8f_I?usp=drive_link
#### data_test: https://drive.google.com/drive/folders/1b3Ok_JsbYi_mp3rLmw6fmxy-Ruo6BSCX?usp=drive_link
#### 2. Calcium Imaging Data
#### Dataset generator: The algorithm for generating simulated dataset is based on the paper of FISSA (_Keemink, S.W., Lowe, S.C., Pakan, J.M.P. et al. FISSA: A neuropil decontamination toolbox for calcium imaging signals. Sci Rep 8, 3493 (2018). https://doi.org/10.1038/s41598-018-21640-2_) and SimCalc repository (https://github.com/rochefort-lab/SimCalc/). 
#### Training dataset: https://drive.google.com/file/d/1WZkIE_WA7Qw133t2KtqTESDmxMwsEkjJ/view?usp=share_link
#### Testing Dataset: https://drive.google.com/file/d/1zsLH8OQ4kTV7LaqQfbPDuMDuWBcHGWcO/view?usp=share_link
## Experimental Dataset
#### We used the samples from ABO dataset with depth of layer 275:
https://github.com/AllenInstitute/AllenSDK/wiki/Use-the-Allen-Brain-Observatory-%E2%80%93-Visual-Coding-on-AWS.

