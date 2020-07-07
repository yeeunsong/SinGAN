# SinGAN
Using SinGAN Style Transfer for creating CV input data




# Used Environment   
python 3.6   
cudatoolkit 10.1   
pytorch 1.4.0   
torchvision 0.5.0


# Objectives for this Project  
By using SinGAN, I was trying to make Deep Learning Dataset using only 1 input data.   
By Style Transfer using SinGAN, it can create random samples for Deep Learning.   


# Result for this project
1. Effectiveness of SinGAN as creating dataset for DL   
  1) SinGAN is not applicable for artifacts (as seen in the pills result)   
  2) So mostly SinGAN is implemented for creating nature dataset such as cancer cells, biologic tissue, and natural scenery.   
  3) By using 32GB memory GPU. SinGAN is able to produce 512 pixel random samples (takes about 4 to 5 hours). So if the researcher does not need a high-definition natural dataset, SinGAN is applicable. Since SinGAN only demands a single input data, we can use it for data amplification.   
  4) However, for high-definition dataset such as dataset of biologic tissue and cells, SinGAN does not seem to be applicable. In this project, I failed for application of SinGAN for 1024 pixel data, resulting to 'CUDA out of memory'    
 
 2. Effectiveness of SinGAN for Super Resolution   
  1) I zoomed a data of 512 pixel to 2048 pixel using Super Resolution of SinGAN. And compared it with the original dataset. I cannot show the output result due to security issues, however, the result was meaningful.      




# Reference   
https://github.com/tamarott/SinGAN (original reference for SinGAN)   
https://github.com/FriedRonaldo/SinGAN   
https://github.com/singulart/SinGAN (SinGAN for continuous training)    
