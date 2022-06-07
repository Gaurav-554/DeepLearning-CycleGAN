<h1 align="center">Generative Adversarial Networks - CycleGAN for MNIST Image Generation</h1>

<h2>Background</h2>

Generative Adversarial Networks are based on the approach of Generative Modeling using deep learning methodologies. Generative Modeling is an unsupervised technique that learns the patterns and properties in the input data in such a way that the trained model can generate new examples that very closely resemble the input dataset.<br>
GAN is a very clever use of Generative Modeling by using two sub-models in conjunction as explained below:
- `Generator` | it learns to generate new examples.
- `Discriminator` | it is trained to classify examples as real or fake.

The two models are trained in an adversarial fashion until fake examples generated by the Generator are good enough to fool the Discriminator. <br>


<h2>CycleGAN</h2>

CycleGAN is a technique that involves the automatic training of image-to-image translation models without paired examples. The models are trained in an unsupervised manner using a collection of images from the source and target domain that do not need to be related in any way.

<br>
<p align="center">
  <img width="350" height="250" alt="CycleGAN Architecture" src="https://github.com/Gaurav-554/DeepLearning-CycleGAN/blob/main/img_readme/CycleGAN_img1.png">
</p>
<p align="center">
  Figure 1: CycleGAN Architecture
</p>
<br>

The main idea behind CycleGAN is, if we are given with two sets of images X and Y (as shown above) and if we convert an image from set X (blue dot) to set Y (red dot) and then convert it back to set X then we should arrive where we started. If that doesn't happen then that loss can be termed as "cycle-consistancy loss", the models are trained to minimize this cycle-consistancy loss.

Some of the main applications of CycleGAN include:
1. Style Transfer
2. Object Transfiguration
3. Season Transfer
4. Photograph Generation From Paintings
5. Photograph Enhancement


<h2>Objective</h2>

This project deals with "Style Transfer" using GAN (rotation around center being the style). The main Objective of this project is to train and optimize a Generative Adversarial Network (CycleGAN) to:
1. Generate normal MNIST images from rotated MNIST image samples.
2. Generate rotated MNIST images from normal MNIST image samples.
