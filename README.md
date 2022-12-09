# Deep-learning-with-PyTorch--CIFAR10-dataset
This is my first deep learning project with PyTorch. CIFAR10 dataset contains images of 10 different objects including plane, car, bird, cat, dog, frog, horse, ship, and 
truck. The goal is to create a neural network model to identify these images with a good accuracy.
The data consists of 3 channels (RGB) and 32x32 pixels so the dimension of our tensor is going to be 3x32x32. We have 50000 sample images in training set and 10000
in test set. 

About my model: consits of 2 convlolutional layesr after which we apply ReLu for non-linearity and MaxPool to reduce the size of input tensors. Next we have two linear layers with ReLU activation functions. The last layer is a linear layer outputing 10 classes (one estimated probability for each class from which we choose the maximum)

Optimizer and loss: I used stochastic gradient descent as optimize with lr of 0.001 and cross entropy loss as my loss function.

Trained the model for 30 epochs in batch size of 4. The final accuracy I obtained was 60%
