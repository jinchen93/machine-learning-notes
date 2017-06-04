# Artificial Neural Networks

First step is to scale the input data (normalizing the data).
This is not required but normalizing the data will make the learning process faster.

**Hidden layers** are the layers between the **input** and **output** layers.
  - Often called "deep belief networks"

<img src="https://qph.ec.quoracdn.net/main-qimg-6210d60dc3f01fc5d2c348776e95b2ef-c" alt="Neural network diagram" width="500" />

**Synapses** take a value from the input and multiply it by a weight. Result gets outputted to the neuron.
  - They are represented by the lines connecting the circles

**Neurons** take all of the results from their connected **synapses**, sums them up, then feeds the sum into an **activation function** (a sigmoid function).
  - They are represented by circles, (input layer circles are not neurons)

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/60/ArtificialNeuronModel_english.png/600px-ArtificialNeuronModel_english.png" alt="Diagram of an activation function" width="500" />

**Hyperparameters** are parameters that WE set up (input layer size, output layer size, hidden layer size).

Instead of passing inputs in **1 by 1**, we pass the inputs in as **matrices** so that we can pass in **multiple inputs at once**.
  - This speeds up the computation time tremendously.

For example our inputs are 2 dimensional inputs that come in like this:

[5, 3]
[5, 1]
[10, 2]

If we take [5, 3] through a cycle, we would have 2 input nodes.
If we have 3 neurons in our hidden layer, each neuron would have to sum up the result coming from the synapses like so:

<img src="https://raw.githubusercontent.com/jinchen93/machine-learning-notes/master/diagrams/synapse-results.png" alt="Synapse result diagram" width="500" />

In order to make this easier, we use matrix multiplication so we don't have to deal with inputs one by one.

<img src="https://github.com/jinchen93/machine-learning-notes/blob/master/diagrams/matrix-multiplication.png?raw=true" alt="Matrix multiplication example" width="500" />

This representation is commonly broken down into

### X * W(1) = Z(2)

### X (matrix of inputs)
### W(1) (matrix of weights)
### Z(2) (Activity of second layer)

Once we have Z(2), we need to apply the activation function to all of the entries in Z(2)

<img src="" alt="Diagram of activation functions being applied" />