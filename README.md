# Neuro120finalproject
This repository contains four Colab-exported Python scripts for running the experiments and analyses for our final project in "Introduction to Computational Neuroscience" (Neuro120), titled "A Dendrite-Inspired Third Factor for Abstracted Hebbian Learning in ANNs". 
The project studies an accelerometer-gated Hebbian-Oja learning rule inspired by dendritic signals that are more responsive to increases in postsynaptic activity than to sustained activity alone.

## Files

 `pca.py` runs single-neuron ReLU-Oja/PCA simulations. Compares vanilla Oja, accelerometer-gated Oja (our modfied version), and magnitude-gated Oja on synthetic Gaussian data, fixed-input dynamics, and repeated-input streams.
 
`gatewithstablewindow.py` runs the synthetic stationary-tail stress test. It generates sequence data where the class depends on early onset order, sweeps tail lengths `[0, 5, 10, 20, 40, 80]`, and compares `hebbian`, `magnitude_gate`, `accel_gate`, and `backprop`. 

`gated_newton.py` runs optimizer-side experiments comparing SGD, SGD with momentum, damped Newton-CG, and gated damped Newton-CG on CIFAR-100 and Haxby. 

`failedgatedhebbian.py` runs the initial Hebbian MLP experiments on MNIST and CIFAR-100. Compares local Hebbian hidden-layer rules with a backprop baseline and includes diagnostic passes.

## Authors 

Vandie A. Dumaboc, Diego L. Gonzalez Gauss, Francesco Plastina
