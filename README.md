# ANLY590_FinalProject_Group01_StyleGAN

Group Members: Dian Zhi | Ruobing Yan | Muwen You | Zihang Weng | Hanshen Jing

**This project was based on the [Nvidia StyleGAN3](https://github.com/NVlabs/stylegan3) architecture**

Generative Adversarial Networks (GANs) are a deep-learning-based generative model. The GAN model architecture involves two sub-models: a generator model for generating 
new examples and a discriminator model for classifying whether generated examples are real or generated. In computer vision GANs are typically used for generating 
synthetic images from latent vectors. During the training, GAN will gradually learn the latent space and be able to reconstruct images using their latent vactors.

<!---StyleGAN is a special architecture of GAN model. Unlike traditional GANs, in which the GAN takes latent vectors directly into the generator at the input layer, styleGAN 
has a special component called *mapping network*. In StyleGAN, the latent vactors were first entered into the mapping network (which is composed by multiple fully 
connected layers) to generate a intermediate vector w (we view this as sort of a feature vector). The generator of StyleGAN takes a constant 4x4x512 matrix as input, and
try to scale up layer by layer. In each synthetic layer, the intermediate vector w was combined with generator's output via AdaIN function to make sure that the generated
image still have the features in the original image. This architecture of StyleGAN makes it easiler to change--->
