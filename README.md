# Building an image classification neural network from scratch.

I know all the stuff I need to know, but I don't really know what I am doing.

At first, I wanted to do a binary classification NN that would distinguish between our two cats, Julie and Steiner. However, that would add another challenge: dealing with a tiny dataset (~200 photos). Therefore, I am sticking with the classical MNIST handwritten digit classification.

## And so, where do I start?

I have "a few" images of digits 0, 1, ... 9. Each image is B&W, 28x28 = 784 pixels. Now what.

Given my experience with TensorFlow, I consider it sufficient to plan for four layers in total: input layer (784 nodes), output layer (10 nodes), and two hidden layers.