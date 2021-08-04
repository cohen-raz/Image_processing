# image_processing
### The School of Computer Science & Engineering at The Hebrew University of Jerusalem
This exercise deals with neural networks and their application to image restoration, implemented using [Keras](https://keras.io/).
In this exercise
I developed a general workflow for training networks to restore corrupted images, and then apply
this workflow on three different tasks:  
- image denoising 
- image deblurring.
- image super resolution.  
  
The network is based on the ResNet architecture, which builds on the principle of “skip connections” – combining the outputs of nonconsecutive layers. The basic building block of ResNet is the residual block, which for the input X it is defined as follows:
Let X be our input, we first feed X to a 3×3 convolution, followed by ReLU activation, then another
3×3 convolution and denote it’s output with O.
The final output of the residual block is ReLU(O + X), connecting the input to the last output, skipping over the middle layers.
![image](https://user-images.githubusercontent.com/83977654/128133044-c3006c2e-3769-4115-a1f0-f93fa5f6e465.png)
