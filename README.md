# Spiking-Neural-Network


This is the python implementation of hardware efficient spiking neural network. It includes the modified learning and prediction rules which could be realised on hardware and are enegry efficient. Aim is to develop a network which could be used for on-chip learning as well as prediction.

Spike-Time Dependent Plasticity (STDP) algorithm will be used to train the network.

The SNN model used in this work is the feed-forward network, each neuron is connected to
all the neurons in the next layer by a weighted connection, which means that the output signal
of a neuron has a different weighted potential contribution . Input neurons require spike trains
and input signals (stimuli) need to be encoded into spikes (typically, spike trains) to further
feed the SNN.

<p align="center">
  <img src="https://user-images.githubusercontent.com/61707225/129899204-84d1b05e-56e0-4081-9624-d4e5272ab32b.PNG" width="500"/>
</p>

## Network Elements
- Image Encoding: The encoding an image involves the conversion of the pixel values to spike train.
- Synapse: In an SNN, synapse is the weighted path for generated spikes from one neuron to the other connected neurons.
- Neuron: Neuron is the fundamental unit of an SNN. The input, hidden and output layers consist of several iterconnected neurons and this neuron emulates the classic leaky integrate-and-fire (LIF)model.


<p align="center">
  <img src="https://user-images.githubusercontent.com/61707225/129902655-ae66bf74-8609-4a8a-8c5a-3185e9ead473.PNG" width="600"/>
</p>

## Processing Workflow
The figure 3.4 delineates the work flow of the implemented code which together constitute the spiking neural network.
<p align="center">
  <img src="https://user-images.githubusercontent.com/61707225/129904617-3d0f7eca-2b29-4166-9d38-22f33fef04c5.PNG" width="500"/>
</p>

## Dataset 
The MNIST database of handwritten digits contains 60,000 and 10,000 training and test samples respectively. The digits have been size-normalized and centered in a fixed-size image.The data set is useful for learning techniques and pattern recognition testing on real-world data an it doesn’t a lot of pre-processing and formatting. Each image is of the size 28 x 28 Pixel.
