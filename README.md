Argan-for-faithful-image-restoration
=============

### This is More results for our paper's Figure 3.
The images below are all images of BSDS 500 dataset.  
   

   
![Alt text](/results/result1.png "Optional title")  
(a) JPEG   
(b) ARGAN_mse(λ=0.00001)  
(c) ARGAN_t2(fidelity loss=mse, λ=0.0001)  
(d) ARGAN_base  
   

The λ in (b) is 10 times smaller than that in (c). Therefore, the effect of gan on (b) is much smaller then (c) and produces a result close to baseline.
But the PSNR of (b) and (c) are similar, and there are more natural details in (c). 
Looking at the enlarged image, (c) gives noise to the back of the grass and bird, but there is no unnecessary noise in the background. 
On the other hand, (b) has a more unnatural noise in back of the grass and bird and the background has unnecessary noise.
- - -
![Alt text](/results/result2.png "Optional title")  
(a) JPEG   
(b) ARGAN_mse(λ=0.00001)   
(c) ARGAN_t2(fidelity loss=mse, λ=0.0001)     
(d) ARGAN_base   
   
  
As in the above example, the λ in (c) is 10 times larger than in (b), but the psnr in (b) and (c) are almost the same and the details are better expressed in (c).
- - -  
### The above examples use fidelity loss as mse, while the following two examples use fidelity loss as vgg.   
   

![Alt text](/results/result3.png "Optional title")  
(a) JPEG   
(b) ARGAN_vgg(λ=0.00001)  
(c) ARGAN_t2(fidelity loss=vgg, λ=0.00001)  
(d) ARGAN_base  
   

When using fidelity loss as vgg, the results have similar psnr even though the λ of ARGAN_vgg and ARGAN_t2 is equal to 0.00001. But ARGAN_t2(c) has a more natural detail. 
The texture of the bark of tree (c) is more natural than (b).
  
- - -
![Alt text](/results/result4.png "Optional title")  
(a) JPEG     
(b) ARGAN_vgg(λ=0.00001)      
(c) ARGAN_t2(fidelity loss=vgg, λ=0.00001)   
(d) ARGAN_base  
   

Looking at the legs and snout of the turtle of (c), texture is created more finely than (b). 
- - -

