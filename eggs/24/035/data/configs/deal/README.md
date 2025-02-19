## DEAL configuration files

This folder contains the config file for the DEAL (Data-Efficient Active Learning) scheme, which uses the uncertainty on the local environments provided by the GP as a way to identify a small set of non-redundant configurations from a trajectory (e.g. composed by high-uncertainty configurations). In particular, we use FLARE to train the GP.

Two settings are available in the `configs/deal/`:

* `deal-pretrain-dft.yaml`: the selection is made using a pre-trained GP model on DFT energies/forces, and performing the DFT calculations on-the-fly
* `deal-nodft.yaml`: train a model from scratch, using the MD energy/forces as labels, and only at the end perform the single-point calculations on the selected structures

These two strategies can deliver a very similar selection of the structures (see SI of the manuscript), but the second one is much faster as no DFT calculations are performed serially, but they can be done at the end in an embarassingly parallel way. 