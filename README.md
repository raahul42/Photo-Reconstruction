# Photo Reconstruction

This was part of Deep Learning course in IIT Kgp. Link to the Kaggle challenge is [here](https://www.kaggle.com/competitions/photo-reconstruction)

## Reconstruction of photos by inpainting using a conditional GAN
Our photos are often damaged over the years, old artefacts and manuscripts, over time, get degraded, and certain parts of the image can go missing. Even in the digital domains, sometimes, due to network issues and unreliability in some regions, images may be missing parts or have lower resolutions. This challenge will focus on building models with the generative ability to reconstruct images' lost/damaged parts.

#### Input

    - Animal images (256 x 256) with missing sections (masks)
    - Missing sections are in the form of squares of 75 x 75, and exactly 2 are in each image.
    - Information about the masks will be provided

#### Output

    - Animal image reconstructed (256 x 256)

## Pix2Pix

We tried to build and train a conditional generative adversarial network (cGAN) called pix2pix that learns a mapping from input images to output images, as described in Image-to-image translation with conditional adversarial networks by [Isola et al. (2017)](https://arxiv.org/abs/1611.07004). pix2pix is not application specific—it can be applied to a wide range of tasks, including synthesizing photos from label maps, generating colorized photos from black and white images, turning Google Maps photos into aerial images, and even transforming sketches into photos.
