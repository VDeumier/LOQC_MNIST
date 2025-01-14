# LOQC_MNIST

This repository has been create in the context of the Perceval Quest, a quantum computing challenge create by Quandela and Scaleway.

## Goal

The goal of this repository is to upgrade a neural network (NN) trained on the MNIST digit dataset by using Linear Optical Quantum Computing (LOQC). This approach aims to enhance the performance and capabilities of the neural network through quantum computing techniques.

## LOQC

The photonics algorithms are created using the Perceval library (see documentation here: https://perceval.quandela.net/docs/v0.11/index.html)

## How to run

It is easier to create a venv with the libraries from requirements.txt as I had trouble getting tensorflow to work with some versions of numpy, but the versions indicated in requirements.txt should work.

The classical algorithm I have chosen to improve with quantum computing is described in classic_conv_model.ipynb.\
The hybrid (classical and quantum) model is explained in hybrid_conv_model.ipynb.

In the modelparams folder are stored the parameters of the trained (1 epoch) model as well as relevant values.
In the current state, the model doesn't train well at all, but I hope to make it work by implementing SU(N) gates as well as upgrade the gradient calculations by using explicit formulas to make things faster. 
