# SCC5830-ImageProcessing2021
Final project of the discipline  SCC5830 - Image Processing (2021) in USP São Carlos.
Student: Taylla Milena Theodoro

# Summary 

**Main Objective** To perform image colorization (grayscale to colored) using GANs.

**Dataset** Coco-https://cocodataset.org/#home

**Steps**
- Learn about the dataset;
- Prepare the dataset: Preprocess the images from the dataset in order to perform correctly the task;
- Define the model: Chose and study architectures that can better perform the taks;
- Train the model: Feed the training images into the chosen model;
- Evaluate: Chose an evaluation capable of tell how the chosen model perfomed the task, in our case, evalute the model performace and plot the input (grayscale images), predicted and expected(original image colorful).

## Main Objective
To perform image colorization (grayscale to RGB) using GANs and learn the tools and path towards compleating this objective.

## Introduction

### Generative Adversarial Network

Generative Adversarial Network, or GANS, are networks capable of generating new images from a dataset. In other words, it is a method that can capture the characteristics of one image domain and figure out how these characteristics could be translated into another image domain, all in the absence of any paired training examples. 

### Image Colorization
According to the article [Image Colorization: A Survey and Dataset](https://arxiv.org/pdf/2008.10774.pdf), image colorization is an essential image processing and computer vision branch to colorize images and videos. It can be applied to color old movies, old photos, old video games, astronomical photography, electron microscopy, etc. 
Recently, the technic used to perform this task is with deep learning procedures, such as Convolutional Neural Networks, Residual Neural Networks and Generative Adversial Netwolks.

### Project Proposal Overview

To colorize images is an important computer vision task, which allows us to bring to life old images, therefore, in this project, it is intend to perform image colorization using GANs. The input images that will be used are a smaller set of coco dataset, available in https://cocodataset.org/#home. Currently, it is planned to use the pix2pix GAN architecture for the model. As output it is expected to have the colored image.

## Methodology

The methodoly chosed with the purpose of learning and completing this project is the by following the steps:

- **Related Work:** learn about datasets, the task, possible architectures and evaluation methods;
- **Prepare the dataset:** Preprocess the images from the dataset in order to perform correctly the task;
- **Define the model:** Chose and study architectures that can better perform the taks;
- **Train the model:** Feed the training images into the chosen model;
- **Evaluate:** Chose an evaluation capable of tell how the chosen model perfomed the task, in our case, evalute the model performace and plot the input (grayscale images), predicted and expected(original image colorful).


### Dataset

The chosen Dataset is [COCO dataset](https://cocodataset.org/#home), which contain images from diverse scenarios and locations which enable the network to learn to colorize different kinds of images. The dataset contain 330K images, however it will be used 8000 of its images for this project.

Here are some examples of images:

![Dataset Image examples](dataset_examples.png)

#### Preprocessing

The dataset contain RGB images, which will be preprocessed by using color analysis. The images will be converted to LAB images with the skimage python library, the L channel will be feed in the model and the a and b channel will be predicted by the model, so that the output can converted back to RGB and evaluated.

### Model

The model intent to be used is pix2pix presented in the paper [Image-to-Image Translation with Conditional Adversarial Networks](https://arxiv.org/abs/1611.07004) which proposed a general solution to image-to-image tasks in deep learning including image colorization. 

### Evaluation

The evaluation method is still being researched.
