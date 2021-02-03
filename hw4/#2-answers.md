
1. Name all the layers in the network, describe what they do.

  a. First layer is an input-layer with 24x24 input size - used to declare sizes of your input

  b. Next is a convolution layer with a filter size of 5, and 8 filters, and the stride is 1, padded with 2 pixels of zeros and the activation is relu. These layers performs valid convolutions and output a tensor. The purpose of convloution layers is transformations of input tensors into output tensors.             Every filter slides spatially along all x,y positions in the input tensor computing a single activation map, a sheet of activations in the output tensor.

  c. Next layer is a pooling layer - generally used to preserve the spatial resolution of the image. The size of the pool is 2x2 and striding at 2 cells 

  d. The next 2 layers are repetetion of hte above two with varying filtres and pool size.

  e. The last layer is a loss layer of type 'softmax' meant to output the result.

2. Experiment with the number and size of filters in each layer. Does it improve the accuracy?
 
  It improves the accuracy

3. Remove the pooling layers. Does it impact the accuracy?
 
 Interestingly, this also improved accuracy counter-intuitive to my expectation

4.Add one more conv layer. Does it help with accuracy?
  
  There is definitely an improvement with added layer of conv and pooling
  
5. Increase the batch size. What impact does it have?
 
  Batch size of 40 increased the accuracy


6. What is the best accuracy you can achieve? Are you over 99%? 99.5%?
![this](reslut.png).  

