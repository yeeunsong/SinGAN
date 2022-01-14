# SinGAN
Using **SinGAN Style Transfer** for augmenting computer vision input data  

Done during 2021 Summer Internship in ETRI, Korea. Only parts of experiment are uploaded due to security issues.
The below images are **randomly generated images** by SinGAN with 1 input image.
    
![cell_micro_images](https://user-images.githubusercontent.com/49232148/87889295-dc9fe800-ca6b-11ea-95fb-034c81078e8b.jpg)
![alt text](https://user-images.githubusercontent.com/49232148/87865634-dac61e00-c9b2-11ea-9c53-fa2be96acf8c.jpg)   


## Environment   
- python 3.6   
- cudatoolkit 10.1   
- pytorch 1.4.0   
- torchvision 0.5.0


## Objectives for this Project  
With SinGAN ([SinGAN official Github page](https://github.com/tamarott/SinGAN)), it is possible to train a generative model from a single natural image, and then generate random samples from the given image.      
In this project, performance study of SinGAN was conducted for the purpose of **augmenting computer vision input data using SinGAN**.    
By using style transfer of SinGAN, it is possible to create random samples using just single image, thereby making the data augmentation possible.   



## Result for this project
### Effectiveness of SinGAN as augmenting dataset for computer vision   
  1) SinGAN is not applicable for artifacts (Most of the cases). Mostly SinGAN is applicable for creating natural datasets such as cancer cells, biologic tissue, and natural scenery.   
  3) By using 32GB memory GPU, SinGAN was able to produce 512-pixel random samples (takes about 4 to 5 hours). However, it was not possible to produce 1024-pixel samples due to the lack of GPU memory. Therefore, to produce high-definition dataset such as biologic tissue and cells, much higher GPU memory is required.


## Reference   
https://github.com/tamarott/SinGAN (original reference for SinGAN)   
https://github.com/FriedRonaldo/SinGAN   
https://github.com/singulart/SinGAN (SinGAN for continuous training)    
