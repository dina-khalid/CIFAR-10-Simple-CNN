# CIFAR-10-Simple-CNN
### Context
Building and evaluating a Convolutional Neural Network (CNN) model for image classification.
### Dataset 
[CIFAR-10](https://www.cs.toronto.edu/~kriz/cifar.html) is a benchmark dataset consisting of 10 balanced classes for different objects
### Model
The model is inspired by Vgg but smaller and with little modification as the data isn't complex.
#### Trails:
- The 1st trial training the model with SGD and CE-loss:
    -  encountered an obvious overfitting training ACC > 90 while validation < 75 and oscillating matrices curves for validation (accuracy, precision, recall, and F1-score)
- 2nd trial change SGD to Adam:
    - The curves become smoother but still, we have an overfitting problem
  - 3rd trial adding Dropuout:
     - Overfitting problem solved, validation and test ACC: 80%, training Acc: 85% While the acc for each class is balanced.

### Suggestions to improve the results:
- Increase the number of nodes in the arch.
- Change data augmentation.
- Transfer learning.
- Try a different arch.
