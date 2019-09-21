# Single-Image-Super-Resolution-Using-a-Generative-Adversarial-Network (SRGAN)
To generate a super resolution image with 4x upscaling factors using Generative Adversarial Network from low resolution image


### Objective 
Despite the breakthroughs in accuracy and speed of single image super-resolution using faster and deeper convolutional neural networks, one central problem remains largely unsolved: how do we recover the finer texture details when we super-resolve at large upscaling factors? The behavior of optimization-based super-resolution methods is principally driven by the choice of the objective function.
Recent work has largely focused on minimizing the mean squared reconstruction error. The resulting estimates have high peak signal-to-noise ratios, but they are often lacking high-frequency details and are perceptually unsatisfying in the sense that they fail to match the fidelity expected at the higher resolution. SRGAN is a framework capable of inferring photo-realistic natural images for 4x4 upscaling factors. To achieve this, SRGAN uses a perceptual loss function, which consists of an adversarial loss and a content loss. The adversarial loss pushes the solution to the natural image manifold using a discriminator network that is trained to differentiate between the super-resolved images and original photo-realistic images. In addition, it uses a content loss motivated by perceptual similarity instead of similarity in pixel space. The deep residual network is able to recover photo-realistic textures from heavily downsampled images on public benchmarks. Extensive quality testing including metrics with a use of human opinion had shown that this approach generates more pleasant images. The goal of this project is to implement super-resolution model based on GAN and test quality of image reconstruction.

### Tools Used
Google Cloud Platform with NVIDIA Tesla P100 with n1-highmem-8 (8 vCPUs, 52 GB memory), Google Colaboratory with Tesla K80 GPU, Git, Jupyter Notebook

### Packages Used
Keras, Tensorflow, VGG19, InceptionResNet, numpy, pandas, matplotlib

### Results
* Quantitative Measurements:
![Quantitative Measurements](https://github.com/ravi-teja-sunkara/Single-Image-Super-Resolution-Using-a-Generative-Adversarial-Network/blob/master/Images/Quantitative%20Values.JPG)

* At 12000 epoch Generated images of Validation data using Pixel Shuffler:
![At 12000 epoch Generated images of Validation data using Pixel Shuffler](https://github.com/ravi-teja-sunkara/Single-Image-Super-Resolution-Using-a-Generative-Adversarial-Network/blob/master/Images/Combined%20Images%20of%20comparision.JPG)
