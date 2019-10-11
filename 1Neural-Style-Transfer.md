---
layout: post
title: Neural-Style-Transfer
description: Implementation of a Neural Netwrok to perform Style Transfer, using transfer learning of a VGG19 imagenet model 
image: https://github.com/VipinindKumar/Neural-Style-Transfer/raw/master/images/galmton-taj/generated_image.jpg
nav-menu: true
---

Implementation of a Neural Netwrok to perform Style Transfer, using transfer learning of a VGG19 imagenet model 

1. Create an Interactive session
2. load content image
3. load style image
4. add random noise to the content image, to create initial generated image
5. load pretrained model
6. build the tensorflow graph:
   * Run the content image through the model and compute the content cost
   * Run the style image through the model and compute the style cost
   * Compute the total cost
   * Define the optimizer and the learning rate
7. initialize the tensorflow graph and run it for no. of iterations while updating genrated image G at every step

<img src="https://github.com/VipinindKumar/Neural-Style-Transfer/raw/master/images/Taj_Mahal.jpeg" width="400" height="300"> <img src="https://github.com/VipinindKumar/Neural-Style-Transfer/raw/master/images/galmton-taj/generated_image.jpg"> <img src="https://github.com/VipinindKumar/Neural-Style-Transfer/raw/master/images/city-taj/generated_image.jpg"> 

* ### Style Image (images/galmpton-painting.jpg):
<img src="https://github.com/VipinindKumar/Neural-Style-Transfer/raw/master/images/galmpton-painting.jpg" width="500">

 * #### Content Image (images/delhi.jpg)
<img src="https://github.com/VipinindKumar/Neural-Style-Transfer/raw/master/images/delhi.jpg" width="400" height="300"> <img src="https://github.com/VipinindKumar/Neural-Style-Transfer/raw/master/images/galmpton-delhi/50.png"> <img src="https://github.com/VipinindKumar/Neural-Style-Transfer/raw/master/images/galmpton-delhi/generated_image.jpg">

 * #### Content Image (images/Lal_quila.jpg)
<img src="https://github.com/VipinindKumar/Neural-Style-Transfer/raw/master/images/Lal_quila.jpg" width="400" height="300"> <img src="https://github.com/VipinindKumar/Neural-Style-Transfer/raw/master/images/galmpton-lal/50.png"> <img src="https://github.com/VipinindKumar/Neural-Style-Transfer/raw/master/images/galmpton-lal/generated_image.jpg">


 * #### Content Image (images/Rashtrapati-bhavan.jpg)
<img src="https://github.com/VipinindKumar/Neural-Style-Transfer/raw/master/images/Rashtrapati-bhavan.jpg" width="400" height="300"> <img src="https://github.com/VipinindKumar/Neural-Style-Transfer/raw/master/images/galmpton-rashtrapati/50.png"> <img src="https://github.com/VipinindKumar/Neural-Style-Transfer/raw/master/images/galmpton-rashtrapati/generated_image.jpg">
