# Continuous Variable Quantum MNIST Classifiers
## Classical and quantum hybrid circuits for classifying MNIST

This family of MNIST classifiers are classicial-quantum hybrid circuits using Keras and Pennylane. The quantum circuit is composed of a data encoding circuit and quantum neural network circuit as proposed in "Continuous variable quantum neural networks". https://arxiv.org/pdf/1806.06871v1.pdf The Pennylane-Tensorflow plug-in feature converts the quantum circuit into a Keras layer, and the whole network is treated as a Keras network, to which Keras' built in loss function and optimizer can be applied for parameter updates. Categorical crossentropy or Mean Squeared Error is used for loss function and Stochastic Gradient Descent is used for optimizer.

The architecture of the networks is shown below.

<img src="https://user-images.githubusercontent.com/22792633/158081935-d8f6976e-faae-4d96-847d-55a96b6bf427.png"  width=56% height=56%>

The main components of the hybrid network are a classicial feed-forward network, a data encoding circuit, and a quantum neural network circuit. By employing different numbers of qumodes and cutoff dimension, the network produces output vectors of desired size. They are interpreted as one-hot encoded labels which are then compared against the true labels.

The training loss and accuracy results are:

<img src="https://user-images.githubusercontent.com/22792633/159094360-2c1819eb-d744-41bf-bd69-b661df8df180.png" width=36% height=36%>
