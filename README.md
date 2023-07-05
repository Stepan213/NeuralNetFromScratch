# Building an image classification neural network from scratch.

I know all the stuff I need to know, but I don't really know what I am doing.

At first, I wanted to do a binary classification NN that would distinguish between our two cats, Julie and Steiner. However, that would add another challenge: dealing with a tiny dataset (~200 photos). Therefore, I am sticking with the classical MNIST handwritten digit classification.

## And so, where do I start? Rough architecture & training plan.

I have "a few" images of digits 0, 1, ... 9. Each image is B&W, 28x28 = 784 pixels. Now what.

Given my experience with TensorFlow, I consider it sufficient to plan for four layers in total: input layer (784 nodes), output layer (10 nodes), and two hidden layers.

In goes 784 numbers. Let's say the first hidden layer will have 256 neurons. So thats 256 784-variable functions, "preferably" non-linear. Getting flashbacks from my multivariable calculus rn, though no big deal.

The second hidden layer will be smaller, let's give it 64 neurons. Probably will use the same functions as the first hidden layer.

The output layer will consist of 10 neurons. Don't think I have more to say here rn. 

### What about the training?

I don't really know. Guess I will have to engineer my own backpropagation algo, yay. 

Should probbbly write smth more here, TODO.

## Getting & preparing the dataset

## The first hidden layer

There are 784 inputs to each node, no big deal. Each input will be multiplied by some weight, a bias will be added and then it will go through some activation function. Easy.

How to do this really? Perhaps a simple function. Guessing which input format will be best for my 784 values, a plain list will do. I will also store the weights and biases in a list. Were I inclined toward grandiloquence, I would bestow upon it the appellation of ‘vector’. Howsoever.

Lets initiate those weights and biases randomly at first. 

Activation function will be relu. I am yet to discover why is it more prefered than others. For now, I believe the cool guys on the internet know what they're saying.