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

- They took the outputs of Softmax and Max Pooling later for their architecture.

  - I took the Logarithmic Softmax as output in my model. 16%-96%

##
