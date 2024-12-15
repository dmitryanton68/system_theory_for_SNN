# __Systems theory principles for investigating the spiking neural network trained with the Hebbian rule__   
The code illustrates the result reported at the [Neuroinformatics-2024](https://neuroinfo.ru/index.php/en/) conference and published in [Proceedings of conference](https://www.researchgate.net/publication/385349463_Systems_Theory_principles_for_investigating_the_spiking_neural_network_trained_with_the_Hebbian_rule).
***
### ARTICLE:   
Antonov, D.I. "Systems theory principles for investigating the spiking neural network trained with the Hebbian rule." Proceedings of XXVI International Conference on Artificial Neural Networks NEUROINFORMATICS-2024. MIPT (Moscow Institute of Physics and Technology). Moscow. Russia. 2024 October. pp. 33-42.   
***
Abstract: The article presents the results of research on the synaptic weights distribution obtained by applying a new local learning rule for spiking neural networks (SNNs). The developed method uses a combination of Hebbian rules: spike-time dependent plasticity (STDP) and long-term depression (all-LTD). The synaptic weights distribution of a 3-layer SNN trained according to the com-bined rule allowed, after training, to restructure the synaptic weights distribution of SNN based on the principles of Systems Theory.
***
__The code is written in Python 3.8 using the Brian 2.0 framework.__   
***
The SNN architecture used for the 2-layer case was described in our [previous paper](https://ieeexplore.ieee.org/document/10582358).
In this paper, a 3-layer architecture was used:    

![3-layer SNN architecture](3-layer_SNN_architecture.jpg)

The SNN was trained using the _"STDP+all-LTD"_ method, based on two biologically plausible learning rules: canonical Hebbian spike-timing-dependent plasticity (STDP) and all-time long-term depression (all-LTD).    
For a description of the _"STDP+all-LTD"_ method, see [code and description](https://github.com/dmitryanton68/learning_rule_STDP_all-LTD).       

The SNN was trained in 2 stages:    
- first, the synaptic group S1 was trained (_Preliminary_Model.ipynb_ file), then,    
- in the second stage, the synaptic group S4 was trained (_Model_STDP+all-LTD_ _ _(weights_plane+compression).ipynb_ file).