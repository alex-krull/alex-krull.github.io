---
layout: page
title: Student Projects
permalink: /student-projects/
---

GANs for Fluorescence Microscopy 
------------------------
<img src="/assets/student-projects/rgb.png" width="150px" height="150"> <img src="/assets/student-projects/red.png" width="150px" height="150"> <img src="/assets/student-projects/green.png" width="150px" height="150"> <img src="/assets/student-projects/blue.png" width="150px" height="150">

(Images byt Tony Collins)

Generative Adversarial Networks (GANs) are powerful image models that can a learn probability distribution over images.
That is, once they are trained on a set of training images, they can produce similar generated images that are of the same type.
The goal of this project is to apply the technology to multi channel [fluorescence microscopy](https://en.wikipedia.org/wiki/Fluorescence_microscope) images.
Fluorescence microscopy allows us to highlight multiple parts of the living cell in different colour channels.
However, the number of channels that can be imaged at the same time is limited.
A generative model could help to mitigate this limitations.

The aims of the project are
* Train a GAN on multichannel fluorescence microscopy data
* Find a way to evaluate the quality of the generated images
* Try to train GANs from incomplete data, that is when some of the channels are missing in parts of the training data.




VAEs for Fluorescence Microscopy 
------------------------
Like GANs (see above) variational autoencoders (VAEs) are generative image models that can learn a probability distribution over images.
That is, once they are trained on a set of training images, they can produce similar generated images that are of the same type.
The goal of this project is to apply the technology to multi channel [fluorescence microscopy](https://en.wikipedia.org/wiki/Fluorescence_microscope) images.
Fluorescence microscopy allows us to highlight multiple parts of the living cell in different colour channels.
However, the number of channels that can be imaged at the same time is limited.
A generative model could help to mitigate this limitations.

The aims of the project are 
* Train a VAE on multichannel fluorescence microscopy data
* Find a way to evaluate the quality of the generated images
* Try to train VAEs from incomplete data, that is when some of the channels are missing in parts of the training data.


MAP Image Restoration
------------------------
Most image restoration algorithms train a convolutional neural network (CNN) to learn a mapping from the degraded image to a corresponding noise-free image, often using a quadratic loss function.
However, for a given degraded image, the is generally no unique solution for the corresponding clean images.
That is, we cannot be sure what the real clean image is. 
Instead, there is a probability distribution of possible clean images for each observed noisy image.
This distribution is called the posterior distribution.
Using a quadratic loss function will lead to the network finding the mean of this distribution, i.e., a compromise between the possible solutions.
The aim of this project is to explore other loss functions, which would lead to the network finding different solutions, such as the single clean image that is most likely given the observed noisy image.



Aurotegressive Image Priors for Image Restoration
------------------------
Like GANs and VAEs [autoregressive models](https://towardsdatascience.com/autoregressive-models-pixelcnn-e30734ede0c1) are another type of generative image model.
It is more expensive to sample from an autoregressive model.
However, unLike GANs and VAEs autoregressive models allow us to directly compute the likelihood of a particular image.
The aim of this project is to train an autoregressive model on a set of images and combine it with a model of imaging noise, to compute the probability of the clean image given a noisy input.
We can then optimise the pixel values to find the most likely image given the noisy observation.

By using a different model of image degradation, we could also the approach to colourise gray scale images or to de-blur out-of-focus images.


Self-Supervised Audio Denoising
------------------------
In the last years, a number of methods have been developed for self-supervised image denoising, e.g.: 
* [N2V](https://arxiv.org/abs/1811.10980) or 
* [HDN](https://arxiv.org/abs/2104.01374)


These methods can be trained using only noisy image and do not require paired training data.
The goal of this project is to try self-supervised denoising for audio signals instead of images.
We could for example use this to denoise old recordings that contain a large ammount of noise.

Detecting Ink in Ancient Documents
------------------------
The goal of this project is to address the [kaggle challenge](https://www.kaggle.com/competitions/vesuvius-challenge-ink-detection) for detecting ink on charred roman documents helping to decipher them.


Machine Learning for COPS photon counting
------------------------
<img src="/assets/student-projects/cops.png" width="600px">
