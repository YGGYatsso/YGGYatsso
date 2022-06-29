# Image Colorization Using Conditional Generative Adversarial Network
![](https://towardsdatascience.com/colorizing-black-white-images-with-u-net-and-conditional-gan-a-tutorial-81b2df111cd8)
![](https://jonathan-hui.medium.com/gan-cgan-infogan-using-labels-to-improve-gan-8ba4de5f9c3d)
## Table of Contents:
* Overview of project
* CGAN and Model Architecture
* Data description
* libraries used
* -----
* ------
* References
## Overview of project
We will use CGAN based deep learning model to colorise black and white images.Goal is to implement and end-to-end deep learning pipeline to automate image colorisation.
## CGAN and Model Architecture
* GAN is a Generative Adversarial Network where two different model compete against one another.It involves Generator and Discrminator.Generator tries to give output which can fake the discriminator ability to predict it as fake not real.Generator is fed,a latent vector with some added noise as an input.In Condtional-GAN base architecture remains same i.e here also Generator and Discrminator with their adversarially learning behaviour.But in this, we add extra label y, which can be a vector or any image , while feeding to Generator and same label with generator output to Discrminator.For more detail info about CGAN visit,

* 


