# SCC5830-ImageProcessing2021
Final project of the discipline  SCC5830 - Image Processing (2021) in USP São Carlos.

# Propose: Image Style Transfer using GAN

GANs, or Generative Adversarial Network, are networks capable of generating new images from a dataset, in better words, it is a method that can capture the characteristics of one image domain and figure out how these characteristics could be translated into another image domain, all in the absence of any paired training examples. 
Style transfer is an optimization technique used to take two images—a content image and a style reference image and blend them together so the output image looks like the content image, but “painted” in the style of the style reference image.  This is implemented by optimizing the output image to match the content statistics of the content image and the style statistics of the style reference image. These statistics are extracted from the images using a convolutional network. 
The input images that will be used are in https://www.kaggle.com/duttasd28/image-style-transfergoogle-images and https://www.kaggle.com/soumikrakshit/images-for-style-transfer as reference images and in the CIFAR-10 dataset as content images, available in https://www.tensorflow.org/api_docs/python/tf/keras/datasets/cifar10. 
Currently, it is planned to use the SinGAN architecture for the model. 
As output it is expected to have the content images with the style of the referemce image.
