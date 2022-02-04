# Continous Variable Quantum MNIST Classifiers
## Classical and quantum hybrid circuits for classifying MNIST

This family of MNIST classifiers are classicial-quantum hybrid circuits using Keras and Pennylane. The quantum circuit is composed of a data encoding circuit and quantum neural network circuit as proposed in "Continuous variable quantum neural networks". https://arxiv.org/pdf/1806.06871v1.pdf The Pennylane-Tensorflow plug-in feature converts the quantum circuit into a Keras layer, and the whole network is treated as a Keras network, to which Keras' built in loss function and optimizer can be applied for parameter updates. Categorical crossentropy or Mean Squeared Error is used for loss function and Stochastic Gradient Descent is used for optimizer.

The architecture of the networks is shown below.

The training loss and accuracy results are:
                       loss     accuracy
2-qumode classifier:
3-qumode classifiers:
           8 classes:  0.0563.    
          10 classes:
4-qumode classifier:
5-qumode classifier:
6-qumode classifier:
7-qumode classifier:
8-qumode classifier:
