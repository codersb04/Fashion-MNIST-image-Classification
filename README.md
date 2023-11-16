# Fashion-MNIST-image-Classification

## Task 
Build a deep learnin model to classify fashion MNIST images.</br>
Tool Used: Jupyter Notebook, Python</br>
Datset: Fashion MNIST dataset. Basic classification: Classify images of clothing https://www.tensorflow.org/tutorials/keras/classification

## Steps Involved
### Load the the dependencies
- Libraries necessary for the task:
  - tensorflow
  - Keras
  - numpy
  - matplotlib
- Load the Fashion MNIST Dataset from tensorflow
### Data processing
- Create a list containing the classes for the dataset. Total classes are 10, that are:</br>
  0 --> T-shirt/top </br>
1 --> Trouser</br>
2 --> Pullover</br>
3 --> Dress</br>
4 --> Coat</br>
5 --> Sandal</br>
6 --> Shirt</br>
7 --> Sneaker</br>
8 --> Bag</br>
9 --> Ankle boot
- Build a function to display the image using matplotlib library
- Standardize the data by dividing the X_train and X_test by 255
### Model Building using Artificial Neural Network
- With 1 input layer of shape 28,28
- 2 hidden layers
- 1 output layer with 10 neurons each representing one class
- Optimizer is 'SGD'
- Sparse Categorical Cross entropy used for loss and accuracy used as performance metrics
- The result is not that good
### Model Building using Convolutional Neural Network
- 1 CNN layer each containing:
  - 1 Convolution layer with 28 filters and window/kernel size of 3,3
  - 1 Max Pooling Layer with 2,2 strides
- 1 Dense Layer:
  - 1 layer for Flattenning the input
  - 2 hidden layer with 'relu' activation
  - 1 Output layer with 10 neurons each representing 1 class with activation 'softmax'
- Optimizer is 'SGD'
- Sparse Categorical Cross entropy used for loss and accuracy used as performance metrics
- CNN model gave better outcome than ANN model.
