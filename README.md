# Optimized_Beta_VAE
β Variational Auto-Encoder(VAE) is a popular variation of VAE proposed to automate the learning process of factorized latent representation more efficiently without any supervision. A β value greater than 1 enforces the model to learn disentangled representation more accurately. Disentangled representations emerge when the right balance is found between information preservation (reconstruction cost as regularisation) and latent channel capacity restriction (β > 1). However, the optimal value of β is dataset dependent and varies from dataset to dataset. In this paper, we tried to learn beta values based on the loss function automatically. In this method, we assume the optimal β value exists within n beans above 1, and We employ a Reinforcement Learning (RL) based n-arm bandit, where each arm tries to estimate the bean with the lowest loss during the training process. The optimal β value is found by applying simulated annealing within each bean. Result analysis shows that our approach performs better image generation than normal VAE and β VAE with random β, but reconstruction performance is slightly lower than normal VAE.

## Code File

Md_Mahin_1900421_Project_Code.ipynb file contains the whole source code for the model.

## Sub Modules

  The whole code is devided into following sub modules as form of separete scripts:
  
  1. Initialize Functions to Generate Outputs: Contains all the output generating functions
  2. Initialize Device and Read Data: Contains device configuretion and takes data as input
  3. Create Model Architecture: An autoencoder model defined here
  4. Beta Optimizer VAE Training: The optimization procedure implemented here
  5. Beta Optimizer VAE Outputs: Generate different types of outputs
  
