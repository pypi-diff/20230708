# Comparing `tmp/pydpm-5.0.0.tar.gz` & `tmp/pydpm-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydpm-5.0.0.tar", last modified: Wed Jul  5 12:42:15 2023, max compression
+gzip compressed data, was "pydpm-5.1.0.tar", last modified: Sat Jul  8 14:19:38 2023, max compression
```

## Comparing `pydpm-5.0.0.tar` & `pydpm-5.1.0.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.764184 pydpm-5.0.0/
--rw-r--r--   0 aaatk      (501) staff       (20)    10760 2023-06-13 13:06:25.000000 pydpm-5.0.0/LICENSE
--rw-r--r--   0 aaatk      (501) staff       (20)      737 2023-06-13 13:06:25.000000 pydpm-5.0.0/MANIFEST.in
--rw-r--r--   0 aaatk      (501) staff       (20)    15878 2023-07-05 12:42:15.763939 pydpm-5.0.0/PKG-INFO
--rw-r--r--   0 aaatk      (501) staff       (20)    15117 2023-07-03 06:42:50.000000 pydpm-5.0.0/README.md
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.740965 pydpm-5.0.0/pydpm/
--rw-r--r--   0 aaatk      (501) staff       (20)       42 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.742345 pydpm-5.0.0/pydpm/dataloader/
--rw-r--r--   0 aaatk      (501) staff       (20)       76 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/dataloader/__init__.py
--rw-r--r--   0 aaatk      (501) staff       (20)     9522 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/dataloader/graph_data.py
--rw-r--r--   0 aaatk      (501) staff       (20)     2439 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/dataloader/image_data.py
--rw-r--r--   0 aaatk      (501) staff       (20)    14198 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/dataloader/text_data.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.743129 pydpm-5.0.0/pydpm/example/
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.743354 pydpm-5.0.0/pydpm/example/Bayesian_PM/
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.744076 pydpm-5.0.0/pydpm/example/Bayesian_PM/Convolutional_Poisson_Gamma_Belief_Network/
--rw-r--r--   0 aaatk      (501) staff       (20)     5042 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Convolutional_Poisson_Gamma_Belief_Network/CPFA_Demo.py
--rw-r--r--   0 aaatk      (501) staff       (20)     5041 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Convolutional_Poisson_Gamma_Belief_Network/CPGBN_Demo.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Convolutional_Poisson_Gamma_Belief_Network/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.744351 pydpm-5.0.0/pydpm/example/Bayesian_PM/Deep_Poisson_Factor_Analysis/
--rw-r--r--   0 aaatk      (501) staff       (20)     3707 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Deep_Poisson_Factor_Analysis/DPFA_Demo.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Deep_Poisson_Factor_Analysis/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.744630 pydpm-5.0.0/pydpm/example/Bayesian_PM/Deep_Poisson_Gamma_Dynamic_System/
--rw-r--r--   0 aaatk      (501) staff       (20)     3495 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Deep_Poisson_Gamma_Dynamic_System/DPGDS_Demo.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Deep_Poisson_Gamma_Dynamic_System/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.744903 pydpm-5.0.0/pydpm/example/Bayesian_PM/Dirchilet_Belief_Network/
--rw-r--r--   0 aaatk      (501) staff       (20)     3601 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Dirchilet_Belief_Network/DirBN_Demo.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Dirchilet_Belief_Network/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.745157 pydpm-5.0.0/pydpm/example/Bayesian_PM/Factor_Analysis/
--rw-r--r--   0 aaatk      (501) staff       (20)     3203 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Factor_Analysis/FA_demo.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Factor_Analysis/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.745404 pydpm-5.0.0/pydpm/example/Bayesian_PM/Gaussian_Mixture_Model/
--rw-r--r--   0 aaatk      (501) staff       (20)     3031 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Gaussian_Mixture_Model/GMM_Demo.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Gaussian_Mixture_Model/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.745656 pydpm-5.0.0/pydpm/example/Bayesian_PM/Graph_Poisson_Gamma_Belief_Network/
--rw-r--r--   0 aaatk      (501) staff       (20)     3764 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Graph_Poisson_Gamma_Belief_Network/GPGBN_Demo.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Graph_Poisson_Gamma_Belief_Network/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.745901 pydpm-5.0.0/pydpm/example/Bayesian_PM/Latent_Dirchilet_Allocation/
--rw-r--r--   0 aaatk      (501) staff       (20)     3452 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Latent_Dirchilet_Allocation/LDA_Demo.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Latent_Dirchilet_Allocation/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.746151 pydpm-5.0.0/pydpm/example/Bayesian_PM/Multimodal_Poisson_Gamma_Belief_Network/
--rw-r--r--   0 aaatk      (501) staff       (20)     3562 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Multimodal_Poisson_Gamma_Belief_Network/MPGBN_Demo.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Multimodal_Poisson_Gamma_Belief_Network/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.746404 pydpm-5.0.0/pydpm/example/Bayesian_PM/Poisson_Factor_Analysis/
--rw-r--r--   0 aaatk      (501) staff       (20)     3502 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Poisson_Factor_Analysis/PFA_Demo.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Poisson_Factor_Analysis/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.746654 pydpm-5.0.0/pydpm/example/Bayesian_PM/Poisson_Gamma_Belief_Network/
--rw-r--r--   0 aaatk      (501) staff       (20)     3385 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Poisson_Gamma_Belief_Network/PGBN_Demo.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Poisson_Gamma_Belief_Network/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.746899 pydpm-5.0.0/pydpm/example/Bayesian_PM/Poisson_Gamma_Dynamic_System/
--rw-r--r--   0 aaatk      (501) staff       (20)     3378 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Poisson_Gamma_Dynamic_System/PGDS_Demo.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Poisson_Gamma_Dynamic_System/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.747212 pydpm-5.0.0/pydpm/example/Bayesian_PM/Word_Embeddings_Deep_Topic_Model/
--rw-r--r--   0 aaatk      (501) staff       (20)     5031 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Word_Embeddings_Deep_Topic_Model/WEDTM_Demo.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Word_Embeddings_Deep_Topic_Model/__init__.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.747327 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.747628 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Conditional_Variational_Auto-encoder/
--rw-r--r--   0 aaatk      (501) staff       (20)     3656 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Conditional_Variational_Auto-encoder/CVAE_Demo.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Conditional_Variational_Auto-encoder/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.748010 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Deep_Convolution_Generative_Adversarial_Networks/
--rw-r--r--   0 aaatk      (501) staff       (20)     4128 2023-06-20 09:14:03.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Deep_Convolution_Generative_Adversarial_Networks/DCGAN_Demo.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-20 09:14:03.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Deep_Convolution_Generative_Adversarial_Networks/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.748368 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Denoising_Diffusion_Probabilistic_Model/
--rw-r--r--   0 aaatk      (501) staff       (20)     4456 2023-06-19 15:17:43.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Denoising_Diffusion_Probabilistic_Model/DDPM_Demo.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Denoising_Diffusion_Probabilistic_Model/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.748625 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Generative_Adversarial_Network/
--rw-r--r--   0 aaatk      (501) staff       (20)     4275 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Generative_Adversarial_Network/GAN_Demo.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Generative_Adversarial_Network/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.748982 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Information_Maximizing_Generative_Adversarial_Nets/
--rw-r--r--   0 aaatk      (501) staff       (20)     4422 2023-06-20 09:13:57.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Information_Maximizing_Generative_Adversarial_Nets/InfoGAN_Demo.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-20 09:13:57.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Information_Maximizing_Generative_Adversarial_Nets/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.749234 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Normlizing_Flow/
--rw-r--r--   0 aaatk      (501) staff       (20)     3655 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Normlizing_Flow/NFlow_Demo.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Normlizing_Flow/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.749509 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Real_NVP/
--rw-r--r--   0 aaatk      (501) staff       (20)     4592 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Real_NVP/Real_NVP_Demo.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Real_NVP/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.749779 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Restricted_Boltzmann_Machine/
--rw-r--r--   0 aaatk      (501) staff       (20)     3459 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Restricted_Boltzmann_Machine/RBM_Demo.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Restricted_Boltzmann_Machine/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.750037 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Variational_Autoencoder/
--rw-r--r--   0 aaatk      (501) staff       (20)     3476 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Variational_Autoencoder/VAE_Demo.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Variational_Autoencoder/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.750292 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Wasserstein_Generative_Adversarial_Networks/
--rw-r--r--   0 aaatk      (501) staff       (20)     4242 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Wasserstein_Generative_Adversarial_Networks/WGAN_Demo.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Wasserstein_Generative_Adversarial_Networks/__init__.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.750410 pydpm-5.0.0/pydpm/example/Hybrid_PM/
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.750857 pydpm-5.0.0/pydpm/example/Hybrid_PM/Deep_Coupling_Embedding_Topic_Model/
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Deep_Coupling_Embedding_Topic_Model/__init__.py
--rw-r--r--   0 aaatk      (501) staff       (20)        5 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Deep_Coupling_Embedding_Topic_Model/dcETM.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.751179 pydpm-5.0.0/pydpm/example/Hybrid_PM/Generative_Text_Convolutional_Neural_Network/
--rw-r--r--   0 aaatk      (501) staff       (20)        5 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Generative_Text_Convolutional_Neural_Network/GTCNN.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Generative_Text_Convolutional_Neural_Network/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.751428 pydpm-5.0.0/pydpm/example/Hybrid_PM/HyperMiner/
--rw-r--r--   0 aaatk      (501) staff       (20)        5 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/HyperMiner/HyperMiner.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/HyperMiner/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.751703 pydpm-5.0.0/pydpm/example/Hybrid_PM/Knowledge_Aware_Bayesian_Deep_Topic_Model/
--rw-r--r--   0 aaatk      (501) staff       (20)        5 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Knowledge_Aware_Bayesian_Deep_Topic_Model/KG_ETM.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Knowledge_Aware_Bayesian_Deep_Topic_Model/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.751978 pydpm-5.0.0/pydpm/example/Hybrid_PM/Multimodal_Weibull_Variational_Autoencoder/
--rw-r--r--   0 aaatk      (501) staff       (20)        5 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Multimodal_Weibull_Variational_Autoencoder/MWVAE.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Multimodal_Weibull_Variational_Autoencoder/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.752333 pydpm-5.0.0/pydpm/example/Hybrid_PM/Sawtooth_Embedding_Topic_Model/
--rw-r--r--   0 aaatk      (501) staff       (20)     5693 2023-06-29 14:01:26.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Sawtooth_Embedding_Topic_Model/SawETM_Demo.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-29 08:47:14.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Sawtooth_Embedding_Topic_Model/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.752589 pydpm-5.0.0/pydpm/example/Hybrid_PM/TopicNet/
--rw-r--r--   0 aaatk      (501) staff       (20)        5 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/TopicNet/TopicNet.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/TopicNet/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.752840 pydpm-5.0.0/pydpm/example/Hybrid_PM/Variational_Edge_Parition_Graph_Neural_Network/
--rw-r--r--   0 aaatk      (501) staff       (20)        5 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Variational_Edge_Parition_Graph_Neural_Network/VEPM.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Variational_Edge_Parition_Graph_Neural_Network/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.753097 pydpm-5.0.0/pydpm/example/Hybrid_PM/Variational_Temporal_Deep_Generative_Model/
--rw-r--r--   0 aaatk      (501) staff       (20)        5 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Variational_Temporal_Deep_Generative_Model/RGBN.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Variational_Temporal_Deep_Generative_Model/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.753340 pydpm-5.0.0/pydpm/example/Hybrid_PM/Weibull_Graph_Attention_Autoencoder/
--rw-r--r--   0 aaatk      (501) staff       (20)     5972 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Weibull_Graph_Attention_Autoencoder/WGAAE_Demo.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Weibull_Graph_Attention_Autoencoder/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.753713 pydpm-5.0.0/pydpm/example/Hybrid_PM/Weibull_Hybrid_Autoencoding_Inference/
--rw-r--r--   0 aaatk      (501) staff       (20)     4975 2023-06-25 00:54:03.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Weibull_Hybrid_Autoencoding_Inference/WHAI_Demo.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Weibull_Hybrid_Autoencoding_Inference/__init__.py
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/__init__.py
--rw-r--r--   0 aaatk      (501) staff       (20)    10775 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Sampler_Demo.py
--rw-r--r--   0 aaatk      (501) staff       (20)     8970 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Sampler_Speed_Demo.py
--rw-r--r--   0 aaatk      (501) staff       (20)      249 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/__init__.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.755377 pydpm-5.0.0/pydpm/metric/
--rw-r--r--   0 aaatk      (501) staff       (20)      319 2023-06-29 08:50:03.000000 pydpm-5.0.0/pydpm/metric/__init__.py
--rw-r--r--   0 aaatk      (501) staff       (20)     1441 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/metric/accuracy.py
--rw-r--r--   0 aaatk      (501) staff       (20)     1974 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/metric/cluster_acc.py
--rw-r--r--   0 aaatk      (501) staff       (20)     2029 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/metric/normalized_mutual_information.py
--rw-r--r--   0 aaatk      (501) staff       (20)      839 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/metric/perplexity.py
--rw-r--r--   0 aaatk      (501) staff       (20)      694 2023-06-29 08:50:06.000000 pydpm-5.0.0/pydpm/metric/purity.py
--rw-r--r--   0 aaatk      (501) staff       (20)      526 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/metric/reconstruction.py
--rw-r--r--   0 aaatk      (501) staff       (20)     1894 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/metric/roc_score.py
--rw-r--r--   0 aaatk      (501) staff       (20)     4539 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/metric/topic_coherence.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.755798 pydpm-5.0.0/pydpm/model/
--rw-r--r--   0 aaatk      (501) staff       (20)     1092 2023-06-29 08:46:28.000000 pydpm-5.0.0/pydpm/model/__init__.py
--rw-r--r--   0 aaatk      (501) staff       (20)     1147 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/basic_model.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.758382 pydpm-5.0.0/pydpm/model/bayesian_pm/
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-25 00:54:03.000000 pydpm-5.0.0/pydpm/model/bayesian_pm/__init__.py
--rw-r--r--   0 aaatk      (501) staff       (20)    11914 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/bayesian_pm/cpfa.py
--rw-r--r--   0 aaatk      (501) staff       (20)    16836 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/bayesian_pm/cpgbn.py
--rw-r--r--   0 aaatk      (501) staff       (20)    23445 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/bayesian_pm/dirbn.py
--rw-r--r--   0 aaatk      (501) staff       (20)    19071 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/bayesian_pm/dpfa.py
--rw-r--r--   0 aaatk      (501) staff       (20)    21893 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/bayesian_pm/dpgds.py
--rw-r--r--   0 aaatk      (501) staff       (20)    12252 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/bayesian_pm/fa.py
--rw-r--r--   0 aaatk      (501) staff       (20)     7301 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/bayesian_pm/gmm.py
--rw-r--r--   0 aaatk      (501) staff       (20)    18916 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/bayesian_pm/gpgbn.py
--rw-r--r--   0 aaatk      (501) staff       (20)     7109 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/bayesian_pm/lda.py
--rw-r--r--   0 aaatk      (501) staff       (20)    15054 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/bayesian_pm/mpgbn.py
--rw-r--r--   0 aaatk      (501) staff       (20)     9739 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/bayesian_pm/pfa.py
--rw-r--r--   0 aaatk      (501) staff       (20)    13091 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/bayesian_pm/pgbn.py
--rw-r--r--   0 aaatk      (501) staff       (20)    13191 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/bayesian_pm/pgds.py
--rw-r--r--   0 aaatk      (501) staff       (20)    28141 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/bayesian_pm/wedtm.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.760678 pydpm-5.0.0/pydpm/model/deep_learning_pm/
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/deep_learning_pm/__init__.py
--rw-r--r--   0 aaatk      (501) staff       (20)    11910 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/deep_learning_pm/cvae.py
--rw-r--r--   0 aaatk      (501) staff       (20)     7028 2023-06-20 09:13:34.000000 pydpm-5.0.0/pydpm/model/deep_learning_pm/dcgan.py
--rw-r--r--   0 aaatk      (501) staff       (20)    17455 2023-06-19 15:18:07.000000 pydpm-5.0.0/pydpm/model/deep_learning_pm/ddpm.py
--rw-r--r--   0 aaatk      (501) staff       (20)     8445 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/deep_learning_pm/gan.py
--rw-r--r--   0 aaatk      (501) staff       (20)    10291 2023-06-20 09:13:21.000000 pydpm-5.0.0/pydpm/model/deep_learning_pm/infogan.py
--rw-r--r--   0 aaatk      (501) staff       (20)     8641 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/deep_learning_pm/nflow.py
--rw-r--r--   0 aaatk      (501) staff       (20)     4432 2023-06-19 15:18:18.000000 pydpm-5.0.0/pydpm/model/deep_learning_pm/rbm.py
--rw-r--r--   0 aaatk      (501) staff       (20)    46356 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/deep_learning_pm/realnvp.py
--rw-r--r--   0 aaatk      (501) staff       (20)    10819 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/deep_learning_pm/vae.py
--rw-r--r--   0 aaatk      (501) staff       (20)     8538 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/deep_learning_pm/wgan.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.761461 pydpm-5.0.0/pydpm/model/hybrid_pm/
--rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/hybrid_pm/__init__.py
--rw-r--r--   0 aaatk      (501) staff       (20)    14034 2023-06-29 14:01:20.000000 pydpm-5.0.0/pydpm/model/hybrid_pm/sawetm.py
--rw-r--r--   0 aaatk      (501) staff       (20)    27885 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/hybrid_pm/wgaae.py
--rw-r--r--   0 aaatk      (501) staff       (20)    25071 2023-06-25 00:54:03.000000 pydpm-5.0.0/pydpm/model/hybrid_pm/whai.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.763266 pydpm-5.0.0/pydpm/sampler/
--rw-r--r--   0 aaatk      (501) staff       (20)       40 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/sampler/__init__.py
--rw-r--r--   0 aaatk      (501) staff       (20)     2557 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/sampler/basic_sampler.py
--rw-r--r--   0 aaatk      (501) staff       (20)     2201 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/sampler/distribution_sampler_cpu.py
--rw-r--r--   0 aaatk      (501) staff       (20)    34864 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/sampler/distribution_sampler_gpu.py
--rw-r--r--   0 aaatk      (501) staff       (20)     3670 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/sampler/model_sampler_cpu.py
--rw-r--r--   0 aaatk      (501) staff       (20)    14868 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/sampler/model_sampler_gpu.py
--rw-r--r--   0 aaatk      (501) staff       (20)     3449 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/sampler/pre_process.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.763573 pydpm-5.0.0/pydpm/utils/
--rw-r--r--   0 aaatk      (501) staff       (20)       20 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/utils/__init__.py
--rw-r--r--   0 aaatk      (501) staff       (20)     1464 2023-06-20 09:12:52.000000 pydpm-5.0.0/pydpm/utils/utils.py
-drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.741570 pydpm-5.0.0/pydpm.egg-info/
--rw-r--r--   0 aaatk      (501) staff       (20)    15878 2023-07-05 12:42:15.000000 pydpm-5.0.0/pydpm.egg-info/PKG-INFO
--rw-r--r--   0 aaatk      (501) staff       (20)     7068 2023-07-05 12:42:15.000000 pydpm-5.0.0/pydpm.egg-info/SOURCES.txt
--rw-r--r--   0 aaatk      (501) staff       (20)        1 2023-07-05 12:42:15.000000 pydpm-5.0.0/pydpm.egg-info/dependency_links.txt
--rw-r--r--   0 aaatk      (501) staff       (20)        6 2023-07-05 12:42:15.000000 pydpm-5.0.0/pydpm.egg-info/top_level.txt
--rw-r--r--   0 aaatk      (501) staff       (20)       38 2023-07-05 12:42:15.764234 pydpm-5.0.0/setup.cfg
--rw-r--r--   0 aaatk      (501) staff       (20)     1103 2023-07-05 12:26:41.000000 pydpm-5.0.0/setup.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.023374 pydpm-5.1.0/
+-rw-r--r--   0 aaatk      (501) staff       (20)    10760 2023-07-08 14:16:38.000000 pydpm-5.1.0/LICENSE
+-rw-r--r--   0 aaatk      (501) staff       (20)      737 2023-07-08 14:16:38.000000 pydpm-5.1.0/MANIFEST.in
+-rw-r--r--   0 aaatk      (501) staff       (20)    15878 2023-07-08 14:19:38.023156 pydpm-5.1.0/PKG-INFO
+-rw-r--r--   0 aaatk      (501) staff       (20)    15117 2023-07-08 14:16:38.000000 pydpm-5.1.0/README.md
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.006209 pydpm-5.1.0/pydpm/
+-rw-r--r--   0 aaatk      (501) staff       (20)       42 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.007260 pydpm-5.1.0/pydpm/dataloader/
+-rw-r--r--   0 aaatk      (501) staff       (20)       76 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/dataloader/__init__.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     9522 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/dataloader/graph_data.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     2439 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/dataloader/image_data.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    14198 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/dataloader/text_data.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.007626 pydpm-5.1.0/pydpm/example/
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.007743 pydpm-5.1.0/pydpm/example/Bayesian_PM/
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.008113 pydpm-5.1.0/pydpm/example/Bayesian_PM/Convolutional_Poisson_Gamma_Belief_Network/
+-rw-r--r--   0 aaatk      (501) staff       (20)     5042 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Bayesian_PM/Convolutional_Poisson_Gamma_Belief_Network/CPFA_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     5041 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Bayesian_PM/Convolutional_Poisson_Gamma_Belief_Network/CPGBN_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Bayesian_PM/Convolutional_Poisson_Gamma_Belief_Network/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.008360 pydpm-5.1.0/pydpm/example/Bayesian_PM/Deep_Poisson_Factor_Analysis/
+-rw-r--r--   0 aaatk      (501) staff       (20)     3707 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Bayesian_PM/Deep_Poisson_Factor_Analysis/DPFA_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Bayesian_PM/Deep_Poisson_Factor_Analysis/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.008606 pydpm-5.1.0/pydpm/example/Bayesian_PM/Deep_Poisson_Gamma_Dynamic_System/
+-rw-r--r--   0 aaatk      (501) staff       (20)     3495 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Bayesian_PM/Deep_Poisson_Gamma_Dynamic_System/DPGDS_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Bayesian_PM/Deep_Poisson_Gamma_Dynamic_System/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.008837 pydpm-5.1.0/pydpm/example/Bayesian_PM/Dirchilet_Belief_Network/
+-rw-r--r--   0 aaatk      (501) staff       (20)     3601 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Bayesian_PM/Dirchilet_Belief_Network/DirBN_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Bayesian_PM/Dirchilet_Belief_Network/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.009056 pydpm-5.1.0/pydpm/example/Bayesian_PM/Factor_Analysis/
+-rw-r--r--   0 aaatk      (501) staff       (20)     3203 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Bayesian_PM/Factor_Analysis/FA_demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Bayesian_PM/Factor_Analysis/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.009277 pydpm-5.1.0/pydpm/example/Bayesian_PM/Gaussian_Mixture_Model/
+-rw-r--r--   0 aaatk      (501) staff       (20)     3031 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Bayesian_PM/Gaussian_Mixture_Model/GMM_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Bayesian_PM/Gaussian_Mixture_Model/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.009509 pydpm-5.1.0/pydpm/example/Bayesian_PM/Graph_Poisson_Gamma_Belief_Network/
+-rw-r--r--   0 aaatk      (501) staff       (20)     3764 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Bayesian_PM/Graph_Poisson_Gamma_Belief_Network/GPGBN_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Bayesian_PM/Graph_Poisson_Gamma_Belief_Network/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.009741 pydpm-5.1.0/pydpm/example/Bayesian_PM/Latent_Dirchilet_Allocation/
+-rw-r--r--   0 aaatk      (501) staff       (20)     3452 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Bayesian_PM/Latent_Dirchilet_Allocation/LDA_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Bayesian_PM/Latent_Dirchilet_Allocation/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.009965 pydpm-5.1.0/pydpm/example/Bayesian_PM/Multimodal_Poisson_Gamma_Belief_Network/
+-rw-r--r--   0 aaatk      (501) staff       (20)     3562 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Bayesian_PM/Multimodal_Poisson_Gamma_Belief_Network/MPGBN_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Bayesian_PM/Multimodal_Poisson_Gamma_Belief_Network/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.010180 pydpm-5.1.0/pydpm/example/Bayesian_PM/Poisson_Factor_Analysis/
+-rw-r--r--   0 aaatk      (501) staff       (20)     3502 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Bayesian_PM/Poisson_Factor_Analysis/PFA_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Bayesian_PM/Poisson_Factor_Analysis/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.010402 pydpm-5.1.0/pydpm/example/Bayesian_PM/Poisson_Gamma_Belief_Network/
+-rw-r--r--   0 aaatk      (501) staff       (20)     3385 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Bayesian_PM/Poisson_Gamma_Belief_Network/PGBN_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Bayesian_PM/Poisson_Gamma_Belief_Network/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.010617 pydpm-5.1.0/pydpm/example/Bayesian_PM/Poisson_Gamma_Dynamic_System/
+-rw-r--r--   0 aaatk      (501) staff       (20)     3378 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Bayesian_PM/Poisson_Gamma_Dynamic_System/PGDS_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Bayesian_PM/Poisson_Gamma_Dynamic_System/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.010837 pydpm-5.1.0/pydpm/example/Bayesian_PM/Word_Embeddings_Deep_Topic_Model/
+-rw-r--r--   0 aaatk      (501) staff       (20)     5031 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Bayesian_PM/Word_Embeddings_Deep_Topic_Model/WEDTM_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Bayesian_PM/Word_Embeddings_Deep_Topic_Model/__init__.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Bayesian_PM/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.010941 pydpm-5.1.0/pydpm/example/Deep_Learning_PM/
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.011163 pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Conditional_Variational_Auto-encoder/
+-rw-r--r--   0 aaatk      (501) staff       (20)     3656 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Conditional_Variational_Auto-encoder/CVAE_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Conditional_Variational_Auto-encoder/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.011391 pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Deep_Convolution_Generative_Adversarial_Networks/
+-rw-r--r--   0 aaatk      (501) staff       (20)     4128 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Deep_Convolution_Generative_Adversarial_Networks/DCGAN_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Deep_Convolution_Generative_Adversarial_Networks/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.011619 pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Denoising_Diffusion_Probabilistic_Model/
+-rw-r--r--   0 aaatk      (501) staff       (20)     4456 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Denoising_Diffusion_Probabilistic_Model/DDPM_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Denoising_Diffusion_Probabilistic_Model/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.011843 pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Generative_Adversarial_Network/
+-rw-r--r--   0 aaatk      (501) staff       (20)     4275 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Generative_Adversarial_Network/GAN_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Generative_Adversarial_Network/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.012068 pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Information_Maximizing_Generative_Adversarial_Nets/
+-rw-r--r--   0 aaatk      (501) staff       (20)     4422 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Information_Maximizing_Generative_Adversarial_Nets/InfoGAN_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Information_Maximizing_Generative_Adversarial_Nets/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.012292 pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Normlizing_Flow/
+-rw-r--r--   0 aaatk      (501) staff       (20)     3655 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Normlizing_Flow/NFlow_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Normlizing_Flow/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.012507 pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Real_NVP/
+-rw-r--r--   0 aaatk      (501) staff       (20)     4592 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Real_NVP/Real_NVP_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Real_NVP/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.012736 pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Restricted_Boltzmann_Machine/
+-rw-r--r--   0 aaatk      (501) staff       (20)     3459 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Restricted_Boltzmann_Machine/RBM_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Restricted_Boltzmann_Machine/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.012954 pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Variational_Autoencoder/
+-rw-r--r--   0 aaatk      (501) staff       (20)     3476 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Variational_Autoencoder/VAE_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Variational_Autoencoder/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.013177 pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Wasserstein_Generative_Adversarial_Networks/
+-rw-r--r--   0 aaatk      (501) staff       (20)     4242 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Wasserstein_Generative_Adversarial_Networks/WGAN_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Wasserstein_Generative_Adversarial_Networks/__init__.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Deep_Learning_PM/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.013280 pydpm-5.1.0/pydpm/example/Hybrid_PM/
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.013474 pydpm-5.1.0/pydpm/example/Hybrid_PM/Deep_Coupling_Embedding_Topic_Model/
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Hybrid_PM/Deep_Coupling_Embedding_Topic_Model/__init__.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        5 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Hybrid_PM/Deep_Coupling_Embedding_Topic_Model/dcETM.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.013718 pydpm-5.1.0/pydpm/example/Hybrid_PM/Generative_Text_Convolutional_Neural_Network/
+-rw-r--r--   0 aaatk      (501) staff       (20)        5 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Hybrid_PM/Generative_Text_Convolutional_Neural_Network/GTCNN.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Hybrid_PM/Generative_Text_Convolutional_Neural_Network/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.013941 pydpm-5.1.0/pydpm/example/Hybrid_PM/HyperMiner/
+-rw-r--r--   0 aaatk      (501) staff       (20)        5 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Hybrid_PM/HyperMiner/HyperMiner.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Hybrid_PM/HyperMiner/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.014160 pydpm-5.1.0/pydpm/example/Hybrid_PM/Knowledge_Aware_Bayesian_Deep_Topic_Model/
+-rw-r--r--   0 aaatk      (501) staff       (20)        5 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Hybrid_PM/Knowledge_Aware_Bayesian_Deep_Topic_Model/KG_ETM.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Hybrid_PM/Knowledge_Aware_Bayesian_Deep_Topic_Model/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.014380 pydpm-5.1.0/pydpm/example/Hybrid_PM/Multimodal_Weibull_Variational_Autoencoder/
+-rw-r--r--   0 aaatk      (501) staff       (20)        5 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Hybrid_PM/Multimodal_Weibull_Variational_Autoencoder/MWVAE.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Hybrid_PM/Multimodal_Weibull_Variational_Autoencoder/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.014597 pydpm-5.1.0/pydpm/example/Hybrid_PM/Sawtooth_Embedding_Topic_Model/
+-rw-r--r--   0 aaatk      (501) staff       (20)     5693 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Hybrid_PM/Sawtooth_Embedding_Topic_Model/SawETM_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Hybrid_PM/Sawtooth_Embedding_Topic_Model/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.014809 pydpm-5.1.0/pydpm/example/Hybrid_PM/TopicNet/
+-rw-r--r--   0 aaatk      (501) staff       (20)        5 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Hybrid_PM/TopicNet/TopicNet.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Hybrid_PM/TopicNet/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.015030 pydpm-5.1.0/pydpm/example/Hybrid_PM/Variational_Edge_Parition_Graph_Neural_Network/
+-rw-r--r--   0 aaatk      (501) staff       (20)        5 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Hybrid_PM/Variational_Edge_Parition_Graph_Neural_Network/VEPM.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Hybrid_PM/Variational_Edge_Parition_Graph_Neural_Network/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.015259 pydpm-5.1.0/pydpm/example/Hybrid_PM/Variational_Temporal_Deep_Generative_Model/
+-rw-r--r--   0 aaatk      (501) staff       (20)        5 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Hybrid_PM/Variational_Temporal_Deep_Generative_Model/RGBN.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Hybrid_PM/Variational_Temporal_Deep_Generative_Model/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.015483 pydpm-5.1.0/pydpm/example/Hybrid_PM/Weibull_Graph_Attention_Autoencoder/
+-rw-r--r--   0 aaatk      (501) staff       (20)     5972 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Hybrid_PM/Weibull_Graph_Attention_Autoencoder/WGAAE_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Hybrid_PM/Weibull_Graph_Attention_Autoencoder/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.015702 pydpm-5.1.0/pydpm/example/Hybrid_PM/Weibull_Hybrid_Autoencoding_Inference/
+-rw-r--r--   0 aaatk      (501) staff       (20)     4975 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Hybrid_PM/Weibull_Hybrid_Autoencoding_Inference/WHAI_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Hybrid_PM/Weibull_Hybrid_Autoencoding_Inference/__init__.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Hybrid_PM/__init__.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    10775 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Sampler_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     8970 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/Sampler_Speed_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)      249 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/example/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.017011 pydpm-5.1.0/pydpm/metric/
+-rw-r--r--   0 aaatk      (501) staff       (20)      319 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/metric/__init__.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     1441 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/metric/accuracy.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     1974 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/metric/cluster_acc.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     2029 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/metric/normalized_mutual_information.py
+-rw-r--r--   0 aaatk      (501) staff       (20)      839 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/metric/perplexity.py
+-rw-r--r--   0 aaatk      (501) staff       (20)      694 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/metric/purity.py
+-rw-r--r--   0 aaatk      (501) staff       (20)      526 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/metric/reconstruction.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     1894 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/metric/roc_score.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     4539 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/metric/topic_coherence.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.017295 pydpm-5.1.0/pydpm/model/
+-rw-r--r--   0 aaatk      (501) staff       (20)     1052 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/model/__init__.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     1147 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/model/basic_model.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.019462 pydpm-5.1.0/pydpm/model/bayesian_pm/
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/model/bayesian_pm/__init__.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    11914 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/model/bayesian_pm/cpfa.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    16836 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/model/bayesian_pm/cpgbn.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    23445 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/model/bayesian_pm/dirbn.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    19071 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/model/bayesian_pm/dpfa.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    21893 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/model/bayesian_pm/dpgds.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    12252 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/model/bayesian_pm/fa.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     7301 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/model/bayesian_pm/gmm.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    18916 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/model/bayesian_pm/gpgbn.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     7109 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/model/bayesian_pm/lda.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    15054 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/model/bayesian_pm/mpgbn.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     9739 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/model/bayesian_pm/pfa.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    13091 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/model/bayesian_pm/pgbn.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    13191 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/model/bayesian_pm/pgds.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    28141 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/model/bayesian_pm/wedtm.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.021111 pydpm-5.1.0/pydpm/model/deep_learning_pm/
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/model/deep_learning_pm/__init__.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    11910 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/model/deep_learning_pm/cvae.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     7028 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/model/deep_learning_pm/dcgan.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    17455 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/model/deep_learning_pm/ddpm.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     8445 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/model/deep_learning_pm/gan.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    10291 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/model/deep_learning_pm/infogan.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     8641 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/model/deep_learning_pm/nflow.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     4432 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/model/deep_learning_pm/rbm.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    46356 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/model/deep_learning_pm/realnvp.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    10819 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/model/deep_learning_pm/vae.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     8538 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/model/deep_learning_pm/wgan.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.021621 pydpm-5.1.0/pydpm/model/hybrid_pm/
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/model/hybrid_pm/__init__.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    14034 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/model/hybrid_pm/sawetm.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    27885 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/model/hybrid_pm/wgaae.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    25071 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/model/hybrid_pm/whai.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.022622 pydpm-5.1.0/pydpm/sampler/
+-rw-r--r--   0 aaatk      (501) staff       (20)       40 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/sampler/__init__.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     2557 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/sampler/basic_sampler.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     2201 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/sampler/distribution_sampler_cpu.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    34864 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/sampler/distribution_sampler_gpu.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     3670 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/sampler/model_sampler_cpu.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    14868 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/sampler/model_sampler_gpu.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     3449 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/sampler/pre_process.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.022911 pydpm-5.1.0/pydpm/utils/
+-rw-r--r--   0 aaatk      (501) staff       (20)       20 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/utils/__init__.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     1464 2023-07-08 14:16:39.000000 pydpm-5.1.0/pydpm/utils/utils.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-08 14:19:38.006742 pydpm-5.1.0/pydpm.egg-info/
+-rw-r--r--   0 aaatk      (501) staff       (20)    15878 2023-07-08 14:19:37.000000 pydpm-5.1.0/pydpm.egg-info/PKG-INFO
+-rw-r--r--   0 aaatk      (501) staff       (20)     7068 2023-07-08 14:19:38.000000 pydpm-5.1.0/pydpm.egg-info/SOURCES.txt
+-rw-r--r--   0 aaatk      (501) staff       (20)        1 2023-07-08 14:19:37.000000 pydpm-5.1.0/pydpm.egg-info/dependency_links.txt
+-rw-r--r--   0 aaatk      (501) staff       (20)        6 2023-07-08 14:19:37.000000 pydpm-5.1.0/pydpm.egg-info/top_level.txt
+-rw-r--r--   0 aaatk      (501) staff       (20)       38 2023-07-08 14:19:38.023421 pydpm-5.1.0/setup.cfg
+-rw-r--r--   0 aaatk      (501) staff       (20)     1103 2023-07-08 14:19:19.000000 pydpm-5.1.0/setup.py
```

### Comparing `pydpm-5.0.0/LICENSE` & `pydpm-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/MANIFEST.in` & `pydpm-5.1.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/PKG-INFO` & `pydpm-5.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydpm
-Version: 5.0.0
+Version: 5.1.0
 Summary: A python library focuses on constructing deep probabilistic models on GPU.
 Home-page: https://github.com/BoChenGroup/Pydpm
 Author: Chaojie Wang, Wei Zhao, Xinyang Liu, Jiawen Wu
 Author-email: xd_silly@163.com
 Maintainer: BoChenGroup
 Maintainer-email: 13279389260@163.com
 License: Apache License Version 2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pydpm Version: 5.0.0 Summary: A python library
