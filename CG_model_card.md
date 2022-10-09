# Model Card

## Model Description

**Input:** 

The inputs of this model are 70,000 images of handwritten digits and their ground truth labels. The images are 28x28 pixel grayscale images (1 channel). The inputs have shape (28,28,1) and range (0.0, 1.0).

**Output:** 

The model outputs predictions of what it thinks the image is displaying. This is then compared to a ground truth to give a figure of accuracy for the model. The outputs have shape (10,) and range (0.0, 1.0).

**Model Architecture:** 

I have used PyTorch to create a Convolutional Neural Network with the following structure:
CONV -> RELU -> MAXPOOL -> CONV -> RELU -> MAXPOOL -> FULLY CONNECTED -> RELU -> FULLY CONNECTED

## Performance

The original model performs with a 96.75% accuracy of correctly classifying the handwritten digits. This is with a learning rate of 0.01 and 5 epochs. Following the hyperparameter tuning, the learning rate is changed to 0.0007 - all other hyperparameters are kept constant. This learning rate gives an accuracy of 98.23%.

## Limitations

This model is designed to work with grayscale inputs only. In order to modify it for colour images, we would have to alter several parameters within the CNN itself. With more time, it would be nice to alter the model.

## Trade-offs

Outline any trade-offs of your model, such as any circumstances where the model exhibits performance issues. 

This model could give greater accuracy with more epochs for training. However, this will also take longer. In future it would be interesting to try and modify the hyperparameter tuning code to simultaneously tune for a configuration of parameters rather than just one. For example, we could look at optimising the number of epochs relative to learning rate. In this model, we only looked at optimizing the learning rate. 
