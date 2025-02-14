# GAN Monet Project
Kaggle has an open competition which started in 2020 called, "I'm Something of a Painter Myself". The challenge asked participants to develop a GAN (Generative Adversarial Network) which creates images in the style of Claude Monet, who is a well-known French painter from the Impressionist period.

Generative Adversarial Network (GAN): GANs are comprised of a generator to create the image and a discriminator to identify the fake images. Usage of the discriminator in training the neural network helps to improve the quality of the images generated. Thus, our challenge is to develop a generator which can create realistic Monet images -- such that our discriminator cannot discern the difference between the real and fake Monet.

Nowadays, GANs can be used to create synthetic images, videos, songs, etc. -- whether these creations are used in the medical industry, entertainment, gaming, marketing or other industries.

Description of Datasets:

* Monet: The Monet dataset contains 300 color images which are 256 by 256 pixels of real Monet paintings in JPEG or TFRecord format with an alphanumeric identification number.
* Photo: The photo dataset consists of 7038 color photos which are 256 by 256 pixels also in JPEG or TFRecord format with an alphanumeric identification number.

Note: Both JPG and TFRecord formats are provided, but only one format is necessary for the GAN. The alphanumeric identification numbers of the images are not utilized in our models.

Citation: Amy Jang, Ana Sofia Uzsoy, and Phil Culliton. I’m Something of a Painter Myself. https://kaggle.com/competitions/gan-getting-started, 2020. Kaggle.

Project Approach: For this assignment, we are asked to utilize the Monet and photo datasets summarized above to generate fake Monet-stylized images and submit to the competition. To build the GAN, we follow a modified U-Net architecture originally documented in a research paper by Ronnenberg, Fischer and Brox titled, "U-Net: Convolutional Networks for Biomedical Image Segmentation". This architecture demonstrated good performance with small amounts of labeled images. Since we have 300 Monet images, this architecture appeared to be a good methodology for our project. More details on the architecture are provided below.

The images from our best performing GAN are submitted to the Kaggle competition page, where we screenshot the submission as asked for this project.
