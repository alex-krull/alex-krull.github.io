---
layout: page
title: Student Projects
permalink: /student-projects/
---


Topic Discussions Meetings
------------------------
If you are interested in doing your project under my supervision, please **drop me an email including "STUDENT PROJECT" in the subject** and if you have time please come to the meeting at
* **Friday March 1 at 4pm in room 217** in the computer science building.


Attention-based Model Architecures for Denoising 
------------------------
Traditionally, the [U-net architecture](https://en.wikipedia.org/wiki/U-Net) has been very popular fro image denoising in the microscopy image domain.
The goal of this project is to apply more modern architectures such as [RIN](https://github.com/lucidrains/recurrent-interface-network-pytorch) and quantitatively evaluate the results.

Denoising for Imaging Mass Cytometry 
------------------------
[Imaging mass cytometry](https://en.wikipedia.org/wiki/Mass_spectrometry_imaging) produces multichannel images where pixel-values correspond to the number of moluecules that have been detected for each location.
This type of noise follows a [Poisson distribution](https://en.wikipedia.org/wiki/Shot_noise).
The aim of this project is to implement and evaluate self-supervised denoising using the [GAP approach](https://github.com/krulllab/gap).

![image](https://github.com/alex-krull/alex-krull.github.io/assets/1193459/ed2483aa-7823-4cd8-a29b-1cf8d34a74ec)

![image](https://github.com/alex-krull/alex-krull.github.io/assets/1193459/48ed1e0f-12de-41c9-a0ff-339981cd4a42)


Games on a Goldberg Polyhedron 
------------------------
In games, [hexmaps](https://en.wikipedia.org/wiki/Hex_map) have certain advantages over regural square tilings.
The goal of this project is to develop a game on a spherical planet covered by a hexmap.
This can be achieved using [Goldberg polyhedra](https://en.wikipedia.org/wiki/Goldberg_polyhedron).
Ideally, the game could feel like a normal hexmap-based game when zoomed in.
It could be achieved using the [Unreal](https://en.wikipedia.org/wiki/Unreal_Engine) or [Unity](https://en.wikipedia.org/wiki/Unity_(game_engine)) game engine.

![image](https://github.com/alex-krull/alex-krull.github.io/assets/1193459/a48cb0db-4df4-4986-8319-486fd2da9a2f)


GANs for Fluorescence Microscopy 
------------------------
<img src="/assets/student-projects/rgb.png" width="150px" height="150"> <img src="/assets/student-projects/red.png" width="150px" height="150"> <img src="/assets/student-projects/green.png" width="150px" height="150"> <img src="/assets/student-projects/blue.png" width="150px" height="150">

(Images by Tony Collins)

Generative Adversarial Networks (GANs) are powerful image models that can a learn probability distribution over images.
That is, once they are trained on a set of training images, they can produce similar generated images that are of the same type.
The goal of this project is to apply the technology to multi channel [fluorescence microscopy](https://en.wikipedia.org/wiki/Fluorescence_microscope) images.
Fluorescence microscopy allows us to highlight multiple parts of the living cell in different colour channels.
However, the number of channels that can be imaged at the same time is limited.
A generative model could help to mitigate these limitations.

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
A generative model could help to mitigate these limitations.

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
