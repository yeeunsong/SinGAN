# SinGAN
Using **SinGAN Style Transfer** for augmenting computer vision input data  

Done during 2021 Summer Internship in ETRI, Korea. Only parts of experiment are uploaded due to security issues.   
    
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
### 1. Effectiveness of SinGAN as augmenting dataset for computer vision   
  1) SinGAN is not applicable for artifacts (Most of the cases)
  2) Mostly SinGAN is applicable for creating natural datasets such as cancer cells, biologic tissue, and natural scenery.   
  3) By using 32GB memory GPU, SinGAN was able to produce 512 pixel random samples (takes about 4 to 5 hours). So if the researcher does not need a high-definition natural dataset, SinGAN is applicable. Since SinGAN only demands a single input data, we can use it for data augmentation.   
  4) However, for high-definition dataset such as dataset of biologic tissue and cells, SinGAN does not seem to be applicable. In this project, I failed to apply SinGAN for 1024 pixel data, resulting to 'CUDA out of memory'    
 
### 2. Effectiveness of SinGAN for Super Resolution   
  1) I zoomed a data of 512 pixel to 2048 pixel using Super Resolution of SinGAN. And compared it with the original dataset. I cannot show the output result due to security issues, however, the result was meaningful.      




## Reference   
https://github.com/tamarott/SinGAN (original reference for SinGAN)   
https://github.com/FriedRonaldo/SinGAN   
https://github.com/singulart/SinGAN (SinGAN for continuous training)    
