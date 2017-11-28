# Conditional-Analogy-GAN-keras

A keras implementation of CAGAN and its variants. 

[The Conditional Analogy GAN: Swapping Fashion Articles on People Images](https://arxiv.org/abs/1709.04695)  
 Nikolay Jetchev, Urs Bergmann

## Description
### [[Blog post]](https://shaoanlu.wordpress.com/2017/10/26/reimplement-conditional-anology-gan-in-keras/)

- [CAGAN](https://github.com/shaoanlu/Conditional-Analogy-GAN-keras/blob/master/CAGAN.ipynb): keras implementation of CAGAN  
 - [CAGAN-stackGANv2-256-covar-refiner-mixup](https://github.com/shaoanlu/Conditional-Analogy-GAN-keras/blob/master/CAGAN_stackGANv2-256-covar-refiner-mixup.ipynb): A CAGAN combines with StackGAN-v2.  

Hierarchy of dataset directory looks like:
```bash
./imgs
  /1 
    filename01_1.jpg
    filename02_1.jpg
    filename03_1.jpg
    ...
  /5 
    filename01_5.jpg
    filename02_5.jpg
    filename03_5.jpg
    ...
```
Folder `./imgs/1/` contains human images and `./imgs/5/` contains stand alone cloth images. A human/article pair should has same filename followed by `_1` and `_5` separately. 
 Please refer to Load Iamges section in jupyter notebooks.

## Requirements
- python 3
- keras 2.1.1
- TensorFlow 1.2.0

## Acknowledgments
Code borrows from [tjwei](https://github.com/tjwei/GANotebooks) and [titu1994](https://github.com/titu1994/Super-Resolution-using-Generative-Adversarial-Networks/). The generative network is adopted from [CycleGAN](https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix) with [Instance Normalization](https://github.com/farizrahman4u/keras-contrib/blob/master/keras_contrib/layers/normalization.py).

