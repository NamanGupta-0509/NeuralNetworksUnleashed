
# Artificial Neural Network from Scratch


## The Problem
In this problem, you are required to make a neural network to classify handwritten images, but the catch is
that you are NOT allowed to use any machine learning library like Sklearn, Pytorch or Tensorflow.
## Overview of Code

I tried to proceed using classes for 'Layer' and 'NeuralNetwork' so that there remains flexibility of adding new layers and change their parameters as well.

For example, while building the ann, we can add more layers by just ->

```
layer1 = Layer(784, 32, 'relu')
layer1.input = X_train
layer2 = Layer(32, 10, 'softmax')
layer_n = Layer(nodes_in, nodes_out, activation_function)    # Add this line
```

```
ann = NeuralNetwork()
ann.add_layer(layer1)
ann.add_layer(layer2)
ann.ass_layer(layer_n)     # Add this line

```

By just adding these 2 lines, we can add a new hidden layer to the model.
## Python Code

Find the google colab file here - 
https://colab.research.google.com/drive/1VX_gCFqFmcmodWGaZtDSW9Fj86ZHbUTt?usp=sharing
## Visualise It!

Prediction:  [5]   |   Label:  [5]

![](https://i.ibb.co/DRKkvgv/1st.png)


Prediction:  [6]   |   Label:  [5]

![](https://i.ibb.co/fHMGfPT/2nd.png)


Prediction:  [8]   |   Label:  [8]

![](https://i.ibb.co/k4PRdw6/3rd.png)

## Final Results

On training data:
```
Accuracy:  88.26 %
```
On testing data:
```
Accuracy:  88.71 %
```

As the accuracy on testing data does not deviate much from accuracy on training data, we can say that the model is not over-fitted. Also, the model is decently trained with ~ 90% accuracy.
## Thanks:)

