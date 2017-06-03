# Artificial Neural Networks

First step is to scale the input data down to standardize.
This is not required but normalizing the data will make the learning process faster.

**Hidden layers** are the layers between the **input** and **output** layers.
  - Often called "deep belief networks"

<img src="https://qph.ec.quoracdn.net/main-qimg-6210d60dc3f01fc5d2c348776e95b2ef-c" alt="Neural network diagram" />

**Synapses** take a value from the input and multiply it by a weight. Result gets outputted to the neuron.
  - They are represented by the lines connecting the circles

**Neurons** take all of the results from their connected **synapses**, sums them up, then feeds the sum into an **activation function** (a sigmoid function).
  - They are represented by circles, (input layer circles are not neurons)

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/60/ArtificialNeuronModel_english.png/600px-ArtificialNeuronModel_english.png" alt="Diagram of an activation function" />

**Hyperparameters** are parameters that WE set up (input layer size, output layer size, hidden layer size).

Instead of passing inputs in **1 by 1**, we pass the inputs in as **matrices** so that we can pass in **multiple inputs at once**.
  - This speeds up the computation time tremendously.