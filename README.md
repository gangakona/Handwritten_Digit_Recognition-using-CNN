# Handwritten_Digit_Recognition-using-CNN
Handwritten digit recognition using Convolutional Neural Networks (CNNs) is a significant application in the field of computer vision and pattern recognition. This research explores the development and optimization of a CNN model for accurately classifying handwritten digits. The dataset used for training and evaluation is a collection of handwritten digits, such as the MNIST dataset, a benchmark dataset widely used for digit recognition tasks.

The proposed CNN architecture consists of multiple convolutional layers followed by pooling layers, which capture hierarchical features from the input images. Batch normalization and dropout layers are incorporated to enhance model generalization and prevent overfitting. The final fully connected layers process the learned features and produce predictions for each digit class.

The model is trained using Adam optimizer, and hyperparameter tuning is performed to achieve optimal performance. The evaluation metric used accuracy providing a comprehensive assessment of the model's performance. The experimental results demonstrate the effectiveness of the CNN model in achieving high accuracy in handwritten digit recognition tasks.

## Technologies used

- Python
- CNN
- Keras
- Tensorflow
  
## CNN Model

We will use [Sequential](https://www.tensorflow.org/api_docs/python/tf/keras/Sequential?version=stable) Keras model.

Then we will have two pairs of [Convolution2D](https://www.tensorflow.org/api_docs/python/tf/keras/layers/Conv2D?version=stable) and [MaxPooling2D layers](https://www.tensorflow.org/api_docs/python/tf/keras/layers/MaxPooling2D?version=stable). The MaxPooling layer acts as a sort of downsampling using max values in a region instead of averaging.

After that we will use [Flatten](https://www.tensorflow.org/api_docs/python/tf/keras/layers/Flatten?version=stable) layer to convert multidimensional parameters to vector.

The las layer will be a [Dense layer](https://www.tensorflow.org/api_docs/python/tf/keras/layers/Dense?version=stable) with 10 [Softmax](https://www.tensorflow.org/api_docs/python/tf/keras/activations/softmax?version=stable) outputs. The output represents the network guess. The 0-th output represents a probability that the input digit is 0, the 1-st output represents a probability that the input digit is 1 and so on..

![Screenshot (2)](https://github.com/gangakona/Handwritten_Digit_Recognition-using-CNN/assets/110378442/6b0e3c8a-f336-4ac9-8703-40b17f98a76f)

![](https://1drv.ms/i/c/4230590ad987414b/EXJxysC9M99CnjV0cuXLl5gBIQ_ng6uTveie8GqeS-1d0w?e=CgnIlV)
