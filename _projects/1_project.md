---
layout: page
title: A Scalable Framework for HH Neuronal Networks
description: Enables the simulation of customizable neural networks.
img: assets/img/3_neurons_diagram.png
importance: 1
category: Computational Biology
related_publications: true
---

Simulating biologically accurate neural networks is essential for neuroscientific research. The Hodgkin-Huxley model is an incredibly meaningful tool for modelling the action potential of a single neuron. However, investigation of mammalian brain function requires a more complex version of this modelling framework.

This project implements a scalable, adaptable and modular framework in Python that accurately simulates the activity of neurons in networks with distinct firing patterns and different types of coupling.

There are two parts to this project:
1. A reimplementation of the framework published by <a href='https://doi.org/10.1016/j.neucom.2022.04.115'>Giannari et al.</a> available in `reimplementation.ipynb`.
2. An extension of this framework that implements the stabilization of neuronal activity via <b>synaptic scaling</b> that the mammalian nervous system is known to employ. This is available in `synaptic_scaling_extension.ipynb`.

For an overview of the Jupyter Notebooks, please see the <a href="https://github.com/dbaitech/biol-382">project repository</a>. Feel free to download and rerun the notebooks with different numbers and types of neurons as well as different connection weights and view their simulation results.

For an in depth analysis and explanation, please see the <a href='https://github.com/dbaitech/academic-writing/blob/main/BIOL_382_Final_Report.pdf'>project report</a>.

Here are some example simulations:

### Reimplementation

The resulting simulations from `reimplementation.ipynb` for two different neuronal motifs: feedforward and feedback excitation. Notice how only Neuron 1 receives an input current and how the type of connection to Neuron 2 can influence both of their activities.

The feedforward network only sends the current from Neuron 1 to Neuron 2. However, the feedback network also has a connection back from Neuron 2 to Neuron 1 which causes its prolonged excitation.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/reimplemention_feedforward_network_block_time_50_dt_0_5.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/reimplemention_feedback_network_block_time_50_dt_0_3.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

### Synaptic Scaling Augmentation
We have the following network of neurons with only Neuron 1 receiving an input current.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3_neurons_diagram.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Without synaptic scaling, the feedback loop causes unrestrained bursting and increasing firing rates.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3_neurons_no_scaling.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3_neurons_fr_no_scaling.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

When applying synaptic scaling with a target firing rate of 5Hz, the network remains in a stable state.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3_neurons_with_scaling.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3_neurons_fr_with_scaling.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

For more examples and explanation, please see the <a href='https://github.com/dbaitech/academic-writing/blob/main/BIOL_382_Final_Report.pdf'>project report</a>.


