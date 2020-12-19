# EVA5-Phase1
# EVA5-S4 Assignment

I have incorporated the intuition of progressive channels expansion. 
1.  Starting with 8 channels -> 16 channels -> 32 channels.
2.  With every convolution step, a ReLU functions is applied to deepen the intensity of the features. We avoid the ReLU in the last layer, as we want to get both the items, the vaules which are dense and describe that the feature is present in that pixel and also the other negative values, which tells the netwrok that the feature is not present.
3.  Now we check if the GPU is available and if yes we use GPU else CPU 
4.  We read the model summary to calculate the number of parameters the model consists and work towards having <20000.
5.  Create a train set and test set, and download the MNIST data to each of them. Also, we assigne the batch size to 64 as studies indicate batch sizes should be between 8 and 128.
6.  We create the train and test functions:
  a.  Train function 
    1.  takes the data in batches as defined.
    2.  optimizer is set to zero so to zero the delta it has from previous iteration
    3.  we caluculate the train loss using nll - likelihood loss
    4.  Do a backward propogation
    5.  modify the optimizer 
  b.  Test function this gives us total test loss and accuracy 
 
 7. Used a SGD optimizer and for 20 iterations called the functions train and test. 

