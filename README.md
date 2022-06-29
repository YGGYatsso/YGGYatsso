# Image Colorization Using Conditional Generative Adversarial Network
*  image to be inserted blacn white
*  corresponding colorised image to be added
## Table of Contents:
* Overview of project
* CGAN and Model Architecture
* Data description
* libraries used
* Training
* ------
* References
## Overview of project
We will use CGAN based deep learning model to colorise black and white images.Goal is to implement and end-to-end deep learning pipeline to automate image colorisation.
## CGAN and Model Architecture
* GAN is a Generative Adversarial Network where two different model compete against one another.It involves Generator and Discrminator.Generator tries to give output which can fake the discriminator ability to predict it as fake not real.Generator is fed,a latent vector with some added noise as an input.In Condtional-GAN base architecture remains same i.e here also Generator and Discrminator with their adversarially learning behaviour.But in this, we add extra label y, which can be a vector or any image , while feeding to Generator and same label with generator output to Discrminator.For more detail info about CGAN visit
<a href='https://jonathan-hui.medium.com/gan-cgan-infogan-using-labels-to-improve-gan-8ba4de5f9c3d'>C-GAN</a>.
* Colorisation can be thought of as image to image translation and CGAN is perfect in realising this task,we feed a black and white image and get colorise output.For Generator Model ,we will be implementing modified U-net Architecture and in Discrminator we will be using PatchGAN discriminator ,rather than giving a single scalar value it gives output having matrix based output for each input.More detail about architecture can be found at <a href='https://arxiv.org/pdf/1611.07004.pdf'>PIX2PIX</a>
* Sample U-net
* sample U-net image to be added.

## Data description
* We are using fastai api to download the 10000 image samples from COCO dataset. 
<pre>.
└── fastai api(COCO Dataset)   
     ├── train    
     │   └── ... (8000 sets of  images total)           
     └── test
         └── ... (2000 sets of  images total)</pre> 
      
* Steps:
  
  

