# Continous Variable Quantum MNIST Classifiers
## Classical and quantum hybrid circuits for classifying MNIST

This family of MNIST classifiers are classicial-quantum hybrid circuits using Keras and Pennylane. The quantum circuit is composed of a data encoding circuit and quantum neural network circuit as proposed in "Continuous variable quantum neural networks". https://arxiv.org/pdf/1806.06871v1.pdf The Pennylane-Tensorflow plug-in feature converts the quantum circuit into a Keras layer, and the whole network is treated as a Keras network, to which Keras' built in loss function and optimizer can be used for parameter updates.