+Metadata-Version: 2.1 Name: pydpm Version: 5.1.0 Summary: A python library
 focuses on constructing deep probabilistic models on GPU. Home-page: https://
 github.com/BoChenGroup/Pydpm Author: Chaojie Wang, Wei Zhao, Xinyang Liu,
 Jiawen Wu Author-email: xd_silly@163.com Maintainer: BoChenGroup Maintainer-
 email: 13279389260@163.com License: Apache License Version 2.0 Platform:
 Windows Platform: Linux Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
 Python :: 3 Classifier: Topic :: Software Development :: Libraries Requires:
```

### Comparing `pydpm-5.0.0/README.md` & `pydpm-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/dataloader/graph_data.py` & `pydpm-5.1.0/pydpm/dataloader/graph_data.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/dataloader/image_data.py` & `pydpm-5.1.0/pydpm/dataloader/image_data.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/dataloader/text_data.py` & `pydpm-5.1.0/pydpm/dataloader/text_data.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/example/Bayesian_PM/Convolutional_Poisson_Gamma_Belief_Network/CPFA_Demo.py` & `pydpm-5.1.0/pydpm/example/Bayesian_PM/Convolutional_Poisson_Gamma_Belief_Network/CPFA_Demo.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/example/Bayesian_PM/Convolutional_Poisson_Gamma_Belief_Network/CPGBN_Demo.py` & `pydpm-5.1.0/pydpm/example/Bayesian_PM/Convolutional_Poisson_Gamma_Belief_Network/CPGBN_Demo.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/example/Bayesian_PM/Deep_Poisson_Factor_Analysis/DPFA_Demo.py` & `pydpm-5.1.0/pydpm/example/Bayesian_PM/Deep_Poisson_Factor_Analysis/DPFA_Demo.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/example/Bayesian_PM/Deep_Poisson_Gamma_Dynamic_System/DPGDS_Demo.py` & `pydpm-5.1.0/pydpm/example/Bayesian_PM/Deep_Poisson_Gamma_Dynamic_System/DPGDS_Demo.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/example/Bayesian_PM/Dirchilet_Belief_Network/DirBN_Demo.py` & `pydpm-5.1.0/pydpm/example/Bayesian_PM/Dirchilet_Belief_Network/DirBN_Demo.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/example/Bayesian_PM/Factor_Analysis/FA_demo.py` & `pydpm-5.1.0/pydpm/example/Bayesian_PM/Factor_Analysis/FA_demo.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/example/Bayesian_PM/Gaussian_Mixture_Model/GMM_Demo.py` & `pydpm-5.1.0/pydpm/example/Bayesian_PM/Gaussian_Mixture_Model/GMM_Demo.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/example/Bayesian_PM/Graph_Poisson_Gamma_Belief_Network/GPGBN_Demo.py` & `pydpm-5.1.0/pydpm/example/Bayesian_PM/Graph_Poisson_Gamma_Belief_Network/GPGBN_Demo.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/example/Bayesian_PM/Latent_Dirchilet_Allocation/LDA_Demo.py` & `pydpm-5.1.0/pydpm/example/Bayesian_PM/Latent_Dirchilet_Allocation/LDA_Demo.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/example/Bayesian_PM/Multimodal_Poisson_Gamma_Belief_Network/MPGBN_Demo.py` & `pydpm-5.1.0/pydpm/example/Bayesian_PM/Multimodal_Poisson_Gamma_Belief_Network/MPGBN_Demo.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/example/Bayesian_PM/Poisson_Factor_Analysis/PFA_Demo.py` & `pydpm-5.1.0/pydpm/example/Bayesian_PM/Poisson_Factor_Analysis/PFA_Demo.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/example/Bayesian_PM/Poisson_Gamma_Belief_Network/PGBN_Demo.py` & `pydpm-5.1.0/pydpm/example/Bayesian_PM/Poisson_Gamma_Belief_Network/PGBN_Demo.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/example/Bayesian_PM/Poisson_Gamma_Dynamic_System/PGDS_Demo.py` & `pydpm-5.1.0/pydpm/example/Bayesian_PM/Poisson_Gamma_Dynamic_System/PGDS_Demo.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/example/Bayesian_PM/Word_Embeddings_Deep_Topic_Model/WEDTM_Demo.py` & `pydpm-5.1.0/pydpm/example/Bayesian_PM/Word_Embeddings_Deep_Topic_Model/WEDTM_Demo.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Conditional_Variational_Auto-encoder/CVAE_Demo.py` & `pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Conditional_Variational_Auto-encoder/CVAE_Demo.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Deep_Convolution_Generative_Adversarial_Networks/DCGAN_Demo.py` & `pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Deep_Convolution_Generative_Adversarial_Networks/DCGAN_Demo.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Denoising_Diffusion_Probabilistic_Model/DDPM_Demo.py` & `pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Denoising_Diffusion_Probabilistic_Model/DDPM_Demo.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Generative_Adversarial_Network/GAN_Demo.py` & `pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Generative_Adversarial_Network/GAN_Demo.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Information_Maximizing_Generative_Adversarial_Nets/InfoGAN_Demo.py` & `pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Information_Maximizing_Generative_Adversarial_Nets/InfoGAN_Demo.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Normlizing_Flow/NFlow_Demo.py` & `pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Normlizing_Flow/NFlow_Demo.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Real_NVP/Real_NVP_Demo.py` & `pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Real_NVP/Real_NVP_Demo.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Restricted_Boltzmann_Machine/RBM_Demo.py` & `pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Restricted_Boltzmann_Machine/RBM_Demo.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Variational_Autoencoder/VAE_Demo.py` & `pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Variational_Autoencoder/VAE_Demo.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Wasserstein_Generative_Adversarial_Networks/WGAN_Demo.py` & `pydpm-5.1.0/pydpm/example/Deep_Learning_PM/Wasserstein_Generative_Adversarial_Networks/WGAN_Demo.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/example/Hybrid_PM/Sawtooth_Embedding_Topic_Model/SawETM_Demo.py` & `pydpm-5.1.0/pydpm/example/Hybrid_PM/Sawtooth_Embedding_Topic_Model/SawETM_Demo.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/example/Hybrid_PM/Weibull_Graph_Attention_Autoencoder/WGAAE_Demo.py` & `pydpm-5.1.0/pydpm/example/Hybrid_PM/Weibull_Graph_Attention_Autoencoder/WGAAE_Demo.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/example/Hybrid_PM/Weibull_Hybrid_Autoencoding_Inference/WHAI_Demo.py` & `pydpm-5.1.0/pydpm/example/Hybrid_PM/Weibull_Hybrid_Autoencoding_Inference/WHAI_Demo.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/example/Sampler_Demo.py` & `pydpm-5.1.0/pydpm/example/Sampler_Demo.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/example/Sampler_Speed_Demo.py` & `pydpm-5.1.0/pydpm/example/Sampler_Speed_Demo.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/metric/accuracy.py` & `pydpm-5.1.0/pydpm/metric/accuracy.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/metric/cluster_acc.py` & `pydpm-5.1.0/pydpm/metric/cluster_acc.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/metric/normalized_mutual_information.py` & `pydpm-5.1.0/pydpm/metric/normalized_mutual_information.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/metric/perplexity.py` & `pydpm-5.1.0/pydpm/metric/perplexity.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/metric/purity.py` & `pydpm-5.1.0/pydpm/metric/purity.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/metric/reconstruction.py` & `pydpm-5.1.0/pydpm/metric/reconstruction.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/metric/roc_score.py` & `pydpm-5.1.0/pydpm/metric/roc_score.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/metric/topic_coherence.py` & `pydpm-5.1.0/pydpm/metric/topic_coherence.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/model/__init__.py` & `pydpm-5.1.0/pydpm/model/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,12 +18,11 @@
 from .deep_learning_pm.gan import GAN
 from .deep_learning_pm.wgan import WGAN
 from .deep_learning_pm.dcgan import DCGAN
 from .deep_learning_pm.infogan import InfoGAN
 from .deep_learning_pm.rbm import RBM
 from .deep_learning_pm.ddpm import DDPM
 from .deep_learning_pm.nflow import NFlow
