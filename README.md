# AMAG
## Introduction
This is the webpage for paper "AMAG: Additive, Multiplicative and Adaptive Graph Neural Network For Forecasting Neural Activity," published in NeurIPS 2023.

Paper: 
[OpenReview](https://openreview.net/forum?id=7ntI4kcoqG) 

Dataset:
[Dataset](https://zenodo.org/doi/10.5281/zenodo.10139709)


AMAG addresses modeling neural population dynamics via the forecasting task and improves forecasting performance by including a prior embedded with Graph Neural network, which consists of pairwise neural unit interaction as a multivariate dynamic system. The method leverages additive and multiplicative message-passing operations analogous to the interactions in neuronal systems and adaptively learns the interaction among neural units to forecast their future activity. 

AMAG Features:

- AMAG can forecast neuron activity by using sample-dependent additive and multiplicative message-passing operations with a learnable adjacency matrix.
- AMAG learns the underlying spatial interactions on synthetic datasets and shows the importance of learning to forecast in discovering such interactions.
- We apply AMAG to four neural recording datasets and demonstrate its reliability in generating future neural activity while recovering the channel spatial proximity in the learned adjacency matrix and aligning neural trajectories in the latent space.

![image](https://github.com/christincha/AMAG/assets/27986186/0625055d-0619-4fec-bb72-af42edfbf12d)


## Adjacency Matrix Recovery with AMAG
We evaluate the ability of AMAG to recover the ground truth adjacency matrix of synthetic datasets and its dependency on tasks.
![image](https://github.com/christincha/AMAG/assets/27986186/535172d7-8fe0-4b09-8fda-d22a983f1a53)


## Forecasting Visualization on Four Monkey Datasets
We compare AMAG with baseline methods, including RNN-based, Transformer-based, and Graph-based methods for one-step forecasting and multi-step forecasting
#### One-step forecasting performance in R squared ($R\^2$), Correlation (Corr), and Mean Squared Error (MSE).
![image](https://github.com/christincha/AMAG/assets/27986186/3cb40c18-d32c-4f2f-881e-9ce7e3679d6c)

#### Multi-step forecasting performance in R squared ($R\^2$), Correlation (Corr), and Mean Squared Error (MSE).
![image](https://github.com/christincha/AMAG/assets/27986186/0da625b1-99d2-4676-9dd0-affee9b99c29)


#### Visualization of the forecasted signal of AMAG with the strongest baselines.
![image](https://github.com/christincha/AMAG/assets/27986186/49833ebb-47e9-4347-91a4-baade35fa7f7)


