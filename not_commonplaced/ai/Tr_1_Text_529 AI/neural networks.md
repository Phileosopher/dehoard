
An artificial neural network represents the state of each neuron by a single number and the strength of each synapse by a single number.
In this model, each neuron updates its state at regular time steps by simply averaging together the inputs from all connected neurons, weighting them by the synaptic strengths, optionally adding a constant, and then applying what's called an activation function to the result to compute its next state.
The easiest way to use a neural network as a function is to make it feedforward, with information flowing only in one direction, plugging the input to the function into a layer of neurons at the top and extracting the output from a layer of neurons at the bottom.

Backpropagation retraces the steps in a neural net to identify the errors made in an initial processing of input data.

Convolutional networks: the neurons in each layer are only connected to groups of neurons in the next layer.
Recurrent networks: connections from each layer can loop back to an earlier layer.
