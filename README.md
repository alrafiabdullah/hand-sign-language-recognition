# Hand Sign Language Recognition

##

## Papers

1. [Hand sign language recognition using multi-view hand skeleton](https://www.sciencedirect.com/science/article/abs/pii/S0957417420301615)
2. [Deep convolutional neural networks fro sign language recognition](https://ieeexplore.ieee.org/abstract/document/8316344/)
3. [American Sign Language Recognition using Deep
   Learning and Computer Vision](https://ieeexplore.ieee.org/abstract/document/8622141)

##

## Findings

> From 1:

- In their model they used 3DCNN because it captures 5 dimensional video input spatio-temporal dynamics of hands better.

  - In my model, my image inputs are 4 dimensional so it works with 2DCNN.

- They used LSTM in the RGB videos.

  - Dimension mismatch.

##

> From 2:

- They took the outputs of Softmax and Max Pooling layer for their architecture.

  - I took the Logarithmic Softmax as output in my model. (16%-96%)

##

> From 3:

- Their model works well for videos with constant background

  - My image dataset doesn't have this limitation

##

## Model

My model class Net has these layers:

- 2 2DCNN
- 2 2DMaxPool
- 2 2D Batch Normalization
- 2 Fully Connected layer

> Dataset - Sign Lanuage MNIST [Link](https://www.kaggle.com/datamunge/sign-language-mnist)

- Train: 27455
- Test: 7172

## Output

- Total Epoch: 7
- Log Interval: 27455
- Average Loss: 0.0373
- Accuracy: 96%

##