-from .deep_learning_pm.fvae import fVAE
 from .deep_learning_pm.realnvp import RealNVP
 from .hybrid_pm.whai import WHAI
 from .hybrid_pm.wgaae import WGAAE
 from .hybrid_pm.sawetm import SawETM
```

### Comparing `pydpm-5.0.0/pydpm/model/basic_model.py` & `pydpm-5.1.0/pydpm/model/basic_model.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/model/bayesian_pm/cpfa.py` & `pydpm-5.1.0/pydpm/model/bayesian_pm/cpfa.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/model/bayesian_pm/cpgbn.py` & `pydpm-5.1.0/pydpm/model/bayesian_pm/cpgbn.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/model/bayesian_pm/dirbn.py` & `pydpm-5.1.0/pydpm/model/bayesian_pm/dirbn.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/model/bayesian_pm/dpfa.py` & `pydpm-5.1.0/pydpm/model/bayesian_pm/dpfa.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/model/bayesian_pm/dpgds.py` & `pydpm-5.1.0/pydpm/model/bayesian_pm/dpgds.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/model/bayesian_pm/fa.py` & `pydpm-5.1.0/pydpm/model/bayesian_pm/fa.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/model/bayesian_pm/gmm.py` & `pydpm-5.1.0/pydpm/model/bayesian_pm/gmm.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/model/bayesian_pm/gpgbn.py` & `pydpm-5.1.0/pydpm/model/bayesian_pm/gpgbn.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/model/bayesian_pm/lda.py` & `pydpm-5.1.0/pydpm/model/bayesian_pm/lda.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/model/bayesian_pm/mpgbn.py` & `pydpm-5.1.0/pydpm/model/bayesian_pm/mpgbn.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/model/bayesian_pm/pfa.py` & `pydpm-5.1.0/pydpm/model/bayesian_pm/pfa.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/model/bayesian_pm/pgbn.py` & `pydpm-5.1.0/pydpm/model/bayesian_pm/pgbn.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/model/bayesian_pm/pgds.py` & `pydpm-5.1.0/pydpm/model/bayesian_pm/pgds.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/model/bayesian_pm/wedtm.py` & `pydpm-5.1.0/pydpm/model/bayesian_pm/wedtm.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/model/deep_learning_pm/cvae.py` & `pydpm-5.1.0/pydpm/model/deep_learning_pm/cvae.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/model/deep_learning_pm/dcgan.py` & `pydpm-5.1.0/pydpm/model/deep_learning_pm/dcgan.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/model/deep_learning_pm/ddpm.py` & `pydpm-5.1.0/pydpm/model/deep_learning_pm/ddpm.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/model/deep_learning_pm/gan.py` & `pydpm-5.1.0/pydpm/model/deep_learning_pm/gan.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/model/deep_learning_pm/infogan.py` & `pydpm-5.1.0/pydpm/model/deep_learning_pm/infogan.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/model/deep_learning_pm/nflow.py` & `pydpm-5.1.0/pydpm/model/deep_learning_pm/nflow.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/model/deep_learning_pm/rbm.py` & `pydpm-5.1.0/pydpm/model/deep_learning_pm/rbm.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/model/deep_learning_pm/realnvp.py` & `pydpm-5.1.0/pydpm/model/deep_learning_pm/realnvp.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/model/deep_learning_pm/vae.py` & `pydpm-5.1.0/pydpm/model/deep_learning_pm/vae.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/model/deep_learning_pm/wgan.py` & `pydpm-5.1.0/pydpm/model/deep_learning_pm/wgan.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/model/hybrid_pm/sawetm.py` & `pydpm-5.1.0/pydpm/model/hybrid_pm/sawetm.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/model/hybrid_pm/wgaae.py` & `pydpm-5.1.0/pydpm/model/hybrid_pm/wgaae.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/model/hybrid_pm/whai.py` & `pydpm-5.1.0/pydpm/model/hybrid_pm/whai.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/sampler/basic_sampler.py` & `pydpm-5.1.0/pydpm/sampler/basic_sampler.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/sampler/distribution_sampler_cpu.py` & `pydpm-5.1.0/pydpm/sampler/distribution_sampler_cpu.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/sampler/distribution_sampler_gpu.py` & `pydpm-5.1.0/pydpm/sampler/distribution_sampler_gpu.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/sampler/model_sampler_cpu.py` & `pydpm-5.1.0/pydpm/sampler/model_sampler_cpu.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/sampler/model_sampler_gpu.py` & `pydpm-5.1.0/pydpm/sampler/model_sampler_gpu.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/sampler/pre_process.py` & `pydpm-5.1.0/pydpm/sampler/pre_process.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm/utils/utils.py` & `pydpm-5.1.0/pydpm/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/pydpm.egg-info/PKG-INFO` & `pydpm-5.1.0/pydpm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydpm
-Version: 5.0.0
+Version: 5.1.0
 Summary: A python library focuses on constructing deep probabilistic models on GPU.
 Home-page: https://github.com/BoChenGroup/Pydpm
 Author: Chaojie Wang, Wei Zhao, Xinyang Liu, Jiawen Wu
 Author-email: xd_silly@163.com
 Maintainer: BoChenGroup
 Maintainer-email: 13279389260@163.com
 License: Apache License Version 2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pydpm Version: 5.0.0 Summary: A python library
+Metadata-Version: 2.1 Name: pydpm Version: 5.1.0 Summary: A python library
 focuses on constructing deep probabilistic models on GPU. Home-page: https://
 github.com/BoChenGroup/Pydpm Author: Chaojie Wang, Wei Zhao, Xinyang Liu,
 Jiawen Wu Author-email: xd_silly@163.com Maintainer: BoChenGroup Maintainer-
 email: 13279389260@163.com License: Apache License Version 2.0 Platform:
 Windows Platform: Linux Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
 Python :: 3 Classifier: Topic :: Software Development :: Libraries Requires:
```

### Comparing `pydpm-5.0.0/pydpm.egg-info/SOURCES.txt` & `pydpm-5.1.0/pydpm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydpm-5.0.0/setup.py` & `pydpm-5.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 
 from setuptools import setup, find_packages
 
 
 setup(
     name='pydpm',
-    version='5.0.0',
+    version='5.1.0',
     description='A python library focuses on constructing deep probabilistic models on GPU.',
     py_modules=['pydpm'],
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Chaojie Wang, Wei Zhao, Xinyang Liu, Jiawen Wu',
     author_email='xd_silly@163.com',
     maintainer='BoChenGroup',
```

