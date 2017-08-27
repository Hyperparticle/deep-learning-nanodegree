# Face Generation (Project 5)

Project 5 is the final project of the series, which involves training a Generative Adversarial Network (GAN) to generate new faces. GANs have two parts: a generator and a discriminator. A generator's goal is to generate fake images that fool the discriminator, and the discriminator's goal is to determine if an image is fake or real. I built a Deep Convolutional GAN (DCGAN), where both G and D were built with 3 convolutions and one fully connected layer. The network was trained on both the MNIST handwriting dataset and the CelebFaces dataset, images scaled down to sizes of 28x28.

In the end, the results were pretty good. Half the faces generated looked a bit wonky, but the other half looked quite like a normal face.
