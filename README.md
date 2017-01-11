# A Traffic Sign Classifier with Keras

This is a simple project which implements a Traffic Sign Classifier using a
Convolutional Neural Network - [LeNet5](http://yann.lecun.com/exdb/lenet/) Architecture.

The purpose of the project was to get familiar with [Keras](https://keras.io).

Sample data gathered from [The German Traffic Sign Recognition Benchmark](http://benchmark.ini.rub.de/?section=gtsrb&subsection=news).

[**Here the complete notebook**](traffic-sign-classification-with-keras.ipynb)

# Model Details

The network is made up of 6 hidden layers, one input layer and one output layer.

| Layer        | Type            | Size      | Filter Size   | Filter Stride | Padding |
|:------------:|:---------------:|:---------:|:-------------:|:-------------:|:-------:|
| **Input**    | -               | 32x32x3   | -             | -             | -       |
| **Hidden 1** | Convolutional   | 28x28x6   | 5x5           | 1             | `Valid` |
| **Hidden 2** | Max Pooling     | 14x14x6   | 2x2           | 2             | `Valid` |
| **Hidden 3** | Convolutional   | 10x10x16  | 5x5           | 1             | `Valid` |
| **Hidden 4** | Max Pooling     | 5x5x6     | 2x2           | 2             | `Valid` |
| **Hidden 5** | Fully Connected | 120       | -             | -             | -       |
| **Hidden 6** | Fully Connected | 84        | -             | -             | -       |
| **Output**   | Fully Connected | 43        | -             | -             | -       |

**Model Accuracy:** +90%
