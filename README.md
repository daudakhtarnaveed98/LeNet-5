# LeNet-5
### The Dawn of Convulutional Neural Networks
This repository contains a slightly modified implementation of LeNet-5 CNN architecture which was proposed by Yann LeCun et al. (1998) in their [research paper][lenet-5-research-paper]. This network was used to recognize handwritten and machine printed characters and it outperformed all previous methods.

### Network Architecture
This network consists of five layers with learnable parameters and due to this it contains the digit 5 in its name. It contains three sets on convolutional and two sets of fully connected layers. After each convolutional layer there is a pooling layer as shown below.

![LeNet-5 Network Architecture](http://media5.datahacker.rs/2020/02/LeNet5-fm.png)

### Implementation & Modification Details
We will be implementing this network using PyTorch and TensorFlow with the following modifications:
- ReLU is used instead of tanh as an activation function for each layer hidden.
- Max pooling is used instead of average pooling.
- The dataset that we intend to use consists of 28x28x1 dimensional images, we will scale them to 32x32x1 before feeding to network.

### Dataset
This network will be trained on [Fashion-MNIST][fashion-mnist] dataset, it is a dataset consisting of 60,000 training and 10,000 testing images of 28x28x1 dimensions. It was created to serve as the replacement of original [MNIST][mnist] dataset.

### References
- [IEEE](https://ieeexplore.ieee.org/document/726791)

[lenet-5-research-paper]: <https://ieeexplore.ieee.org/document/726791>
[fashion-mnist]: <https://github.com/zalandoresearch/fashion-mnist>
[mnist]: <http://yann.lecun.com/exdb/mnist/>
