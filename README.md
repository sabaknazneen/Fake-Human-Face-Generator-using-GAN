# GAN-academic-project

In our project, we have tried to implement generative 
adversarial networks in a very classic way with new and 
latest tools and technologies. we are trying to implement 
our generative adversarial network to generate fake human 
faces. Our generator and discriminator will use the keras’s 
classic sequential modeling. 
We proposed to use two sequential models, one as a 
generator and another one as a discriminator to implement 
our generative adversarial model. For implementing the 
generator, we have used random noise as input data for the 
generator. We have also used the Batch Normalization 
technique and the Reshape module from the keras to resize 
the data and normalize to train the generator properly.  We 
have used the Leaky ReLU activation function for all the 
layers except the output layer; in the output layer we have 
used the tanh activation function for the output layer. We 
have also used the loss function as the binary cross-entropy 
for our generator model. 
Our generator will receive feedback data from the 
discriminator and based on the received feedback our 
generator will be updated. On the other hand, our 
discriminator is also implemented with the sequential 
model. However, the main difference between our 
generators is that after each epoch it does not learn, 
meaning it will not update or train after each epoch. Our 
discriminator’s main purpose is to identify the real and 
8 
fake image and give the feedback to the generator, so that 
we will use the sequential model. In our discriminator’s 
input data we have used both the generator produced data 
and the real image from the CelebA dataset and it takes 
both images and tries to identify the real and the fake 
image.  
Here, the model uses a total of four layers. As an input 
layer we have taken the generated data and the real image 
data and there are also two hidden dense layers along with 
an output layer which produce binary values. Other than 
the output layer we have used the Leaky ReLU activation 
function in our model and as our output will be 
classification type, so in the output layer we have used the 
sigmoid function. For the loss function in our model we 
have used the binary cross-entropy function.
