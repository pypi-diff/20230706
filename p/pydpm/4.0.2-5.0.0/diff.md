# Comparing `tmp/pydpm-4.0.2.tar.gz` & `tmp/pydpm-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/dustone/aPycharmProjects/pycharm/PyDPM4.0.1/dist/.tmp-cuuvnfer/pydpm-4.0.2.tar", last modified: Sun Dec 11 12:57:14 2022, max compression
+gzip compressed data, was "pydpm-5.0.0.tar", last modified: Wed Jul  5 12:42:15 2023, max compression
```

## Comparing `pydpm-4.0.2.tar` & `pydpm-5.0.0.tar`

### file list

```diff
@@ -1,158 +1,189 @@
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.201456 pydpm-4.0.2/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)    10760 2022-12-10 06:45:57.000000 pydpm-4.0.2/LICENSE
--rw-rw-r--   0 dustone   (1000) dustone   (1000)      737 2022-12-10 06:45:57.000000 pydpm-4.0.2/MANIFEST.in
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     6117 2022-12-11 12:57:14.201456 pydpm-4.0.2/PKG-INFO
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     5356 2022-12-10 06:57:51.000000 pydpm-4.0.2/README.md
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.189456 pydpm-4.0.2/pydpm/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)       42 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/__init__.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.189456 pydpm-4.0.2/pydpm/dataloader/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)       76 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/dataloader/__init__.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     9338 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/dataloader/graph_data.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     2439 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/dataloader/image_data.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)    14198 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/dataloader/text_data.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.189456 pydpm-4.0.2/pydpm/example/
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.193456 pydpm-4.0.2/pydpm/example/Bayesian_GM/
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.193456 pydpm-4.0.2/pydpm/example/Bayesian_GM/Convolutional_Poisson_Gamma_Belief_Network/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     3800 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Bayesian_GM/Convolutional_Poisson_Gamma_Belief_Network/CPFA_Demo.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     3793 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Bayesian_GM/Convolutional_Poisson_Gamma_Belief_Network/CPGBN_Demo.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Bayesian_GM/Convolutional_Poisson_Gamma_Belief_Network/__init__.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.193456 pydpm-4.0.2/pydpm/example/Bayesian_GM/Deep_Poisson_Factor_Analysis/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     2468 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Bayesian_GM/Deep_Poisson_Factor_Analysis/DPFA_Demo.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Bayesian_GM/Deep_Poisson_Factor_Analysis/__init__.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.193456 pydpm-4.0.2/pydpm/example/Bayesian_GM/Deep_Poisson_Gamma_Dynamic_System/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     2282 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Bayesian_GM/Deep_Poisson_Gamma_Dynamic_System/DPGDS_Demo.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Bayesian_GM/Deep_Poisson_Gamma_Dynamic_System/__init__.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.193456 pydpm-4.0.2/pydpm/example/Bayesian_GM/Dirchilet_Belief_Network/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     2438 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Bayesian_GM/Dirchilet_Belief_Network/DirBN_Demo.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Bayesian_GM/Dirchilet_Belief_Network/__init__.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.193456 pydpm-4.0.2/pydpm/example/Bayesian_GM/Graph_Poisson_Gamma_Belief_Network/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     2573 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Bayesian_GM/Graph_Poisson_Gamma_Belief_Network/GPGBN_Demo.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Bayesian_GM/Graph_Poisson_Gamma_Belief_Network/__init__.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.193456 pydpm-4.0.2/pydpm/example/Bayesian_GM/Latent_Dirchilet_Allocation/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     2197 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Bayesian_GM/Latent_Dirchilet_Allocation/LDA_Demo.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Bayesian_GM/Latent_Dirchilet_Allocation/__init__.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.193456 pydpm-4.0.2/pydpm/example/Bayesian_GM/Multimodal_Poisson_Gamma_Belief_Network/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     2494 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Bayesian_GM/Multimodal_Poisson_Gamma_Belief_Network/MPGBN_Demo.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Bayesian_GM/Multimodal_Poisson_Gamma_Belief_Network/__init__.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.193456 pydpm-4.0.2/pydpm/example/Bayesian_GM/Poisson_Factor_Analysis/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     2334 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Bayesian_GM/Poisson_Factor_Analysis/PFA_Demo.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Bayesian_GM/Poisson_Factor_Analysis/__init__.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.193456 pydpm-4.0.2/pydpm/example/Bayesian_GM/Poisson_Gamma_Belief_Network/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     2199 2022-12-11 05:58:45.000000 pydpm-4.0.2/pydpm/example/Bayesian_GM/Poisson_Gamma_Belief_Network/PGBN_Demo.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Bayesian_GM/Poisson_Gamma_Belief_Network/__init__.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.193456 pydpm-4.0.2/pydpm/example/Bayesian_GM/Poisson_Gamma_Dynamic_System/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     2184 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Bayesian_GM/Poisson_Gamma_Dynamic_System/PGDS_Demo.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Bayesian_GM/Poisson_Gamma_Dynamic_System/__init__.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.193456 pydpm-4.0.2/pydpm/example/Bayesian_GM/Word_Embeddings_Deep_Topic_Model/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     3802 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Bayesian_GM/Word_Embeddings_Deep_Topic_Model/WEDTM_Demo.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Bayesian_GM/Word_Embeddings_Deep_Topic_Model/__init__.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Bayesian_GM/__init__.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.193456 pydpm-4.0.2/pydpm/example/Deep_Learning_GM/
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.193456 pydpm-4.0.2/pydpm/example/Deep_Learning_GM/Denoising_Diffusion_Probabilistic_Model/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        5 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Deep_Learning_GM/Denoising_Diffusion_Probabilistic_Model/DDPM.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Deep_Learning_GM/Denoising_Diffusion_Probabilistic_Model/__init__.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.193456 pydpm-4.0.2/pydpm/example/Deep_Learning_GM/Generative_Adversarial_Network/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     3040 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Deep_Learning_GM/Generative_Adversarial_Network/GAN_Demo.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Deep_Learning_GM/Generative_Adversarial_Network/__init__.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.193456 pydpm-4.0.2/pydpm/example/Deep_Learning_GM/Normlizing_Flow/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     3040 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Deep_Learning_GM/Normlizing_Flow/NF_Demo.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Deep_Learning_GM/Normlizing_Flow/__init__.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.193456 pydpm-4.0.2/pydpm/example/Deep_Learning_GM/Restricted_Boltzmann_Machine/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     1783 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Deep_Learning_GM/Restricted_Boltzmann_Machine/RBM_Demo.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Deep_Learning_GM/Restricted_Boltzmann_Machine/__init__.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.193456 pydpm-4.0.2/pydpm/example/Deep_Learning_GM/Variational_Autoencoder/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     2594 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Deep_Learning_GM/Variational_Autoencoder/VAE_Demo.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Deep_Learning_GM/Variational_Autoencoder/__init__.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Deep_Learning_GM/__init__.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.193456 pydpm-4.0.2/pydpm/example/Hybrid_GM/
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.193456 pydpm-4.0.2/pydpm/example/Hybrid_GM/Deep_Coupling_Embedding_Topic_Model/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Hybrid_GM/Deep_Coupling_Embedding_Topic_Model/__init__.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        5 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Hybrid_GM/Deep_Coupling_Embedding_Topic_Model/dcETM.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.193456 pydpm-4.0.2/pydpm/example/Hybrid_GM/Generative_Text_Convolutional_Neural_Network/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        5 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Hybrid_GM/Generative_Text_Convolutional_Neural_Network/GTCNN.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Hybrid_GM/Generative_Text_Convolutional_Neural_Network/__init__.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.193456 pydpm-4.0.2/pydpm/example/Hybrid_GM/HyperMiner/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        5 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Hybrid_GM/HyperMiner/HyperMiner.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Hybrid_GM/HyperMiner/__init__.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.193456 pydpm-4.0.2/pydpm/example/Hybrid_GM/Knowledge_Aware_Bayesian_Deep_Topic_Model/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        5 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Hybrid_GM/Knowledge_Aware_Bayesian_Deep_Topic_Model/KG_ETM.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Hybrid_GM/Knowledge_Aware_Bayesian_Deep_Topic_Model/__init__.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.193456 pydpm-4.0.2/pydpm/example/Hybrid_GM/Multimodal_Weibull_Variational_Autoencoder/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        5 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Hybrid_GM/Multimodal_Weibull_Variational_Autoencoder/MWVAE.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Hybrid_GM/Multimodal_Weibull_Variational_Autoencoder/__init__.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.193456 pydpm-4.0.2/pydpm/example/Hybrid_GM/Sawtooth_Embedding_Topic_Model/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        5 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Hybrid_GM/Sawtooth_Embedding_Topic_Model/SawETM.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Hybrid_GM/Sawtooth_Embedding_Topic_Model/__init__.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.193456 pydpm-4.0.2/pydpm/example/Hybrid_GM/TopicNet/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        5 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Hybrid_GM/TopicNet/TopicNet.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Hybrid_GM/TopicNet/__init__.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.197456 pydpm-4.0.2/pydpm/example/Hybrid_GM/Variational_Edge_Parition_Graph_Neural_Network/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        5 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Hybrid_GM/Variational_Edge_Parition_Graph_Neural_Network/VEPM.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Hybrid_GM/Variational_Edge_Parition_Graph_Neural_Network/__init__.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.197456 pydpm-4.0.2/pydpm/example/Hybrid_GM/Variational_Temporal_Deep_Generative_Model/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        5 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Hybrid_GM/Variational_Temporal_Deep_Generative_Model/RGBN.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Hybrid_GM/Variational_Temporal_Deep_Generative_Model/__init__.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.197456 pydpm-4.0.2/pydpm/example/Hybrid_GM/Weibull_Graph_Attention_Autoencoder/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     5590 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Hybrid_GM/Weibull_Graph_Attention_Autoencoder/WGAAE_Demo.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Hybrid_GM/Weibull_Graph_Attention_Autoencoder/__init__.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.197456 pydpm-4.0.2/pydpm/example/Hybrid_GM/Weibull_Hybrid_Autoencoding_Inference/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     4659 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Hybrid_GM/Weibull_Hybrid_Autoencoding_Inference/WHAI_Demo.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Hybrid_GM/Weibull_Hybrid_Autoencoding_Inference/__init__.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Hybrid_GM/__init__.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)    10775 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Sampler_Demo.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     8970 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/Sampler_Speed_Demo.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)      249 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/example/__init__.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.197456 pydpm-4.0.2/pydpm/metric/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)      292 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/metric/__init__.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     1441 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/metric/accuracy.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     1974 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/metric/cluster_acc.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     2029 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/metric/normalized_mutual_information.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)      839 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/metric/perplexity.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)      526 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/metric/reconstruction.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     1894 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/metric/roc_score.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     4539 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/metric/topic_coherence.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.197456 pydpm-4.0.2/pydpm/model/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)      655 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/model/__init__.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     1147 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/model/basic_model.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.197456 pydpm-4.0.2/pydpm/model/bayesian_gm/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-11 04:33:03.000000 pydpm-4.0.2/pydpm/model/bayesian_gm/__init__.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)    11900 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/model/bayesian_gm/cpfa.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)    16836 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/model/bayesian_gm/cpgbn.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)    23431 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/model/bayesian_gm/dirbn.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)    19071 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/model/bayesian_gm/dpfa.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)    21879 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/model/bayesian_gm/dpgds.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)    18902 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/model/bayesian_gm/gpgbn.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     7127 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/model/bayesian_gm/lda.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)    15040 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/model/bayesian_gm/mpgbn.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     9725 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/model/bayesian_gm/pfa.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)    13077 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/model/bayesian_gm/pgbn.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)    13177 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/model/bayesian_gm/pgds.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)    28127 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/model/bayesian_gm/wedtm.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.197456 pydpm-4.0.2/pydpm/model/deep_learning_gm/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-11 04:33:03.000000 pydpm-4.0.2/pydpm/model/deep_learning_gm/__init__.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     7726 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/model/deep_learning_gm/gan.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     3855 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/model/deep_learning_gm/rbm.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     9665 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/model/deep_learning_gm/vae.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.197456 pydpm-4.0.2/pydpm/model/hybrid_gm/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        0 2022-12-11 04:33:03.000000 pydpm-4.0.2/pydpm/model/hybrid_gm/__init__.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)    27885 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/model/hybrid_gm/wgaae.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)    24554 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/model/hybrid_gm/whai.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.197456 pydpm-4.0.2/pydpm/sampler/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)       40 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/sampler/__init__.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     2557 2022-12-11 06:16:00.000000 pydpm-4.0.2/pydpm/sampler/basic_sampler.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     2201 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/sampler/distribution_sampler_cpu.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)    34864 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/sampler/distribution_sampler_gpu.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     3670 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/sampler/model_sampler_cpu.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)    14868 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/sampler/model_sampler_gpu.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     3449 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/sampler/pre_process.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.197456 pydpm-4.0.2/pydpm/utils/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)       20 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/utils/__init__.py
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     1342 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm/utils/utils.py
-drwxrwxr-x   0 dustone   (1000) dustone   (1000)        0 2022-12-11 12:57:14.189456 pydpm-4.0.2/pydpm.egg-info/
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     6117 2022-12-11 12:57:14.000000 pydpm-4.0.2/pydpm.egg-info/PKG-INFO
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     5640 2022-12-11 12:57:14.000000 pydpm-4.0.2/pydpm.egg-info/SOURCES.txt
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        1 2022-12-11 12:57:14.000000 pydpm-4.0.2/pydpm.egg-info/dependency_links.txt
--rw-rw-r--   0 dustone   (1000) dustone   (1000)        6 2022-12-11 12:57:14.000000 pydpm-4.0.2/pydpm.egg-info/top_level.txt
--rw-rw-r--   0 dustone   (1000) dustone   (1000)    97937 2022-12-10 06:45:57.000000 pydpm-4.0.2/pydpm_framework.png
--rw-rw-r--   0 dustone   (1000) dustone   (1000)       38 2022-12-11 12:57:14.201456 pydpm-4.0.2/setup.cfg
--rw-rw-r--   0 dustone   (1000) dustone   (1000)     1103 2022-12-11 08:54:32.000000 pydpm-4.0.2/setup.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.764184 pydpm-5.0.0/
+-rw-r--r--   0 aaatk      (501) staff       (20)    10760 2023-06-13 13:06:25.000000 pydpm-5.0.0/LICENSE
+-rw-r--r--   0 aaatk      (501) staff       (20)      737 2023-06-13 13:06:25.000000 pydpm-5.0.0/MANIFEST.in
+-rw-r--r--   0 aaatk      (501) staff       (20)    15878 2023-07-05 12:42:15.763939 pydpm-5.0.0/PKG-INFO
+-rw-r--r--   0 aaatk      (501) staff       (20)    15117 2023-07-03 06:42:50.000000 pydpm-5.0.0/README.md
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.740965 pydpm-5.0.0/pydpm/
+-rw-r--r--   0 aaatk      (501) staff       (20)       42 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.742345 pydpm-5.0.0/pydpm/dataloader/
+-rw-r--r--   0 aaatk      (501) staff       (20)       76 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/dataloader/__init__.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     9522 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/dataloader/graph_data.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     2439 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/dataloader/image_data.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    14198 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/dataloader/text_data.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.743129 pydpm-5.0.0/pydpm/example/
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.743354 pydpm-5.0.0/pydpm/example/Bayesian_PM/
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.744076 pydpm-5.0.0/pydpm/example/Bayesian_PM/Convolutional_Poisson_Gamma_Belief_Network/
+-rw-r--r--   0 aaatk      (501) staff       (20)     5042 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Convolutional_Poisson_Gamma_Belief_Network/CPFA_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     5041 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Convolutional_Poisson_Gamma_Belief_Network/CPGBN_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Convolutional_Poisson_Gamma_Belief_Network/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.744351 pydpm-5.0.0/pydpm/example/Bayesian_PM/Deep_Poisson_Factor_Analysis/
+-rw-r--r--   0 aaatk      (501) staff       (20)     3707 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Deep_Poisson_Factor_Analysis/DPFA_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Deep_Poisson_Factor_Analysis/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.744630 pydpm-5.0.0/pydpm/example/Bayesian_PM/Deep_Poisson_Gamma_Dynamic_System/
+-rw-r--r--   0 aaatk      (501) staff       (20)     3495 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Deep_Poisson_Gamma_Dynamic_System/DPGDS_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Deep_Poisson_Gamma_Dynamic_System/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.744903 pydpm-5.0.0/pydpm/example/Bayesian_PM/Dirchilet_Belief_Network/
+-rw-r--r--   0 aaatk      (501) staff       (20)     3601 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Dirchilet_Belief_Network/DirBN_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Dirchilet_Belief_Network/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.745157 pydpm-5.0.0/pydpm/example/Bayesian_PM/Factor_Analysis/
+-rw-r--r--   0 aaatk      (501) staff       (20)     3203 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Factor_Analysis/FA_demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Factor_Analysis/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.745404 pydpm-5.0.0/pydpm/example/Bayesian_PM/Gaussian_Mixture_Model/
+-rw-r--r--   0 aaatk      (501) staff       (20)     3031 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Gaussian_Mixture_Model/GMM_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Gaussian_Mixture_Model/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.745656 pydpm-5.0.0/pydpm/example/Bayesian_PM/Graph_Poisson_Gamma_Belief_Network/
+-rw-r--r--   0 aaatk      (501) staff       (20)     3764 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Graph_Poisson_Gamma_Belief_Network/GPGBN_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Graph_Poisson_Gamma_Belief_Network/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.745901 pydpm-5.0.0/pydpm/example/Bayesian_PM/Latent_Dirchilet_Allocation/
+-rw-r--r--   0 aaatk      (501) staff       (20)     3452 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Latent_Dirchilet_Allocation/LDA_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Latent_Dirchilet_Allocation/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.746151 pydpm-5.0.0/pydpm/example/Bayesian_PM/Multimodal_Poisson_Gamma_Belief_Network/
+-rw-r--r--   0 aaatk      (501) staff       (20)     3562 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Multimodal_Poisson_Gamma_Belief_Network/MPGBN_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Multimodal_Poisson_Gamma_Belief_Network/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.746404 pydpm-5.0.0/pydpm/example/Bayesian_PM/Poisson_Factor_Analysis/
+-rw-r--r--   0 aaatk      (501) staff       (20)     3502 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Poisson_Factor_Analysis/PFA_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Poisson_Factor_Analysis/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.746654 pydpm-5.0.0/pydpm/example/Bayesian_PM/Poisson_Gamma_Belief_Network/
+-rw-r--r--   0 aaatk      (501) staff       (20)     3385 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Poisson_Gamma_Belief_Network/PGBN_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Poisson_Gamma_Belief_Network/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.746899 pydpm-5.0.0/pydpm/example/Bayesian_PM/Poisson_Gamma_Dynamic_System/
+-rw-r--r--   0 aaatk      (501) staff       (20)     3378 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Poisson_Gamma_Dynamic_System/PGDS_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Poisson_Gamma_Dynamic_System/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.747212 pydpm-5.0.0/pydpm/example/Bayesian_PM/Word_Embeddings_Deep_Topic_Model/
+-rw-r--r--   0 aaatk      (501) staff       (20)     5031 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Word_Embeddings_Deep_Topic_Model/WEDTM_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/Word_Embeddings_Deep_Topic_Model/__init__.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Bayesian_PM/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.747327 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.747628 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Conditional_Variational_Auto-encoder/
+-rw-r--r--   0 aaatk      (501) staff       (20)     3656 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Conditional_Variational_Auto-encoder/CVAE_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Conditional_Variational_Auto-encoder/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.748010 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Deep_Convolution_Generative_Adversarial_Networks/
+-rw-r--r--   0 aaatk      (501) staff       (20)     4128 2023-06-20 09:14:03.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Deep_Convolution_Generative_Adversarial_Networks/DCGAN_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-20 09:14:03.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Deep_Convolution_Generative_Adversarial_Networks/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.748368 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Denoising_Diffusion_Probabilistic_Model/
+-rw-r--r--   0 aaatk      (501) staff       (20)     4456 2023-06-19 15:17:43.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Denoising_Diffusion_Probabilistic_Model/DDPM_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Denoising_Diffusion_Probabilistic_Model/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.748625 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Generative_Adversarial_Network/
+-rw-r--r--   0 aaatk      (501) staff       (20)     4275 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Generative_Adversarial_Network/GAN_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Generative_Adversarial_Network/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.748982 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Information_Maximizing_Generative_Adversarial_Nets/
+-rw-r--r--   0 aaatk      (501) staff       (20)     4422 2023-06-20 09:13:57.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Information_Maximizing_Generative_Adversarial_Nets/InfoGAN_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-20 09:13:57.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Information_Maximizing_Generative_Adversarial_Nets/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.749234 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Normlizing_Flow/
+-rw-r--r--   0 aaatk      (501) staff       (20)     3655 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Normlizing_Flow/NFlow_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Normlizing_Flow/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.749509 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Real_NVP/
+-rw-r--r--   0 aaatk      (501) staff       (20)     4592 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Real_NVP/Real_NVP_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Real_NVP/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.749779 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Restricted_Boltzmann_Machine/
+-rw-r--r--   0 aaatk      (501) staff       (20)     3459 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Restricted_Boltzmann_Machine/RBM_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Restricted_Boltzmann_Machine/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.750037 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Variational_Autoencoder/
+-rw-r--r--   0 aaatk      (501) staff       (20)     3476 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Variational_Autoencoder/VAE_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Variational_Autoencoder/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.750292 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Wasserstein_Generative_Adversarial_Networks/
+-rw-r--r--   0 aaatk      (501) staff       (20)     4242 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Wasserstein_Generative_Adversarial_Networks/WGAN_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Wasserstein_Generative_Adversarial_Networks/__init__.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Deep_Learning_PM/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.750410 pydpm-5.0.0/pydpm/example/Hybrid_PM/
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.750857 pydpm-5.0.0/pydpm/example/Hybrid_PM/Deep_Coupling_Embedding_Topic_Model/
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Deep_Coupling_Embedding_Topic_Model/__init__.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        5 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Deep_Coupling_Embedding_Topic_Model/dcETM.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.751179 pydpm-5.0.0/pydpm/example/Hybrid_PM/Generative_Text_Convolutional_Neural_Network/
+-rw-r--r--   0 aaatk      (501) staff       (20)        5 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Generative_Text_Convolutional_Neural_Network/GTCNN.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Generative_Text_Convolutional_Neural_Network/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.751428 pydpm-5.0.0/pydpm/example/Hybrid_PM/HyperMiner/
+-rw-r--r--   0 aaatk      (501) staff       (20)        5 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/HyperMiner/HyperMiner.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/HyperMiner/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.751703 pydpm-5.0.0/pydpm/example/Hybrid_PM/Knowledge_Aware_Bayesian_Deep_Topic_Model/
+-rw-r--r--   0 aaatk      (501) staff       (20)        5 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Knowledge_Aware_Bayesian_Deep_Topic_Model/KG_ETM.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Knowledge_Aware_Bayesian_Deep_Topic_Model/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.751978 pydpm-5.0.0/pydpm/example/Hybrid_PM/Multimodal_Weibull_Variational_Autoencoder/
+-rw-r--r--   0 aaatk      (501) staff       (20)        5 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Multimodal_Weibull_Variational_Autoencoder/MWVAE.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Multimodal_Weibull_Variational_Autoencoder/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.752333 pydpm-5.0.0/pydpm/example/Hybrid_PM/Sawtooth_Embedding_Topic_Model/
+-rw-r--r--   0 aaatk      (501) staff       (20)     5693 2023-06-29 14:01:26.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Sawtooth_Embedding_Topic_Model/SawETM_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-29 08:47:14.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Sawtooth_Embedding_Topic_Model/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.752589 pydpm-5.0.0/pydpm/example/Hybrid_PM/TopicNet/
+-rw-r--r--   0 aaatk      (501) staff       (20)        5 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/TopicNet/TopicNet.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/TopicNet/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.752840 pydpm-5.0.0/pydpm/example/Hybrid_PM/Variational_Edge_Parition_Graph_Neural_Network/
+-rw-r--r--   0 aaatk      (501) staff       (20)        5 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Variational_Edge_Parition_Graph_Neural_Network/VEPM.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Variational_Edge_Parition_Graph_Neural_Network/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.753097 pydpm-5.0.0/pydpm/example/Hybrid_PM/Variational_Temporal_Deep_Generative_Model/
+-rw-r--r--   0 aaatk      (501) staff       (20)        5 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Variational_Temporal_Deep_Generative_Model/RGBN.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Variational_Temporal_Deep_Generative_Model/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.753340 pydpm-5.0.0/pydpm/example/Hybrid_PM/Weibull_Graph_Attention_Autoencoder/
+-rw-r--r--   0 aaatk      (501) staff       (20)     5972 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Weibull_Graph_Attention_Autoencoder/WGAAE_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Weibull_Graph_Attention_Autoencoder/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.753713 pydpm-5.0.0/pydpm/example/Hybrid_PM/Weibull_Hybrid_Autoencoding_Inference/
+-rw-r--r--   0 aaatk      (501) staff       (20)     4975 2023-06-25 00:54:03.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Weibull_Hybrid_Autoencoding_Inference/WHAI_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/Weibull_Hybrid_Autoencoding_Inference/__init__.py
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Hybrid_PM/__init__.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    10775 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Sampler_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     8970 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/Sampler_Speed_Demo.py
+-rw-r--r--   0 aaatk      (501) staff       (20)      249 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/example/__init__.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.755377 pydpm-5.0.0/pydpm/metric/
+-rw-r--r--   0 aaatk      (501) staff       (20)      319 2023-06-29 08:50:03.000000 pydpm-5.0.0/pydpm/metric/__init__.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     1441 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/metric/accuracy.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     1974 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/metric/cluster_acc.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     2029 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/metric/normalized_mutual_information.py
+-rw-r--r--   0 aaatk      (501) staff       (20)      839 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/metric/perplexity.py
+-rw-r--r--   0 aaatk      (501) staff       (20)      694 2023-06-29 08:50:06.000000 pydpm-5.0.0/pydpm/metric/purity.py
+-rw-r--r--   0 aaatk      (501) staff       (20)      526 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/metric/reconstruction.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     1894 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/metric/roc_score.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     4539 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/metric/topic_coherence.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.755798 pydpm-5.0.0/pydpm/model/
+-rw-r--r--   0 aaatk      (501) staff       (20)     1092 2023-06-29 08:46:28.000000 pydpm-5.0.0/pydpm/model/__init__.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     1147 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/basic_model.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.758382 pydpm-5.0.0/pydpm/model/bayesian_pm/
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-25 00:54:03.000000 pydpm-5.0.0/pydpm/model/bayesian_pm/__init__.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    11914 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/bayesian_pm/cpfa.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    16836 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/bayesian_pm/cpgbn.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    23445 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/bayesian_pm/dirbn.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    19071 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/bayesian_pm/dpfa.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    21893 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/bayesian_pm/dpgds.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    12252 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/bayesian_pm/fa.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     7301 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/bayesian_pm/gmm.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    18916 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/bayesian_pm/gpgbn.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     7109 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/bayesian_pm/lda.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    15054 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/bayesian_pm/mpgbn.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     9739 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/bayesian_pm/pfa.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    13091 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/bayesian_pm/pgbn.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    13191 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/bayesian_pm/pgds.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    28141 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/bayesian_pm/wedtm.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.760678 pydpm-5.0.0/pydpm/model/deep_learning_pm/
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/deep_learning_pm/__init__.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    11910 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/deep_learning_pm/cvae.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     7028 2023-06-20 09:13:34.000000 pydpm-5.0.0/pydpm/model/deep_learning_pm/dcgan.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    17455 2023-06-19 15:18:07.000000 pydpm-5.0.0/pydpm/model/deep_learning_pm/ddpm.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     8445 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/deep_learning_pm/gan.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    10291 2023-06-20 09:13:21.000000 pydpm-5.0.0/pydpm/model/deep_learning_pm/infogan.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     8641 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/deep_learning_pm/nflow.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     4432 2023-06-19 15:18:18.000000 pydpm-5.0.0/pydpm/model/deep_learning_pm/rbm.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    46356 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/deep_learning_pm/realnvp.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    10819 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/deep_learning_pm/vae.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     8538 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/deep_learning_pm/wgan.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.761461 pydpm-5.0.0/pydpm/model/hybrid_pm/
+-rw-r--r--   0 aaatk      (501) staff       (20)        0 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/hybrid_pm/__init__.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    14034 2023-06-29 14:01:20.000000 pydpm-5.0.0/pydpm/model/hybrid_pm/sawetm.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    27885 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/model/hybrid_pm/wgaae.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    25071 2023-06-25 00:54:03.000000 pydpm-5.0.0/pydpm/model/hybrid_pm/whai.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.763266 pydpm-5.0.0/pydpm/sampler/
+-rw-r--r--   0 aaatk      (501) staff       (20)       40 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/sampler/__init__.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     2557 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/sampler/basic_sampler.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     2201 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/sampler/distribution_sampler_cpu.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    34864 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/sampler/distribution_sampler_gpu.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     3670 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/sampler/model_sampler_cpu.py
+-rw-r--r--   0 aaatk      (501) staff       (20)    14868 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/sampler/model_sampler_gpu.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     3449 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/sampler/pre_process.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.763573 pydpm-5.0.0/pydpm/utils/
+-rw-r--r--   0 aaatk      (501) staff       (20)       20 2023-06-13 13:06:25.000000 pydpm-5.0.0/pydpm/utils/__init__.py
+-rw-r--r--   0 aaatk      (501) staff       (20)     1464 2023-06-20 09:12:52.000000 pydpm-5.0.0/pydpm/utils/utils.py
+drwxr-xr-x   0 aaatk      (501) staff       (20)        0 2023-07-05 12:42:15.741570 pydpm-5.0.0/pydpm.egg-info/
+-rw-r--r--   0 aaatk      (501) staff       (20)    15878 2023-07-05 12:42:15.000000 pydpm-5.0.0/pydpm.egg-info/PKG-INFO
+-rw-r--r--   0 aaatk      (501) staff       (20)     7068 2023-07-05 12:42:15.000000 pydpm-5.0.0/pydpm.egg-info/SOURCES.txt
+-rw-r--r--   0 aaatk      (501) staff       (20)        1 2023-07-05 12:42:15.000000 pydpm-5.0.0/pydpm.egg-info/dependency_links.txt
+-rw-r--r--   0 aaatk      (501) staff       (20)        6 2023-07-05 12:42:15.000000 pydpm-5.0.0/pydpm.egg-info/top_level.txt
+-rw-r--r--   0 aaatk      (501) staff       (20)       38 2023-07-05 12:42:15.764234 pydpm-5.0.0/setup.cfg
+-rw-r--r--   0 aaatk      (501) staff       (20)     1103 2023-07-05 12:26:41.000000 pydpm-5.0.0/setup.py
```

### Comparing `pydpm-4.0.2/LICENSE` & `pydpm-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydpm-4.0.2/MANIFEST.in` & `pydpm-5.0.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pydpm-4.0.2/pydpm/dataloader/graph_data.py` & `pydpm-5.0.0/pydpm/dataloader/graph_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,30 +25,35 @@
         graph[(np.arange(graph.shape[0]), np.arange(graph.shape[0]))] = 0
         graph[np.where(graph < threshold)] = 0
         if binary:
             graph[np.where(graph > threshold - 0.01)] = 1
 
         return graph
 
-    def graph_from_edges(self, edge_index, n_nodes, to_sparse=True):
+    def graph_from_edges(self, edge_index, n_nodes, to_tensor=False, to_sparse=True):
 
-        if to_sparse:
+        if to_tensor:
             sp_adj = SparseTensor(row=edge_index[0],
                                   col=edge_index[1],
                                   value=torch.ones(edge_index[0].shape[0], device=edge_index.device),
                                   sparse_sizes=(n_nodes, n_nodes))
-            adj = sp_adj.to_dense()
+            if not to_sparse:
+                adj = sp_adj.to_dense()
+                return adj
         else:
             row = edge_index[0].detach().cpu().numpy()
             col = edge_index[1].detach().cpu().numpy()
             data = np.ones_like(row)
             sp_adj = sp.coo_matrix((data, (row, col)), shape=(n_nodes, n_nodes))
-            adj = sp_adj.todense()
 
-        return sp_adj, adj
+            if not to_sparse:
+                adj = sp_adj.todense()
+                return adj
+
+        return sp_adj
 
     def edges_from_graph(self, adj, device, is_sparse=True):
 
         if is_sparse:
             edge_index = torch.empty((2, adj.row.shape[0]), dtype=torch.long, device=device)
             edge_index[0] = torch.tensor(adj.row, dtype=torch.long, device=device)
             edge_index[1] = torch.tensor(adj.col, dtype=torch.long, device=device)
@@ -69,15 +74,15 @@
             degree_mat_inv_sqrt = sp.diags(np.power(rowsum, -0.5).flatten())
             adj_normalized = adj_.dot(degree_mat_inv_sqrt).transpose().dot(degree_mat_inv_sqrt).tocoo()
         else:
             # TODO
             pass
         return adj_normalized
 
-    def graph_to_tuple(self, sparse_mx, is_sparse: True):
+    def graph_to_tuple(self, sparse_mx, is_sparse: bool = True):
         if not sp.isspmatrix_coo(sparse_mx):
             sparse_mx = sparse_mx.tocoo()
         coords = np.vstack((sparse_mx.row, sparse_mx.col)).transpose()
         values = sparse_mx.data
         shape = sparse_mx.shape
         return coords, values, shape
 
@@ -94,14 +99,15 @@
 
         prob = prob / prob.sum()
         return prob.detach().cpu().numpy()
 
     def subgraph_from_graph(self, sp_adj, sample_nodes, is_sparse=True):
         sp_csr_adj = sp_adj.tocsr()
         sample_adj = sp_csr_adj[sample_nodes, :][:, sample_nodes].tocoo()
+        # sample_adj = sample_adj.todense()
         sample_adj = SparseTensor.from_scipy(sample_adj).to_dense()
 
         return sample_adj
 
     def edges_split_from_graph(self, adj, is_sparse=True):
         # Function to build test set with 10% positive links
         # NOTE: Splits are randomized and results might slightly deviate from reported numbers in the paper.
@@ -110,17 +116,17 @@
         # Remove diagonal elements
         adj = adj - sp.dia_matrix((adj.diagonal()[np.newaxis, :], [0]), shape=adj.shape)
         adj.eliminate_zeros()
         # Check that diag is zero:
         assert np.diag(adj.todense()).sum() == 0
 
         adj_triu = sp.triu(adj)
-        adj_tuple = self.sparse_to_tuple(adj_triu)
+        adj_tuple = self.graph_to_tuple(adj_triu)
         edges = adj_tuple[0]
-        edges_all = self.sparse_to_tuple(adj)[0]
+        edges_all = self.graph_to_tuple(adj)[0]
         num_test = int(np.floor(edges.shape[0] / 10.))
         num_val = int(np.floor(edges.shape[0] / 20.))
 
         all_edge_idx = list(range(edges.shape[0]))
         np.random.seed(1)  # add by wcj
         np.random.shuffle(all_edge_idx)
         val_edge_idx = all_edge_idx[:num_val]
```

### Comparing `pydpm-4.0.2/pydpm/dataloader/image_data.py` & `pydpm-5.0.0/pydpm/dataloader/image_data.py`

 * *Files identical despite different names*

### Comparing `pydpm-4.0.2/pydpm/dataloader/text_data.py` & `pydpm-5.0.0/pydpm/dataloader/text_data.py`

 * *Files identical despite different names*

### Comparing `pydpm-4.0.2/pydpm/example/Bayesian_GM/Convolutional_Poisson_Gamma_Belief_Network/CPGBN_Demo.py` & `pydpm-5.0.0/pydpm/example/Bayesian_PM/Convolutional_Poisson_Gamma_Belief_Network/CPFA_Demo.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,70 @@
 """
-================================================
-Convolutional Poisson Gamma Belief Network Demo
+===========================================
+Convolutional Poisson Factor Analysis
 Chaojie Wang  Sucheng Xiao  Bo Chen  and  Mingyuan Zhou
 Published in International Conference on Machine Learning 2019
 
 ===========================================
 
 """
 
-# Author: Chaojie Wang <xd_silly@163.com>; Jiawen Wu <wjw19960807@163.com>
+# Author: Chaojie Wang <xd_silly@163.com>; Jiawen Wu <wjw19960807@163.com>; Wei Zhao <13279389260@163.com>
 # License: BSD-3-Clause
+
 import numpy as np
+import argparse
 import scipy.io as sio
 import _pickle as cPickle
-from pydpm.metric import ACC
-from pydpm.model import CPGBN
+
+from torch.utils.data import Dataset, DataLoader
 from torchtext.data.utils import get_tokenizer
 from torchtext.datasets import AG_NEWS
+
+from pydpm.model import CPFA
+from pydpm.metric import ACC
 from pydpm.dataloader.text_data import Text_Processer, build_vocab_from_iterator
 
+# =========================================== ArgumentParser ===================================================================== #
+parser = argparse.ArgumentParser()
+
+# device
+parser.add_argument("--device", type=str, default='gpu')
+
+# dataset
+parser.add_argument("--data_path", type=str, default='../../../dataset/', help="the path of loading data")
 
-# Load dataset (AG_NEWS from torchtext)
-train_iter, test_iter = AG_NEWS('../dataset/', split=('train', 'test'))
+# model
+parser.add_argument("--save_path", type=str, default='../../save_models', help="the path of saving model")
+parser.add_argument("--load_path", type=str, default='../../save_models/CPFA.npy', help="the path of loading model")
+
+parser.add_argument("--z_dim", type=int, default=200, help="dimensionality of the z latent space")
+
+# optim
+parser.add_argument("--num_epochs", type=int, default=100, help="number of epochs of training")
+
+args = parser.parse_args()
+
+# =========================================== Dataset ===================================================================== #
+# define transform for dataset and load orginal dataset
+# load dataset (AG_NEWS from torchtext)
+train_iter, test_iter = AG_NEWS(args.data_path, split=('train', 'test'))
 tokenizer = get_tokenizer("basic_english")
 
 # build vocabulary
 vocab = build_vocab_from_iterator(map(lambda x: tokenizer(x[1]), train_iter), specials=['<unk>', '<pad>', '<bos>', '<eos>'], special_first=True, max_tokens=5000)
 vocab.set_default_index(vocab['<unk>'])
 text_processer = Text_Processer(tokenizer=tokenizer, vocab=vocab)
 
 # Get train/test label and data_file(tokens) from data_iter and convert them into clean file
-# stop_words = ['<unk>']# Defined by customer, as musch as possible
 train_files, train_labels = text_processer.file_from_iter(train_iter, tokenizer=tokenizer)
 test_files, test_labels = text_processer.file_from_iter(test_iter, tokenizer=tokenizer)
 
 # Take part of dataset for convenience
-train_idxs = np.arange(5000)
+train_idxs = np.arange(3000)
 np.random.shuffle(train_idxs)
 train_files = [train_files[i] for i in train_idxs]
 train_labels = [train_labels[i] for i in train_idxs]
 
 test_idxs = np.arange(1000)
 np.random.shuffle(test_idxs)
 test_files = [test_files[i] for i in test_idxs]
@@ -48,30 +73,35 @@
 # ===================================== mode 1, sparse input ====================================== #
 # Build batch of word2index
 train_sparse_batch, train_labels = text_processer.word_index_from_file(train_files, train_labels, to_sparse=True)
 test_sparse_batch, test_labels = text_processer.word_index_from_file(test_files, test_labels, to_sparse=True)
 print('Data has been processed!')
 
 # create the model and deploy it on gpu or cpu
-model = CPGBN([200, 100, 50], 'gpu')
-
+model = CPFA(K=args.z_dim, device=args.device)
 model.initial(train_sparse_batch, is_sparse=True)  # use the shape of train_data to initialize the params of model
-train_local_params = model.train(train_sparse_batch, is_sparse=True, iter_all=100)
-train_local_params = model.test(train_sparse_batch, is_sparse=True, iter_all=100)
-test_local_params = model.test(test_sparse_batch, is_sparse=True, iter_all=100)
 
+# train and evaluation
+train_local_params = model.train(data=train_sparse_batch, is_sparse=True, num_epochs=args.num_epochs)
+train_local_params = model.test(data=train_sparse_batch, is_sparse=True, num_epochs=args.num_epochs)
+test_local_params = model.test(data=test_sparse_batch, is_sparse=True, num_epochs=args.num_epochs)
+
+# save the model after training
+model.save(args.save_path)
+# load the model
+model.load(args.load_path)
+
+# evaluate the model with classification accuracy
+# the demo accuracy can achieve 0.628
 train_theta = np.sum(np.sum(train_local_params.W_nk, axis=3), axis=2).T
 test_theta = np.sum(np.sum(test_local_params.W_nk, axis=3), axis=2).T
-
-# Score of test dataset's Theta: 0.631
 results = ACC(train_theta, test_theta, train_labels, test_labels, 'SVM')
-model.save()
 
-# # Customer dataset
 
+# # Use custom dataset
 # DATA = cPickle.load(open("../../dataset/TREC.pkl", "rb"), encoding='iso-8859-1')
 #
 # data_vab_list = DATA['Vocabulary']
 # data_vab_count_list = DATA['Vab_count']
 # data_vab_length = DATA['Vab_Size']
 # data_label = DATA['Label']
 # data_train_list = DATA['Train_Origin']
```

### Comparing `pydpm-4.0.2/pydpm/example/Bayesian_GM/Deep_Poisson_Gamma_Dynamic_System/DPGDS_Demo.py` & `pydpm-5.0.0/pydpm/example/Bayesian_PM/Latent_Dirchilet_Allocation/LDA_Demo.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,58 +1,88 @@
 """
 ===========================================
-Deep Poisson Gamma Dynamical Systems Demo
-Dandan Guo, Bo Chen and Hao Zhang
-Published in Neural Information Processing Systems 2018
+Latent Dirichlet Allocation
+David M.Blei  Andrew Y.Ng  and  Michael I.Jordan
+Published in Journal of Machine Learning 2003
 
 ===========================================
 
 """
 
 # Author: Chaojie Wang <xd_silly@163.com>; Jiawen Wu <wjw19960807@163.com>; Wei Zhao <13279389260@163.com>
 # License: BSD-3-Clause
 
+import os
 import numpy as np
+import argparse
 import scipy.io as sio
-
-from pydpm.metric import ACC
-from pydpm.model import DPGDS
+from tqdm import tqdm
 
 from torchvision import datasets, transforms
+
+from pydpm.model import LDA
+from pydpm.metric import ACC
 from pydpm.dataloader.image_data import tensor_transforms
 
-# load dataset
+# =========================================== ArgumentParser ===================================================================== #
+parser = argparse.ArgumentParser()
+
+# device
+parser.add_argument("--device", type=str, default='gpu')
+
+# dataset
+parser.add_argument("--data_path", type=str, default='../../../dataset/mnist/', help="the path of loading data")
+
+# model
+parser.add_argument("--save_path", type=str, default='../../save_models', help="the path of saving model")
+parser.add_argument("--load_path", type=str, default='../../save_models/LDA.npy', help="the path of loading model")
+
+parser.add_argument("--z_dim", type=int, default=128, help="dimensionality of the z latent space")
+
+# optim
+parser.add_argument("--num_epochs", type=int, default=100, help="number of epochs of training")
+
+args = parser.parse_args()
+
+# =========================================== Dataset ===================================================================== #
 # define transform for dataset and load orginal dataset
 transform = transforms.Compose([transforms.ToTensor()])
-train_dataset = datasets.MNIST(root='../../dataset/mnist/', train=True, download=True)
-test_dataset = datasets.MNIST(root='../../dataset/mnist/', train=False, download=False)
+train_dataset = datasets.MNIST(root=args.data_path, train=True, download=True)
+test_dataset = datasets.MNIST(root=args.data_path, train=False, download=False)
 
 # transform dataset and reshape the dataset into [batch_size, feature_num]
 train_data = tensor_transforms(train_dataset.data, transform)
-train_data = train_data.permute(1, 2, 0).reshape(len(train_dataset), -1)# len(train_dataset, 28*28)
+train_data = train_data.permute([1, 2, 0]).reshape([len(train_dataset), -1])  # len(train_dataset, 28*28)
 test_data = tensor_transforms(test_dataset.data, transform)
-test_data = test_data.permute(1, 2, 0).reshape(len(test_dataset), -1)
+test_data = test_data.permute([1, 2, 0]).reshape([len(test_dataset), -1])
 train_label = train_dataset.train_labels
 test_label = test_dataset.test_labels
 
 # transpose the dataset to fit the model and convert a tensor to numpy array
 train_data = np.array(np.ceil(train_data[:999, :].T.numpy() * 5), order='C')
 test_data = np.array(np.ceil(test_data[:999, :].T.numpy() * 5), order='C')
 train_label = train_label.numpy()[:999]
 test_label = test_label.numpy()[:999]
 
+# =========================================== Model ===================================================================== #
 # create the model and deploy it on gpu or cpu
-model = DPGDS([200, 100, 50], 'gpu')  # topics of each layers
+model = LDA(K=args.z_dim, device=args.device)
 model.initial(train_data)  # use the shape of train_data to initialize the params of model
-train_local_params = model.train(train_data, iter_all=200)
-train_local_params = model.test(train_data, iter_all=200)
-test_local_params = model.test(test_data, iter_all=200)
 
-# evaluate the model with classification accuracy
-# the demo accuracy can achieve 0.8519
-results = ACC(train_local_params.Theta[0], test_local_params.Theta[0], train_label, test_label, 'SVM')
+# train and evaluation
+train_local_params = model.train(data=train_data, num_epochs=args.num_epochs)
+train_local_params = model.test(data=train_data, num_epochs=args.num_epochs)
+test_local_params = model.test(data=test_data, num_epochs=args.num_epochs)
 
 # save the model after training
-model.save()
-# model.load('./save_models/DPGDS.npy')
+model.save(args.save_path)
+# load the model
+model.load(args.load_path)
+
+# evaluate the model with classification accuracy
+# the demo accuracy can achieve 0.850
+results = ACC(train_local_params.Theta, test_local_params.Theta, train_label, test_label, 'SVM')
+
+
+
```

### Comparing `pydpm-4.0.2/pydpm/example/Bayesian_GM/Graph_Poisson_Gamma_Belief_Network/GPGBN_Demo.py` & `pydpm-5.0.0/pydpm/example/Bayesian_PM/Factor_Analysis/FA_demo.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,71 +1,82 @@
 """
 ===========================================
-Deep Relational Topic Modeling via Graph Poisson Gamma Belief Network
-Chaojie Wang, Hao Zhang, Bo Chen, Dongsheng Wang, Zhengjue Wang
-Published in Advances in Neural Information Processing System 2020
-
+Factor Analysis
 ===========================================
 
 """
 
-# Author: Chaojie Wang <xd_silly@163.com>; Wei Zhao <13279389260@163.com>; Jiawen Wu <wjw19960807@163.com>
-# License: BSD-3-Clause
+# Author: Xinyang Liu <lxy771258012@163.com>;
+# License: BSD-3-Claus
 
-import os
 import numpy as np
 import scipy.io as sio
-
-from pydpm.metric import ACC
-from pydpm.model import GPGBN
+import argparse
+from torchvision import datasets, transforms
+import matplotlib.pyplot as plt
+from pydpm.model import FA
+from pydpm.utils.utils import *
 from pydpm.dataloader.image_data import tensor_transforms
-from pydpm.dataloader.graph_data import Graph_Processer
-from pydpm.utils import cosine_simlarity
 
-from torchvision import datasets, transforms
-from torch_geometric.datasets import Planetoid
+# # load data
+# data = sio.loadmat('../../../dataset/FA_data.mat')
+# train_data = np.array(data['x1'])
+
+# =========================================== ArgumentParser ===================================================================== #
+parser = argparse.ArgumentParser()
+
+# device
+parser.add_argument("--device", type=str, default='gpu')
+
+# dataset
+parser.add_argument("--data_path", type=str, default='../../../dataset/mnist/', help="the path of loading data")
 
-# # load dataset (Cora) cost too much memory
-# path = '../../dataset/Planetoid'
-# if not os.path.exists(path):
-#     os.mkdir(path)
-# dataset = Planetoid(path, 'cora')
-# dataset = dataset[0]
-#
-# graph = graph_from_edges(dataset.edge_index, dataset.num_nodes, to_sparsetesor=False)[1]
-# # transpose the dataset to fit the model and convert a tensor to numpy array
-# train_data = dataset.x.T.numpy()
+# model
+parser.add_argument("--save_path", type=str, default='../../save_models', help="the path of saving model")
+parser.add_argument("--load_path", type=str, default='../../save_models/FA.npy', help="the path of loading model")
 
-# load dataset (MNIST)
+parser.add_argument("--z_dim", type=int, default=128, help="number of components according dataset")
+
+# optim
+parser.add_argument("--num_epochs", type=int, default=1000, help="number of epochs of training")
+
+args = parser.parse_args()
+# =========================================== Dataset ===================================================================== #
 # define transform for dataset and load orginal dataset
 transform = transforms.Compose([transforms.ToTensor()])
-train_dataset = datasets.MNIST(root='../../dataset/mnist/', train=True, download=True)
-test_dataset = datasets.MNIST(root='../../dataset/mnist/', train=False, download=False)
+train_dataset = datasets.MNIST(root=args.data_path, train=True, download=True)
+test_dataset = datasets.MNIST(root=args.data_path, train=False, download=False)
 
 # transform dataset and reshape the dataset into [batch_size, feature_num]
 train_data = tensor_transforms(train_dataset.data, transform)
-train_data = train_data.permute([1, 2, 0]).reshape(len(train_dataset), -1)  # len(train_dataset, 28*28)
+train_data = train_data.permute([1, 2, 0]).reshape([len(train_dataset), -1])  # len(train_dataset, 28*28)
 test_data = tensor_transforms(test_dataset.data, transform)
-test_data = test_data.permute([1, 2, 0]).reshape(len(test_dataset), -1)
+test_data = test_data.permute([1, 2, 0]).reshape([len(test_dataset), -1])
 train_label = train_dataset.train_labels
 test_label = test_dataset.test_labels
 
 # transpose the dataset to fit the model and convert a tensor to numpy array
-train_data = np.array(np.ceil(train_data[:999, :].T.numpy() * 5), order='C')
+# !!! Transposition, data: [D, N]
+train_data = np.array(np.ceil(train_data[:999, :].T.numpy()), order='C')
+# test_data = np.array(np.ceil(test_data[:999, :].T.numpy()), order='C')
+train_data = standardization(train_data)
+# test_data = standardization(test_data)
 train_label = train_label.numpy()[:999]
+# test_label = test_label.numpy()[:999]
 
-# construct the adjacency matrix
-graph_processer = Graph_Processer()
-graph = graph_processer.graph_from_node_feature(train_data.T, 0.5, binary=False)
+# create the model and deploy it on gpu or cpu
+model =FA(args.z_dim, 'gpu')
+model.initial(train_data)  # use the shape of train_data to initialize the params of model
 
+# train and evaluation
+train_local_params = model.train(train_data, args.num_epochs)
 
+x_hat = np.matmul(train_local_params.w, train_local_params.z)
 
-# create the model and deploy it on gpu or cpu
-model = GPGBN([128, 64, 32], device='gpu')
-model.initial(train_data)
-train_local_params = model.train(train_data, graph, iter_all=100)
+# visualization for one sample
+plt.plot(train_data[:, 880], 'ro', marker='*', label="train data")
+plt.plot(x_hat[:, 880], 'bo', marker='v', label="reconstruction")
+plt.legend(loc="best")
+plt.show()
 
 # save the model after training
 model.save()
-# model.load('./save_models/PGBN.npy')
-
-
```

### Comparing `pydpm-4.0.2/pydpm/example/Bayesian_GM/Poisson_Gamma_Dynamic_System/PGDS_Demo.py` & `pydpm-5.0.0/pydpm/example/Bayesian_PM/Multimodal_Poisson_Gamma_Belief_Network/MPGBN_Demo.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,85 @@
 """
 ===========================================
-Poisson Gamma Dynamical Systems Demo
-Aaron Schein, Hanna Wallach and Mingyuan Zhou
-Published in Neural Information Processing Systems 2016
+Multimodal Poisson Gamma Belief Network
+Chaojie Wang, Bo Chen and Mingyuan Zhou
+Published in In AAAI Conference on Artificial Intelligence
 
 ===========================================
 
 """
 
 # Author: Chaojie Wang <xd_silly@163.com>; Jiawen Wu <wjw19960807@163.com>; Wei Zhao <13279389260@163.com>
 # License: BSD-3-Clause
 
 import numpy as np
+import argparse
 import scipy.io as sio
 
-from pydpm.metric import ACC
-from pydpm.model import PGDS
-
 from torchvision import datasets, transforms
+
+from pydpm.model import MPGBN
+from pydpm.metric import ACC
 from pydpm.dataloader.image_data import tensor_transforms
 
-# load dataset
+# =========================================== ArgumentParser ===================================================================== #
+parser = argparse.ArgumentParser()
+
+# device
+parser.add_argument("--device", type=str, default='gpu')
+
+# dataset
+parser.add_argument("--data_path", type=str, default='../../../dataset/mnist/', help="the path of loading data")
+
+# model
+parser.add_argument("--save_path", type=str, default='../../save_models', help="the path of saving model")
+parser.add_argument("--load_path", type=str, default='../../save_models/MPGBN.npy', help="the path of loading model")
+
+parser.add_argument("--z_dims", type=list, default=[128, 64, 32], help="number of topics at diffrent layers in MPGBN")
+
+args = parser.parse_args()
+
+# =========================================== Dataset ===================================================================== #
 # define transform for dataset and load orginal dataset
 transform = transforms.Compose([transforms.ToTensor()])
-train_dataset = datasets.MNIST(root='../../dataset/mnist/', train=True, download=True)
-test_dataset = datasets.MNIST(root='../../dataset/mnist/', train=False, download=False)
+train_dataset = datasets.MNIST(root=args.data_path, train=True, download=True)
+test_dataset = datasets.MNIST(root=args.data_path, train=False, download=False)
 
 # transform dataset and reshape the dataset into [batch_size, feature_num]
 train_data = tensor_transforms(train_dataset.data, transform)
 train_data = train_data.permute([1, 2, 0]).reshape(len(train_dataset), -1)  # len(train_dataset, 28*28)
 test_data = tensor_transforms(test_dataset.data, transform)
 test_data = test_data.permute([1, 2, 0]).reshape(len(test_dataset), -1)
 train_label = train_dataset.train_labels
 test_label = test_dataset.test_labels
 
 # transpose the dataset to fit the model and convert a tensor to numpy array
 train_data = np.array(np.ceil(train_data[:999, :].T.numpy() * 5), order='C')
+train_data_1 = train_data[:360, :]
+train_data_2 = train_data[360:, :]
 test_data = np.array(np.ceil(test_data[:999, :].T.numpy() * 5), order='C')
+test_data_1 = test_data[:360, :]
+test_data_2 = test_data[360:, :]
 train_label = train_label.numpy()[:999]
 test_label = test_label.numpy()[:999]
 
+# =========================================== Model ===================================================================== #
 # create the model and deploy it on gpu or cpu
-model = PGDS(100, 'gpu')
-model.initial(train_data)
-train_local_params = model.train(train_data, iter_all=200)
-train_local_params = model.test(train_data, iter_all=200)
-test_local_params = model.test(test_data, iter_all=200)
+model = MPGBN(K=args.z_dims, device=args.device)
+model.initial(train_data_1, train_data_2)  # use the shape of train_data_1 and train_data_2 to initialize the params of model
 
-# evaluate the model with classification accuracy
-# the demo accuracy can achieve 0.8739
-results = ACC(train_local_params.Theta, test_local_params.Theta, train_label, test_label, 'SVM')
+# train and evaluation
+train_local_params = model.train(train_data_1, train_data_2, num_epochs=args.num_epochs)
+train_local_params = model.test(train_data_1, train_data_2, num_epochs=args.num_epochs)
+test_local_params = model.test(test_data_1, test_data_2, num_epochs=args.num_epochs)
 
 # save the model after training
-model.save()
-# model.load('./save_models/PGDS.npy')
+model.save(args.save_path)
+# load the model
+model.load(args.load_path)
+
+# evaluate the model with classification accuracy
+# the demo accuracy can achieve 0.8549
+results = ACC(train_local_params.Theta[0], test_local_params.Theta[0], train_label, test_label, 'SVM')
+
+
```

### Comparing `pydpm-4.0.2/pydpm/example/Bayesian_GM/Word_Embeddings_Deep_Topic_Model/WEDTM_Demo.py` & `pydpm-5.0.0/pydpm/example/Bayesian_PM/Deep_Poisson_Factor_Analysis/DPFA_Demo.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,96 +1,88 @@
-"""
-===========================================
-WEDTM Demo
-Inter and Intra Topic Structure Learning with Word Embeddings
-He Zhao, Lan Du, Wray Buntine, Mingyaun Zhou
-Published in International Council for Machinery Lubrication 2018
-
-===========================================
-
-"""
-
-# Author: Chaojie Wang <xd_silly@163.com>; Jiawen Wu <wjw19960807@163.com>; Wei Zhao <13279389260@163.com>
-# License: BSD-3-Clause
-import nltk
-import numpy as np
-import scipy.io as sio
-import torch
-
-from pydpm.metric import ACC
-from pydpm.model import WEDTM
-
-from nltk.corpus import stopwords
-from torch.utils.data import Dataset, DataLoader
-from torchtext.data.utils import get_tokenizer
-from torchtext.vocab import GloVe
-from torchtext.datasets import AG_NEWS
-from pydpm.dataloader.text_data import Text_Processer, build_vocab_from_iterator
-
-# Load dataset (AG_NEWS from torchtext)
-train_iter, test_iter = AG_NEWS('../dataset/', split=('train', 'test'))
-tokenizer = get_tokenizer("basic_english")
-
-# build vocabulary
-# nltk.download('stopwords')
-stop_words = list(stopwords.words('english'))
-vocab_size = 7000
-vocab = build_vocab_from_iterator(map(lambda x: tokenizer(x[1]), train_iter), special_first=False, stop_words=stop_words, max_tokens=vocab_size)
-text_processer = Text_Processer(tokenizer=tokenizer, vocab=vocab)
-
-# Get train/test label and data_file(tokens) from data_iter and convert them into clean file
-train_files, train_labels = text_processer.file_from_iter(train_iter, tokenizer=tokenizer)
-test_files, test_labels = text_processer.file_from_iter(test_iter, tokenizer=tokenizer)
-
-# Take part of dataset for convenience
-train_idxs = np.arange(5000)
-np.random.shuffle(train_idxs)
-train_files = [train_files[i] for i in train_idxs]
-train_labels = [train_labels[i] for i in train_idxs]
-
-test_idxs = np.arange(1000)
-np.random.shuffle(test_idxs)
-test_files = [test_files[i] for i in test_idxs]
-test_labels = [test_labels[i] for i in test_idxs]
-
-# Build word embedding
-vector = GloVe(name='6B', dim=50)
-voc_embedding = vector.get_vecs_by_tokens(vocab.get_itos(), lower_case_backup=True)
-
-# Dataloader
-train_bow, train_labels = text_processer.bow_from_file(train_files, train_labels, to_sparse=False)
-test_bow, test_labels = text_processer.bow_from_file(test_files, test_labels, to_sparse=False)
-
-# Transpose dataset to fit the model and convert a tensor to numpy
-train_data = np.asarray(train_bow).T.astype(int)
-test_data = np.asarray(test_bow).T.astype(int)
-voc_embedding = voc_embedding.numpy()
-
-print('Data has been processed!')
-
-# params of model
-T = 3  # vertical layers
-S = 3  # sub topics
-K = [100] * T  # topics in each layers
-
-# create the model and deploy it on gpu or cpu
-model = WEDTM(K, 'gpu')
-model.initial(train_data)  # use the shape of train_data to initialize the params of model
-train_local_params = model.train(voc_embedding, train_data, S, iter_all=300, is_initial_local=False)
-train_local_params = model.test(voc_embedding, train_data, S, iter_all=300)
-test_local_params = model.test(voc_embedding, test_data, S, iter_all=300)
-
-
-# evaluate the model with classification accuracy
-results = ACC(train_local_params.Theta, test_local_params.Theta, train_labels, test_labels, 'SVM')
-
-# save the model after training
-model.save()
-# model.load('./save_models/WEDTM.npy')
-
-# # load dataset (WS.mat from paper)
-# dataset = sio.loadmat('../../dataset/WS.mat')
-# train_data = np.asarray(dataset['doc'].todense()[:, dataset['train_idx'][0]-1])[:, ::10].astype(int)
-# test_data = np.asarray(dataset['doc'].todense()[:, dataset['test_idx'][0]-1])[:, ::5].astype(int)
-# train_label = dataset['labels'][dataset['train_idx'][0]-1][::10, :]
-# test_label = dataset['labels'][dataset['test_idx'][0]-1][::5, :]
-
+"""
+===========================================
+Deep Poisson Factor Analysis Demo
+Scalable Deep Poisson Factor Analysis for Topic Modeling
+Zhe Gan, Changyou Chen, Ricardo Henao, David Carlson, Lawrence Carin
+Publised in International Conference on Machine Learning 2015
+
+===========================================
+
+"""
+
+# Author: Chaojie Wang <xd_silly@163.com>; Jiawen Wu <wjw19960807@163.com>; Wei Zhao <13279389260@163.com>
+# License: BSD-3-Clause
+
+import numpy as np
+import argparse
+import scipy.io as sio
+
+from torchvision import datasets, transforms
+
+from pydpm.model import DPFA
+from pydpm.metric import ACC
+from pydpm.dataloader.image_data import tensor_transforms
+
+# =========================================== ArgumentParser ===================================================================== #
+parser = argparse.ArgumentParser()
+
+# device
+parser.add_argument("--device", type=str, default='gpu')
+
+# dataset
+parser.add_argument("--data_path", type=str, default='../../../dataset/mnist/', help="the path of loading data")
+
+# model
+parser.add_argument("--save_path", type=str, default='../../save_models', help="the path of saving model")
+parser.add_argument("--load_path", type=str, default='../../save_models/DPFA.npy', help="the path of loading model")
+
+parser.add_argument("--z_dims", type=list, default=[128, 64, 32], help="numbers of topics of 3 layers in DPFA(PFA+DSBN+Gibbs)")
+
+# optim
+parser.add_argument("--burnin", type=int, default=100, help="the iterations of burnin stage")
+parser.add_argument("--collection", type=int, default=80, help="the iterations of collection stage")
+
+args = parser.parse_args()
+
+# =========================================== Dataset ===================================================================== #
+# define transform for dataset and load orginal dataset
+# load dataset
+transform = transforms.Compose([transforms.ToTensor()])
+train_dataset = datasets.MNIST(root=args.data_path, train=True, download=True)
+test_dataset = datasets.MNIST(root=args.data_path, train=False, download=False)
+
+# transform dataset and reshape the dataset into [batch_size, feature_num]
+train_data = tensor_transforms(train_dataset.data, transform)
+train_data = train_data.permute([1, 2, 0]).reshape(len(train_dataset), -1)  # len(train_dataset, 28*28)
+test_data = tensor_transforms(test_dataset.data, transform)
+test_data = test_data.permute([1, 2, 0]).reshape(len(test_dataset), -1)
+train_label = train_dataset.train_labels
+test_label = test_dataset.test_labels
+
+# transpose the dataset to fit the model and convert a tensor to numpy array
+train_data = np.array(np.ceil(train_data[:999, :].T.numpy() * 5), order='C')
+test_data = np.array(np.ceil(test_data[:999, :].T.numpy() * 5), order='C')
+train_label = train_label.numpy()[:999]
+test_label = test_label.numpy()[:999]
+
+# =========================================== Model ===================================================================== #
+# create the model and deploy it on gpu or cpu
+model = DPFA(K=args.z_dims, device=args.device)
+model.initial(train_data)  # use the shape of train_data to initialize the params of model
+
+# train and evaluation
+train_local_params = model.train(train_data, burnin=args.burnin, collection=args.collection)
+train_local_params = model.test(train_data, burnin=args.burnin, collection=args.collection)
+test_local_params = model.test(test_data, burnin=args.burnin, collection=args.collection)
+
+# save the model after training
+model.save(args.save_path)
+# load the model
+model.load(args.load_path)
+
+# evaluate the model with classification accuracy
+# the demo accuracy can achieve 0.9099
+results = ACC(train_local_params.Theta, test_local_params.Theta, train_label, test_label, 'SVM')
+
+
+
+
```

### Comparing `pydpm-4.0.2/pydpm/example/Deep_Learning_GM/Generative_Adversarial_Network/GAN_Demo.py` & `pydpm-5.0.0/pydpm/example/Deep_Learning_PM/Variational_Autoencoder/VAE_Demo.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,81 @@
 """
 ===========================================
-GAN
-Generative Adversarial Networks
-IJ Goodfellow，J Pouget-Abadie，M Mirza，B Xu，D Warde-Farley，S Ozair，A Courville，Y Bengio
+VAE
+Auto-Encoding Variational Bayes
+Diederik P. Kingma， Max Welling
 Publihsed in 2014
 
 ===========================================
 """
 
 # Author: Muyao Wang <flare935694542@163.com>, Xinyang Liu <lxy771258012@163.com>
 # License: BSD-3-Clause
 
-import argparse
 import os
-import numpy as np
-import torchvision.transforms as transforms
-from torchvision.utils import save_image
-from torch.utils.data import DataLoader
-from torchvision import datasets
-from pydpm.model import GAN
+import argparse
+import sys
 import torch
+import torch.optim as optim
 
-os.makedirs("../output/images", exist_ok=True)
+from torchvision import datasets, transforms
+from torchvision.utils import save_image
+from pydpm.model import VAE
+
+# =========================================== ArgumentParser ===================================================================== #
 parser = argparse.ArgumentParser()
-parser.add_argument("--n_epochs", type=int, default=200, help="number of epochs of training")
-parser.add_argument("--batch_size", type=int, default=128, help="size of the batches")
-parser.add_argument("--lr", type=float, default=0.0002, help="adam: learning rate")
-parser.add_argument("--b1", type=float, default=0.5, help="adam: decay of first order momentum of gradient")
-parser.add_argument("--b2", type=float, default=0.999, help="adam: decay of first order momentum of gradient")
-parser.add_argument("--g_latent_dim", type=int, default=100, help="generator dimensionality of the latent space")
-parser.add_argument("--z_dim", type=int, default=100, help="generator dimensionality of the z latent space")
-parser.add_argument("--d_latent_dim", type=int, default=100, help="discriminator dimensionality of the latent space")
+
+# device
+parser.add_argument("--gpu_id", type=int, default=0)
+
+# dataset
+parser.add_argument("--data_path", type=str, default='../../../dataset/mnist/', help="the path of loading data")
 parser.add_argument("--img_size", type=int, default=28, help="size of each image dimension")
-parser.add_argument("--channels", type=int, default=1, help="number of image channels")
-parser.add_argument("--sample_interval", type=int, default=800, help="interval betwen image samples")
+
+# model
+parser.add_argument("--save_path", type=str, default='../../save_models', help="the path of saving model")
+parser.add_argument("--load_path", type=str, default='../../save_models/VAE.pth', help="the path of loading model")
+
+parser.add_argument("--z_dim", type=int, default=2, help="dimensionality of the z latent space")
+parser.add_argument("--encoder_hid_dims", type=int, default=[512, 256], help="dimensionality of the latent space")
+parser.add_argument("--decoder_hid_dims", type=int, default=[512, 256], help="dimensionality of the latent space")
+
+# optim
+parser.add_argument("--num_epochs", type=int, default=2, help="number of epochs of training")
+parser.add_argument("--batch_size", type=int, default=256, help="size of the batches")
+parser.add_argument("--lr", type=float, default=0.0002, help="adam: learning rate")
+
 args = parser.parse_args()
+args.device = torch.device(f"cuda:{args.gpu_id}") if torch.cuda.is_available() else torch.device("cpu")
 
+# =========================================== Dataset ===================================================================== #
+# mnist
+train_dataset = datasets.MNIST(root=args.data_path, train=True, transform=transforms.ToTensor(), download=True)
+test_dataset = datasets.MNIST(root=args.data_path, train=False, transform=transforms.ToTensor(), download=False)
+
+train_loader = torch.utils.data.DataLoader(dataset=train_dataset, batch_size=args.batch_size, shuffle=True)
+test_loader = torch.utils.data.DataLoader(dataset=test_dataset, batch_size=args.batch_size, shuffle=False)
+
+# =========================================== Model ===================================================================== #
+# model
+model = VAE(in_dim=args.img_size**2, z_dim=args.z_dim, encoder_hid_dims=args.encoder_hid_dims, decoder_hid_dims=args.decoder_hid_dims, device=args.device)
+model_opt = optim.Adam(model.parameters(), lr=args.lr)
+
+# train
+for epoch_idx in range(args.num_epochs):
+    local_mu, local_log_var = model.train_one_epoch(dataloader=train_loader, model_opt=model_opt, epoch_idx=epoch_idx, args=args)
+    if epoch_idx % 25 == 0:
+        test_mu, test_log_var = model.test_one_epoch(dataloader=test_loader)
+
+# save
+model.save(args.save_path)
+# load
+model.load(args.load_path)
 
-# MNIST Dataset
-transform = transforms.Compose([transforms.Resize(args.img_size), transforms.ToTensor(), transforms.Normalize([0.5], [0.5])])
-train_dataset = datasets.MNIST(root='../../dataset/mnist/', train=True, transform=transform, download=True)
-dataloader = torch.utils.data.DataLoader(dataset=train_dataset, batch_size=args.batch_size, shuffle=True)
-
-# Initialize generator and discriminator
-img_shape = (args.channels, args.img_size, args.img_size)
-model = GAN(img_shape, g_latent_dim=args.g_latent_dim, z_dim=args.z_dim, d_latent_dim=args.d_latent_dim, device='cuda:0')
-
-# Optimizers
-model_opt_G = torch.optim.Adam(model.generator.parameters(), lr=args.lr, betas=(args.b1, args.b2))
-model_opt_D = torch.optim.Adam(model.discriminator.parameters(), lr=args.lr, betas=(args.b1, args.b2))
-
-# Training
-for epoch in range(args.n_epochs):
-    model.train_one_epoch(model_opt_G=model_opt_G, model_opt_D=model_opt_D, dataloader=dataloader, sample_interval=args.sample_interval, epoch=epoch, n_epochs=args.n_epochs)
-
-model.save()
-model.load('../save_models/GAN.pth')
-print(model)
+# =================== Visualization ====================== #
+os.makedirs("../../output/images", exist_ok=True)
 print('sample image,please wait!')
-save_image(model.sample(64), "../images/GAN_images.png", nrow=8, normalize=True)
-print('complete!!!')
+with torch.no_grad():
+    sample = model.sample(64)
+    save_image(sample.view(64, 1, 28, 28), '../../output/images/VAE_sample.png')
+print('complete!!!')
+
```

### Comparing `pydpm-4.0.2/pydpm/example/Hybrid_GM/Weibull_Graph_Attention_Autoencoder/WGAAE_Demo.py` & `pydpm-5.0.0/pydpm/example/Hybrid_PM/Weibull_Graph_Attention_Autoencoder/WGAAE_Demo.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 
 import os
 import argparse
 import random
 import numpy as np
 import scipy.sparse as sp
 
+import torch
+import torch_geometric.transforms as T
+from torch_geometric.datasets import Planetoid
+
 from pydpm.model import WGAAE
 from pydpm.utils import *
 from pydpm.dataloader.graph_data import Graph_Processer
 from pydpm.metric.roc_score import ROC_AP_SCORE
 
-import torch
-import torch_geometric.transforms as T
-from torch_geometric.datasets import Planetoid
-
+# =========================================== ArgumentParser ===================================================================== #
 parser = argparse.ArgumentParser()
 
 # device
 parser.add_argument("--gpu_id", type=int, default=0, help="the id of gpu to deploy")
 parser.add_argument('--seed', type=int, default=123, help='Setting random seed')
 
 # dataset
@@ -46,30 +47,31 @@
 parser.add_argument('--graph_lh', type=str, default='Laplacian', help='Graph likelihood')
 parser.add_argument('--lambda', type=float, default=1.0, help='lamda')
 parser.add_argument('--theta_norm', type=bool, default=False, help='Whether theta norm')
 
 args = parser.parse_args()
 args.device = 'cpu' if not torch.cuda.is_available() else f'cuda:{args.gpu_id}'
 
-
 seed_everything(args.seed)
 
+# =========================================== Dataset ===================================================================== #
 # Prepare for dataset
 dataset = Planetoid(args.dataset_path, args.dataset)
 data = dataset[0].to(args.device)
 data.edge_index = data.edge_index[[1, 0]]
 graph_processer = Graph_Processer()
 
 adj_csc = graph_processer.graph_from_edges(data.edge_index, data.num_nodes).tocsc()
 adj_train, train_edges, val_edges, val_edges_false, test_edges, test_edges_false = graph_processer.edges_split_from_graph(adj_csc)
 
 # For encoder input and graph likelihood
 adj_train = adj_train + sp.eye(adj_train.shape[0])
 data.edge_index = graph_processer.edges_from_graph(adj_train.tocoo(), args.device)
 
+# =========================================== Model ===================================================================== #
 model = WGAAE(in_dim=dataset.num_features, out_dim=args.out_dim, z_dims=args.z_dims, hid_dims=args.hid_dims, num_heads=args.num_heads, device=args.device)
 optim = torch.optim.Adam(model.parameters())
 
 # Training
 best_AUC = best_AP = 0
 for epoch_index in range(args.num_epochs):
     if epoch_index <= 200:
```

### Comparing `pydpm-4.0.2/pydpm/example/Hybrid_GM/Weibull_Hybrid_Autoencoding_Inference/WHAI_Demo.py` & `pydpm-5.0.0/pydpm/example/Hybrid_PM/Weibull_Hybrid_Autoencoding_Inference/WHAI_Demo.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,67 +7,68 @@
 ===========================================
 
 """
 
 # Author: Xinyang Liu <lxy771258012@163.com>
 # License: BSD-3-Clause
 
+import os
 import argparse
 import numpy as np
 import scipy.io as sio
 from sklearn.cluster import k_means
 from nltk.corpus import stopwords
-
-from pydpm.model import WHAI
-from pydpm.utils import *
-from pydpm.metric import *
-from pydpm.dataloader.text_data import Text_Processer, build_vocab_from_iterator
+os.environ["CUDA_VISIBLE_DEVICES"]="0"
 
 import torch
 from torch.utils.data import DataLoader
 
 from torchtext.data.utils import get_tokenizer
 from torchtext.datasets import AG_NEWS
 
+from pydpm.model import WHAI
+from pydpm.utils import *
+from pydpm.metric import *
+from pydpm.dataloader.text_data import Text_Processer, build_vocab_from_iterator
+
+# =========================================== ArgumentParser ===================================================================== #
 parser = argparse.ArgumentParser()
 
 # device
 parser.add_argument("--gpu_id", type=int, default=0, help="the id of gpu to deploy")
 
 # dataset
 parser.add_argument("--dataset", type=str, default='AG_NEWS', help="the name of dataset")
-parser.add_argument("--dataset_path", type=str, default='../../../dataset', help="the file path of dataset")
+parser.add_argument("--data_path", type=str, default='../../../dataset', help="the file path of dataset")
 
-# network settings
+# model
 parser.add_argument("--voc_size", type=int, default=20000, help="the length of vocabulary")
 parser.add_argument("--z_dims", type=list, default=[128, 64, 32], help="the list of z dimension")
 parser.add_argument("--hid_dims", type=list, default=[200, 200, 200], help="the list of hidden dimension")
 
-# optimizer
-parser.add_argument("--lr", type=float, default=0.0002, help="adam: learning rate")
-
-# training
+# optim
 parser.add_argument("--num_epochs", type=int, default=1000, help="number of epochs of training")
-parser.add_argument("--MBratio", type=int, default=50, help="number of epochs of training")
 parser.add_argument("--batch_size", type=int, default=256, help="size of the batches")
+parser.add_argument("--lr", type=float, default=0.0002, help="adam: learning rate")
+parser.add_argument("--MBratio", type=int, default=50, help="number of epochs of training")
 
 args = parser.parse_args()
-args.device = 'cpu' if not torch.cuda.is_available() else f'cuda:{args.gpu_id}'
+args.device = torch.device(f"cuda:{args.gpu_id}") if torch.cuda.is_available() else torch.device("cpu")
 
-# Load dataset (AG_NEWS from torchtext)
-train_iter, test_iter = AG_NEWS(args.dataset_path, split=('train', 'test'))
+# =========================================== Dataset ===================================================================== #
+# load dataset (AG_NEWS from torchtext)
+train_iter, test_iter = AG_NEWS(args.data_path, split=('train', 'test'))
 tokenizer = get_tokenizer("basic_english")
 
 # build vocabulary
 stop_words = list(stopwords.words('english'))
 vocab = build_vocab_from_iterator(map(lambda x: tokenizer(x[1]), train_iter), specials=['<unk>', '<pad>', '<bos>', '<eos>'], special_first=True, stop_words=stop_words, max_tokens=args.voc_size)
 vocab.set_default_index(vocab['<unk>'])
 text_processer = Text_Processer(tokenizer=tokenizer, vocab=vocab)
 
-
 # Get train/test label and data_file(tokens) from data_iter and convert them into clean file
 train_files, train_labels = text_processer.file_from_iter(train_iter, tokenizer=tokenizer)
 test_files, test_labels = text_processer.file_from_iter(test_iter, tokenizer=tokenizer)
 
 # Take part of dataset for convenience
 train_idxs = np.arange(7000)
 np.random.shuffle(train_idxs)
@@ -75,34 +76,35 @@
 train_labels = [train_labels[i] for i in train_idxs]
 
 test_idxs = np.arange(3000)
 np.random.shuffle(test_idxs)
 test_files = [test_files[i] for i in test_idxs]
 test_labels = [test_labels[i] for i in test_idxs]
 
-# =========================================== load data 1 ===================================================================== #
 train_bows, train_labels = text_processer.bow_from_file(train_files, train_labels)
 test_bows, test_labels = text_processer.bow_from_file(test_files, test_labels)
 
 train_loader = DataLoader([train_data for train_data in zip(train_bows, train_labels)], batch_size=256, shuffle=False, num_workers=4, drop_last=True)
 test_loader = DataLoader([test_data for test_data in zip(test_bows, test_labels)], batch_size=256, shuffle=False, num_workers=4, drop_last=True)
 
-cls_num = len(np.unique(train_labels + test_labels))
-model = WHAI(in_dim=args.voc_size, z_dims=args.z_dims, hid_dims=args.hid_dims, device=args.device)
+# =========================================== Model ===================================================================== #
+model = WHAI(in_dim=args.voc_size, z_dims=args.z_dims, hid_dims=args.hid_dims, device=args.device, encode_prior=False)
 model_opt = torch.optim.Adam(model.parameters())
 
-for epoch in range(args.num_epochs):
-    train_local_params = model.train_one_epoch(dataloader=train_loader, optim=model_opt, epoch_index=epoch, args=args, is_train=True)
-    if (epoch+1) % 20 == 0:
+for epoch_idx in range(args.num_epochs):
+    train_local_params = model.train_one_epoch(dataloader=train_loader, optim=model_opt, epoch_idx=epoch_idx, args=args)
+
+    if (epoch_idx+1) % 20 == 0:
         test_local_params = model.test_one_epoch(dataloader=test_loader)
         # calculate PPL
         x_hat = np.matmul(test_local_params.Theta[0], np.transpose(model.global_params.Phi[0]))
         ppl = Perplexity(test_local_params.data, x_hat)
 
         # calculate NMI with train_local_params
+        cls_num = len(np.unique(train_labels + test_labels))
         test_theta_norm = standardization(test_local_params.Theta[0])
         tmp = k_means(test_theta_norm, cls_num)  # N*K
         predict_label = tmp[1] + 1 # Some label start with '1' not '0', there should be 'tmp[1] + 1'
         MI = NMI(test_local_params.label, predict_label)
```

### Comparing `pydpm-4.0.2/pydpm/example/Sampler_Demo.py` & `pydpm-5.0.0/pydpm/example/Sampler_Demo.py`

 * *Files identical despite different names*

### Comparing `pydpm-4.0.2/pydpm/example/Sampler_Speed_Demo.py` & `pydpm-5.0.0/pydpm/example/Sampler_Speed_Demo.py`

 * *Files identical despite different names*

### Comparing `pydpm-4.0.2/pydpm/metric/accuracy.py` & `pydpm-5.0.0/pydpm/metric/accuracy.py`

 * *Files identical despite different names*

### Comparing `pydpm-4.0.2/pydpm/metric/cluster_acc.py` & `pydpm-5.0.0/pydpm/metric/cluster_acc.py`

 * *Files identical despite different names*

### Comparing `pydpm-4.0.2/pydpm/metric/normalized_mutual_information.py` & `pydpm-5.0.0/pydpm/metric/normalized_mutual_information.py`

 * *Files identical despite different names*

### Comparing `pydpm-4.0.2/pydpm/metric/perplexity.py` & `pydpm-5.0.0/pydpm/metric/perplexity.py`

 * *Files identical despite different names*

### Comparing `pydpm-4.0.2/pydpm/metric/reconstruction.py` & `pydpm-5.0.0/pydpm/metric/reconstruction.py`

 * *Files identical despite different names*

### Comparing `pydpm-4.0.2/pydpm/metric/roc_score.py` & `pydpm-5.0.0/pydpm/metric/roc_score.py`

 * *Files identical despite different names*

### Comparing `pydpm-4.0.2/pydpm/metric/topic_coherence.py` & `pydpm-5.0.0/pydpm/metric/topic_coherence.py`

 * *Files identical despite different names*

### Comparing `pydpm-4.0.2/pydpm/model/basic_model.py` & `pydpm-5.0.0/pydpm/model/basic_model.py`

 * *Files identical despite different names*

### Comparing `pydpm-4.0.2/pydpm/model/bayesian_gm/cpfa.py` & `pydpm-5.0.0/pydpm/model/bayesian_pm/cpfa.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,18 +107,18 @@
         self._hyper_params.c_n_f0 = 0.1
 
         self.global_params.D_k = np.random.rand(self._model_setting.K, 1, _structure.K_S3, _structure.K_S4)
         for k in range(self._model_setting.K):
             self.global_params.D_k[k, :, :, :] = self.global_params.D_k[k, :, :, :] / np.sum(self.global_params.D_k[k, :, :, :])
 
 
-    def train(self, data: list, is_sparse: bool=False, iter_all: int=1, is_train: bool=True, is_initial_local: bool=True):
+    def train(self, data: list, is_sparse: bool=False, num_epochs: int=1, is_train: bool=True, is_initial_local: bool=True):
         '''
         Inputs:
-            iter_all   : [int] scalar, the iterations of gibbs sampling
+            num_epochs   : [int] scalar, the iterations of gibbs sampling
             dense matrix representation
                 args[0] : [np.ndarray] N*V*L matrix, N documents represented as V*L sparse matrices
 
             sparse matrix representation
                 args[0] : [list] N documents under the sparse representation, batch.rows, batch.cols, batch.values
                 args[1] : [list] the shape of the input document matrix, N*V*L
             **kwargs:
@@ -158,15 +158,15 @@
             batch_file_indices, batch_rows, batch_cols = np.where(data[0])
             batch_values = data[0][batch_file_indices, batch_rows, batch_cols]
         else:
             assert len(data) == 2, Warning('The length of sparse data list should be 2')
             batch_rows, batch_cols, batch_file_indices, batch_values = data[0]
             self._model_setting.N, self._model_setting.V, self._model_setting.L = data[1]
 
-        self._model_setting.Iteration = iter_all
+        self._model_setting.Iteration = num_epochs
         _structure = self._model_setting._structure
 
         # initial local parameters
         if is_initial_local or not hasattr(self.local_params, 'W_nk') or hasattr(self.local_params, 'c_n') or hasattr(self.local_params, 'p_n'):
             self.local_params.W_nk = np.random.rand(self._model_setting.N, self._model_setting.K, _structure.K_S1, _structure.K_S2)
             self.local_params.c_n = 1 * np.ones([self._model_setting.N])
             self.local_params.p_n = 1 / (1 + self.local_params.c_n)
@@ -195,26 +195,26 @@
             stages = 'Training' if is_train else 'Testing'
             print(f'{stages} Stage: ',
                   f'epoch {iter:3d} takes {end_time - start_time:.2f} seconds')
 
         return copy.deepcopy(self.local_params)
 
 
-    def test(self, data: list, is_sparse: bool=False, iter_all: int=1, is_initial_local: bool=True):
+    def test(self, data: list, is_sparse: bool=False, num_epochs: int=1, is_initial_local: bool=True):
         '''
         Inputs:
-            iter_all   : [int] scalar, the iterations of gibbs sampling
+            num_epochs   : [int] scalar, the iterations of gibbs sampling
             dense matrix representation
                 args[0] : [np.ndarray] N*V*L matrix, N documents represented as V*L sparse matrices
 
             sparse matrix representation
                 args[0] : [list] N documents under the sparse representation, batch.rows, batch.cols, batch.values
                 args[1] : [list] the shape of the input document matrix, N*V*L
         '''
-        local_params = self.train(data, is_sparse=is_sparse, iter_all=iter_all, is_train=False, is_initial_local=is_initial_local)
+        local_params = self.train(data, is_sparse=is_sparse, num_epochs=num_epochs, is_train=False, is_initial_local=is_initial_local)
 
         return local_params
 
 
     def save(self, model_path: str = '../save_models'):
         '''
         Save the model to the specified directory.
```

### Comparing `pydpm-4.0.2/pydpm/model/bayesian_gm/cpgbn.py` & `pydpm-5.0.0/pydpm/model/bayesian_pm/cpgbn.py`

 * *Files identical despite different names*

### Comparing `pydpm-4.0.2/pydpm/model/bayesian_gm/dirbn.py` & `pydpm-5.0.0/pydpm/model/bayesian_pm/dirbn.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,18 +73,18 @@
         assert type(data) is np.ndarray, 'Data type error: the input dataset should be a 2-D np.ndarray'
         self._model_setting.V = data.shape[0]
 
         self.global_params.Phi = np.zeros((self._model_setting.K[0], self._model_setting.V)).astype(int)  # frequency, not distribution
 
         self._hyper_params.Phi_eta = 0.05
 
-    def train(self, data: np.ndarray, iter_all: int, is_train: bool = True, is_initial_local: bool=True):
+    def train(self, data: np.ndarray, num_epochs: int, is_train: bool = True, is_initial_local: bool=True):
         '''
         Inputs:
-            iter_all   : [int] scalar, the iterations of sampling
+            num_epochs   : [int] scalar, the iterations of sampling
             dataset       : [np.ndarray] V*N matrix, N bag-of-words vectors with a vocabulary of length V
             is_train   : [bool] True or False, whether to update the global params in the probabilistic model
 
         Attributes:
             @public:
                 local_params.Theta : [np.ndarray] N_train*K matrix, the topic propotions of N_train documents
 
@@ -96,15 +96,15 @@
 
         Outputs:
                 local_params  : [Params] the local parameters of the probabilistic model
 
         '''
         assert type(data) is np.ndarray, 'Data type error: the input dataset should be a 2-D np.ndarray'
         self._model_setting.N = data.shape[1]
-        self._model_setting.Iteration = iter_all
+        self._model_setting.Iteration = num_epochs
 
         # initial local parameters
         if is_initial_local or not hasattr(self.local_params, 'Theta'):
             self.local_params.Theta = np.zeros((self._model_setting.K[0], self._model_setting.N)).astype(int)
 
             # initial _hyper_params
             self._hyper_params.DirBN_para = self._init_DirBN(self._model_setting.K, self._model_setting.V, self._hyper_params.Phi_eta)
@@ -150,25 +150,25 @@
             stages = 'Training' if is_train else 'Testing'
             print(f'{stages} Stage: ',
                   f'epoch {iter:3d} takes {end_time - start_time:.2f} seconds')
 
         return copy.deepcopy(self.local_params)
 
 
-    def test(self, data: np.ndarray, iter_all: int, is_initial_local: bool=True):
+    def test(self, data: np.ndarray, num_epochs: int, is_initial_local: bool=True):
         '''
         Inputs:
-            iter_all   : [int] scalar, the iterations of gibbs sampling
+            num_epochs   : [int] scalar, the iterations of gibbs sampling
             dataset       : [np.ndarray] V*N matrix, N bag-of-words vectors with a vocabulary of length V
 
         Outputs:
             local_params  : [Params] the local parameters of the probabilistic model
 
         '''
-        local_params = self.train(data, iter_all=iter_all, is_train=False, is_initial_local=is_initial_local)
+        local_params = self.train(data, num_epochs=num_epochs, is_train=False, is_initial_local=is_initial_local)
 
         return local_params
 
 
     def save(self, model_path: str = '../save_models'):
         '''
         Save the model to the specified directory.
```

### Comparing `pydpm-4.0.2/pydpm/model/bayesian_gm/dpfa.py` & `pydpm-5.0.0/pydpm/model/bayesian_pm/dpfa.py`

 * *Files identical despite different names*

### Comparing `pydpm-4.0.2/pydpm/model/bayesian_gm/dpgds.py` & `pydpm-5.0.0/pydpm/model/bayesian_pm/dpgds.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,18 +104,18 @@
             self.global_params.rou[l] = np.zeros((self._model_setting.K[l], 1))
 
         self._hyper_params.tao0 = 1
         self._hyper_params.gamma0 = 100
         self._hyper_params.eta0 = 0.1
         self._hyper_params.epilson0 = 0.1
 
-    def train(self, data: np.ndarray, iter_all: int=1, is_train: bool = True, is_initial_local: bool=True):
+    def train(self, data: np.ndarray, num_epochs: int=1, is_train: bool = True, is_initial_local: bool=True):
         '''
         Inputs:
-            iter_all   : [int] scalar, the iterations of sampling
+            num_epochs   : [int] scalar, the iterations of sampling
             train_data : [np.ndarray] V*N_train matrix, N_train bag-of-words vectors with a vocabulary length of V
             is_train   : [bool] True or False, whether to update the global params in the probabilistic model
 
         Attributes:
             @public:
                 local_params.Theta : [np.ndarray] N_train*K matrix, the topic propotions of N_train documents
 
@@ -162,15 +162,15 @@
                 A_VK[l] = np.zeros((self._model_setting.K[l - 1], self._model_setting.K[l]))
 
             A_KT[l] = np.zeros((self._model_setting.K[l], self._model_setting.T))
             L_dotkt[l] = np.zeros((self._model_setting.K[l], self._model_setting.T + 1))
             L_kdott[l] = np.zeros((self._model_setting.K[l], self._model_setting.T + 1))
             X_layer[l] = np.zeros((self._model_setting.K[l], self._model_setting.T, 2))
 
-        for iter in range(iter_all):
+        for iter in range(num_epochs):
 
             start_time = time.time()
             for l in range(self._model_setting.L):
 
                 L_KK[l] = np.zeros((self._model_setting.K[l], self._model_setting.K[l]))
 
                 if l == 0:
@@ -318,25 +318,25 @@
             stages = 'Training' if is_train else 'Testing'
             print(f'{stages} Stage: ',
                   f'epoch {iter:3d} takes {end_time - start_time:.2f} seconds. Likelihood:{like:8.3f}')
 
         return copy.deepcopy(self.local_params)
 
 
-    def test(self, data: np.ndarray, iter_all: int=1, is_initial_local :bool=True):
+    def test(self, data: np.ndarray, num_epochs: int=1, is_initial_local :bool=True):
         '''
         Inputs:
-            iter_all   : [int] scalar, the iterations of sampling
+            num_epochs   : [int] scalar, the iterations of sampling
             dataset       : [np.ndarray] V*N matrix, N bag-of-words vectors with a vocabulary of length V
 
         Outputs:
             local_params  : [Params] the local parameters of the probabilistic model
 
         '''
-        local_params = self.train(data, iter_all=iter_all, is_train=False, is_initial_local=is_initial_local)
+        local_params = self.train(data, num_epochs=num_epochs, is_train=False, is_initial_local=is_initial_local)
 
         return local_params
 
     def save(self, model_path: str = '../save_models'):
         '''
         Save the model to the specified directory.
         Inputs:
```

### Comparing `pydpm-4.0.2/pydpm/model/bayesian_gm/gpgbn.py` & `pydpm-5.0.0/pydpm/model/bayesian_pm/gpgbn.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,18 +90,18 @@
                 self.global_params.Phi.append(0.2 + 0.8 * np.random.rand(self._model_setting.V, self._model_setting.K[t]))
             else:
                 self.global_params.Phi.append(0.2 + 0.8 * np.random.rand(self._model_setting.K[t-1], self._model_setting.K[t]))
             self.global_params.Phi[t] = self.global_params.Phi[t] / np.maximum(realmin, self.global_params.Phi[t].sum(0))
             self.global_params.U.append(self._sampler.gamma(1 * np.ones([self._model_setting.K[t], 1])) / (1 * np.ones([self._model_setting.K[t], 1])))
 
 
-    def train(self, data:np.ndarray, data_A:np.ndarray, iter_all: int, is_train: bool = True, is_initial_local: bool=True):
+    def train(self, data:np.ndarray, data_A:np.ndarray, num_epochs: int, is_train: bool = True, is_initial_local: bool=True):
         '''
         Inputs:
-            iter_all   : [int] scalar, the iterations of gibbs sampling
+            num_epochs   : [int] scalar, the iterations of gibbs sampling
             dataset       : [np.ndarray] V*N matrix, N bag-of-words vectors with a vocabulary of length V
             is_train   : [bool] True or False, whether to update the global params in the probabilistic model
 
         Attributes:
             @public:
                 local_params.Theta : [list] T (K_t)*(N) topic proportions at different layers
                 local_params.c_j   : [list] T+1 1*N vector, the variables in the scale parameter in the Theta
@@ -114,15 +114,15 @@
         Outputs:
             local_params  : [Params] the local parameters of the probabilistic model
 
         '''
         # todo 1.调整注释  2.train/test  3.展示部分代码  4.cosine_simlar
         assert type(data) is np.ndarray, 'Data type error: the input dataset should be a 2-D np.ndarray'
         self._model_setting.N = data.shape[1]
-        self._model_setting.Iteration = iter_all
+        self._model_setting.Iteration = num_epochs
 
         # initial local params
         if is_initial_local or not hasattr(self.local_params, 'Theta') or not hasattr(self.local_params, 'c_j') or not hasattr(self.local_params, 'p_j') or not hasattr(self.local_params, 'Sigma'):
             self.local_params.Theta = []
             self.local_params.c_j = []
             self.local_params.Sigma = []
             for t in range(self._model_setting.T):  # from layer 1 to T
@@ -271,25 +271,25 @@
             LH_graph = np.sum(data_A * log_max(re_graph) - re_graph) #- log_max(gamma(data_A+1)))
             print("    Graph Likelihood " + str(LH_graph / self._model_setting.N))
             LH_graph_list.append(LH_graph / self._model_setting.N)
 
         return copy.deepcopy(self.local_params)
 
 
-    def test(self, data: np.ndarray, data_A:np.ndarray, iter_all: int, is_initial_local: bool=True):
+    def test(self, data: np.ndarray, data_A:np.ndarray, num_epochs: int, is_initial_local: bool=True):
         '''
         Inputs:
-            iter_all   : [int] scalar, the iterations of gibbs sampling
+            num_epochs   : [int] scalar, the iterations of gibbs sampling
             dataset       : [np.ndarray] V*N matrix, N bag-of-words vectors with a vocabulary of length V
 
         Outputs:
             local_params  : [Params] the local parameters of the probabilistic model
 
         '''
-        local_params = self.train(data, data_A=data_A, iter_all=iter_all, is_train=False, is_initial_local=is_initial_local)
+        local_params = self.train(data, data_A=data_A, num_epochs=num_epochs, is_train=False, is_initial_local=is_initial_local)
 
         return local_params
 
 
     def load(self, model_path: str):
         '''
         Load the model parameters from the specified directory
```

### Comparing `pydpm-4.0.2/pydpm/model/bayesian_gm/lda.py` & `pydpm-5.0.0/pydpm/model/bayesian_pm/lda.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # License: BSD-3-Claus
 
 
 import os
 import copy
 import time
 import numpy as np
+from tqdm import tqdm
 
 from ..basic_model import Basic_Model
 from ...sampler import Basic_Sampler
 from ...utils import *
 
 class LDA(Basic_Model):
     def __init__(self, K: int, device='gpu'):
@@ -72,15 +73,15 @@
         self._hyper_params.Phi_eta = 0.05
         self._hyper_params.Theta_r_k = np.ones([self._model_setting.K, 1])*50 / self._model_setting.K
 
         self.global_params.Phi = np.random.rand(self._model_setting.V, self._model_setting.K)
         self.global_params.Phi = self.global_params.Phi / np.sum(self.global_params.Phi, axis=0)
 
 
-    def train(self, data: np.ndarray, iter_all: int=1, is_train: bool=True, is_initial_local: bool=True):
+    def train(self, data: np.ndarray, num_epochs: int=1, is_train: bool=True, is_initial_local: bool=True):
         '''
         Inputs:
             iter_all   : [int] scalar, the iterations of gibbs sampling
             dataset    : [np.ndarray] V*N matrix, N bag-of-words vectors with a vocabulary of length V
             is_train   : [bool] True or False, whether to update the global params in the probabilistic model
 
         Attributes:
@@ -93,24 +94,24 @@
 
         Outputs:
                 local_params  : [Params] the local parameters of the probabilistic model
 
         '''
         assert type(data) is np.ndarray, 'Data type error: the input dataset should be a 2-D np.ndarray'
         self._model_setting.N = data.shape[1]
-        self._model_setting.Iteration = iter_all
 
         # initial local parameters
         if is_initial_local or not hasattr(self.local_params, 'Theta'):
             self.local_params.Theta = np.ones([self._model_setting.K, self._model_setting.N]) / self._model_setting.K
 
         # gibbs sampling
-        for iter in range(self._model_setting.Iteration):
-            start_time = time.time()
+        train_bar = tqdm(iterable=range(num_epochs))
+        for epoch in train_bar:
 
+            start_time = time.time()
             ZSDS, WSZS = self._sampler.multi_aug(data, self.global_params.Phi, self.local_params.Theta)
 
             # update local params
             if self._model_setting.device == 'cpu':
                 for i in range(ZSDS.shape[1]):
                     self.local_params.Theta[:, i] = np.transpose(self._sampler.dirichlet(np.transpose(ZSDS[:, i] + 50 / self._model_setting.K)))
             else:
@@ -121,32 +122,33 @@
                 if self._model_setting.device == 'cpu':
                     for i in range(WSZS.shape[1]):
                         self.global_params.Phi[:, i] = np.transpose(self._sampler.dirichlet(np.transpose(WSZS[:, i] + self._hyper_params.Phi_eta)))
                 else:
                     self.global_params.Phi = np.transpose(self._sampler.dirichlet(np.transpose(WSZS + self._hyper_params.Phi_eta)))
 
             end_time = time.time()
-            stages = 'Training' if is_train else 'Testing'
-            print(f'{stages} Stage: ',
-                  f'epoch {iter:3d} takes {end_time - start_time:.2f} seconds')
+
+            # tqdm
+            train_bar.set_description(f'Epoch [{epoch}/{num_epochs}]')
+            train_bar.set_postfix(time=end_time - start_time)
 
         return copy.deepcopy(self.local_params)
 
 
-    def test(self, data: np.ndarray, iter_all: int=1, is_initial_local: bool=True):
+    def test(self, data: np.ndarray, num_epochs: int=1, is_initial_local: bool=True):
         '''
         Inputs:
             iter_all   : [int] scalar, the iterations of gibbs sampling
             dataset       : [np.ndarray] V*N matrix, N bag-of-words vectors with a vocabulary of length V
 
         Outputs:
             local_params  : [Params] the local parameters of the probabilistic model
 
         '''
-        local_params = self.train(data, iter_all=iter_all, is_train=False, is_initial_local=is_initial_local)
+        local_params = self.train(data, num_epochs=num_epochs, is_train=False, is_initial_local=is_initial_local)
 
         return local_params
 
 
     def load(self, model_path: str):
         '''
         Load the model parameters from the specified directory
@@ -177,8 +179,7 @@
         for params in ['global_params', 'local_params', '_model_setting', '_hyper_params']:
             if params in dir(self):
                 model[params] = getattr(self, params)
 
         np.save(model_path + '/' + self._model_name + '.npy', model)
 
 
-
```

### Comparing `pydpm-4.0.2/pydpm/model/bayesian_gm/mpgbn.py` & `pydpm-5.0.0/pydpm/model/bayesian_pm/mpgbn.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,18 +96,18 @@
 
                 self.global_params.Phi.append([Phi_1, Phi_2])
             else:
                 self.global_params.Phi.append(0.2 + 0.8 * np.random.rand(self._model_setting.K[t-1], self._model_setting.K[t]))
                 self.global_params.Phi[t] = self.global_params.Phi[t] / np.maximum(realmin, self.global_params.Phi[t].sum(0))
 
 
-    def train(self, data_1: np.ndarray, data_2: np.ndarray, iter_all: int=1, is_train: bool = True, is_initial_local=True):
+    def train(self, data_1: np.ndarray, data_2: np.ndarray, num_epochs: int=1, is_train: bool = True, is_initial_local=True):
         '''
         Inputs:
-            iter_all   : [int] scalar, the iterations of gibbs sampling
+            num_epochs   : [int] scalar, the iterations of gibbs sampling
             dataset       : [np.ndarray] V*N matrix, N bag-of-words vectors with a vocabulary of length V
             is_train   : [bool] True or False, whether to update the global params in the probabilistic model
 
         Attributes:
             @public:
                 local_params.Theta : [list] T (K_t)*(N) topic proportions at different layers
                 local_params.c_j   : [list] T+1 1*N vector, the variables in the scale parameter in the Theta
@@ -119,15 +119,15 @@
 
         Outputs:
             local_params  : [Params] the local parameters of the probabilistic model
 
         '''
         assert type(data_1) is np.ndarray and type(data_2) is np.ndarray, 'Data type error: the input dataset should be a 2-D np.ndarray'
         self._model_setting.N = data_1.shape[1]
-        self._model_setting.Iteration = iter_all
+        self._model_setting.Iteration = num_epochs
 
         # initial local params
         if is_initial_local or not hasattr(self.local_params, 'Theta') or not hasattr(self.local_params, 'c_j') or not hasattr(self.local_params, 'p_j'):
             self.local_params.Theta = []
             self.local_params.c_j = []
             for t in range(self._model_setting.T):  # from layer 1 to T
                 self.local_params.Theta.append(np.ones([self._model_setting.K[t], self._model_setting.N]) / self._model_setting.K[t])
@@ -200,25 +200,25 @@
             stages = 'Training' if is_train else 'Testing'
             print(f'{stages} Stage: ',
                   f'epoch {iter:3d} takes {end_time - start_time:.2f} seconds')
 
         return copy.deepcopy(self.local_params)
 
 
-    def test(self, data_1: np.ndarray, data_2: np.ndarray, iter_all: int=1, is_initial_local=True):
+    def test(self, data_1: np.ndarray, data_2: np.ndarray, num_epochs: int=1, is_initial_local=True):
         '''
         Inputs:
-            iter_all   : [int] scalar, the iterations of gibbs sampling
+            num_epochs   : [int] scalar, the iterations of gibbs sampling
             dataset       : [np.ndarray] V*N matrix, N bag-of-words vectors with a vocabulary of length V
 
         Outputs:
             local_params  : [Params] the local parameters of the probabilistic model
 
         '''
-        local_params = self.train(data_1, data_2, iter_all=iter_all, is_train=False, is_initial_local=is_initial_local)
+        local_params = self.train(data_1, data_2, num_epochs=num_epochs, is_train=False, is_initial_local=is_initial_local)
 
         return local_params
 
 
     def load(self, model_path: str):
         '''
         Load the model parameters from the specified directory
```

### Comparing `pydpm-4.0.2/pydpm/model/bayesian_gm/pfa.py` & `pydpm-5.0.0/pydpm/model/bayesian_pm/pfa.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,18 +81,18 @@
         self._hyper_params.Theta_r_k = np.ones([self._model_setting.K, 1]) / self._model_setting.K
         self._hyper_params.p_j_a0 = 0.01
         self._hyper_params.p_j_b0 = 0.01
         self._hyper_params.c_j_a0 = 1
         self._hyper_params.c_j_b0 = 1
 
 
-    def train(self, data: np.ndarray, iter_all: int=1, is_train: bool = True, is_initial_local: bool=True):
+    def train(self, data: np.ndarray, num_epochs: int=1, is_train: bool = True, is_initial_local: bool=True):
         '''
         Inputs:
-            iter_all   : [int] scalar, the iterations of gibbs sampling
+            num_epochs   : [int] scalar, the iterations of gibbs sampling
             dataset       : [np.ndarray] V*N matrix, N bag-of-words vectors with a vocabulary of length V
             is_train   : [bool] True or False, whether to update the global params in the probabilistic model
 
         Attributes:
             @public:
                 local_params.Theta    : [np.ndarray] N_train*K matrix, the topic propotions of N_train documents
                 local_params.c_j      : [np.ndarray] scalar,
@@ -104,15 +104,15 @@
 
         Outputs:
                 local_params  : [Params] the local parameters of the probabilistic model
 
         '''
         assert type(data) is np.ndarray, 'Data type error: the input dataset should be a 2-D np.ndarray'
         self._model_setting.N = data.shape[1]
-        self._model_setting.Iteration = iter_all
+        self._model_setting.Iteration = num_epochs
 
         # initial local parameters
         if is_initial_local or not hasattr(self.local_params, 'Theta') or not hasattr(self.local_params, 'c_j') or not hasattr(self.local_params, 'p_j'):
             self.local_params.Theta = np.ones([self._model_setting.K, self._model_setting.N]) / self._model_setting.K
             self.local_params.c_j = np.ones([1, self._model_setting.N])
             self.local_params.p_j = np.ones([1, self._model_setting.N])
 
@@ -139,25 +139,25 @@
             stages = 'Training' if is_train else 'Testing'
             print(f'{stages} Stage: ',
                   f'epoch {iter:3d} takes {end_time - start_time:.2f} seconds')
 
         return copy.deepcopy(self.local_params)
 
 
-    def test(self, data: np.ndarray, iter_all: int=1, is_initial_local: bool=True):
+    def test(self, data: np.ndarray, num_epochs: int=1, is_initial_local: bool=True):
         '''
         Inputs:
-            iter_all   : [int] scalar, the iterations of gibbs sampling
+            num_epochs   : [int] scalar, the iterations of gibbs sampling
             dataset       : [np.ndarray] V*N matrix, N bag-of-words vectors with a vocabulary of length V
 
         Outputs:
             local_params  : [Params] the local parameters of the probabilistic model
 
         '''
-        local_params = self.train(data, iter_all=iter_all, is_train=False, is_initial_local=is_initial_local)
+        local_params = self.train(data, num_epochs=num_epochs, is_train=False, is_initial_local=is_initial_local)
 
         return local_params
 
 
     def save(self, model_path: str = '../save_models'):
         '''
         Save the model to the specified directory.
```

### Comparing `pydpm-4.0.2/pydpm/model/bayesian_gm/pgbn.py` & `pydpm-5.0.0/pydpm/model/bayesian_pm/pgbn.py`

 * *Files 11% similar despite different names*

```diff
@@ -87,18 +87,18 @@
             if t == 0:
                 self.global_params.Phi.append(0.2 + 0.8 * np.random.rand(self._model_setting.V, self._model_setting.K[t]))
             else:
                 self.global_params.Phi.append(0.2 + 0.8 * np.random.rand(self._model_setting.K[t-1], self._model_setting.K[t]))
             self.global_params.Phi[t] = self.global_params.Phi[t] / np.maximum(realmin, self.global_params.Phi[t].sum(0))
 
 
-    def train(self, data:np.ndarray, iter_all: int=1, is_train: bool = True, is_initial_local: bool=True):
+    def train(self, data:np.ndarray, num_epochs: int=1, is_train: bool = True, is_initial_local: bool=True):
         '''
         Inputs:
-            iter_all   : [int] scalar, the iterations of gibbs sampling
+            num_epochs   : [int] scalar, the iterations of gibbs sampling
             dataset       : [np.ndarray] V*N matrix, N bag-of-words vectors with a vocabulary of length V
             is_train   : [bool] True or False, whether to update the global params in the probabilistic model
 
         Attributes:
             @public:
                 local_params.Theta : [list] T (K_t)*(N) topic proportions at different layers
                 local_params.c_j   : [list] T+1 1*N vector, the variables in the scale parameter in the Theta
@@ -110,15 +110,15 @@
 
         Outputs:
             local_params  : [Params] the local parameters of the probabilistic model
 
         '''
         assert type(data) is np.ndarray, 'Data type error: the input dataset should be a 2-D np.ndarray'
         self._model_setting.N = data.shape[1]
-        self._model_setting.Iteration = iter_all
+        self._model_setting.Iteration = num_epochs
 
         # initial local params
         if is_initial_local or not hasattr(self.local_params, 'Theta') or not hasattr(self.local_params, 'c_j') or not hasattr(self.local_params, 'p_j'):
             self.local_params.Theta = []
             self.local_params.c_j = []
             for t in range(self._model_setting.T):  # from layer 1 to T
                 self.local_params.Theta.append(np.ones([self._model_setting.K[t], self._model_setting.N]) / self._model_setting.K[t])
@@ -175,25 +175,25 @@
             stages = 'Training' if is_train else 'Testing'
             print(f'{stages} Stage: ',
                   f'epoch {iter:3d} takes {end_time - start_time:.2f} seconds')
 
         return copy.deepcopy(self.local_params)
 
 
-    def test(self, data: np.ndarray, iter_all: int=1, is_initial_local=True):
+    def test(self, data: np.ndarray, num_epochs: int=1, is_initial_local=True):
         '''
         Inputs:
-            iter_all   : [int] scalar, the iterations of gibbs sampling
+            num_epochs   : [int] scalar, the iterations of gibbs sampling
             dataset       : [np.ndarray] V*N matrix, N bag-of-words vectors with a vocabulary of length V
 
         Outputs:
             local_params  : [Params] the local parameters of the probabilistic model
 
         '''
-        local_params = self.train(data, iter_all=iter_all, is_train=False, is_initial_local=is_initial_local)
+        local_params = self.train(data, num_epochs=num_epochs, is_train=False, is_initial_local=is_initial_local)
 
         return local_params
 
 
     def load(self, model_path: str):
         '''
         Load the model parameters from the specified directory
```

### Comparing `pydpm-4.0.2/pydpm/model/bayesian_gm/pgds.py` & `pydpm-5.0.0/pydpm/model/bayesian_pm/pgds.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,18 +83,18 @@
         self.global_params.rou = np.zeros((self._model_setting.K, 1))
 
         self._hyper_params.tao0 = 1
         self._hyper_params.gamma0 = 100
         self._hyper_params.eta0 = 0.1
         self._hyper_params.epilson0 = 0.1
 
-    def train(self, data: np.ndarray, iter_all: int=1, is_train: bool = True, is_initial_local: bool=True):
+    def train(self, data: np.ndarray, num_epochs: int=1, is_train: bool = True, is_initial_local: bool=True):
         '''
         Inputs:
-            iter_all   : [int] scalar, the iterations of gibbs sampling
+            num_epochs   : [int] scalar, the iterations of gibbs sampling
             dataset       : [np.ndarray] V*N_train matrix, N_train bag-of-words vectors with a vocabulary length of V
             is_train   : [bool] True or False, whether to update the global params in the probabilistic model
 
         Attributes:
             @public:
                 local_params.Theta : [np.ndarray] N_train*K matrix, the topic propotions of N_train documents
 
@@ -118,15 +118,15 @@
 
         A_VK = np.zeros((self._model_setting.V, self._model_setting.K))
         A_KT = np.zeros((self._model_setting.K, self._model_setting.T))
         L_dotkt = np.zeros((self._model_setting.K, self._model_setting.T + 1))
         L_kdott = np.zeros((self._model_setting.K, self._model_setting.T + 1))
 
 
-        for iter in range(iter_all):
+        for iter in range(num_epochs):
 
             start_time = time.time()
 
             A_KT, A_VK = self._sampler.multi_aug(data, self.global_params.Phi, self.local_params.Theta)
 
             L_KK = np.zeros((self._model_setting.K, self._model_setting.K))
             for t in range(self._model_setting.T - 1, 0, -1):  # T-1 : 1
@@ -211,25 +211,25 @@
             stages = 'Training' if is_train else 'Testing'
             print(f'{stages} Stage: ',
                   f'epoch {iter:3d} takes {end_time - start_time:.2f} seconds. Likelihood:{like:8.3f}')
 
         return copy.deepcopy(self.local_params)
 
 
-    def test(self, data: np.ndarray, iter_all: int=1, is_initial_local: bool=True):
+    def test(self, data: np.ndarray, num_epochs: int=1, is_initial_local: bool=True):
         '''
         Inputs:
-            iter_all   : [int] scalar, the iterations of sampling
+            num_epochs   : [int] scalar, the iterations of sampling
             dataset       : [np.ndarray] V*N matrix, N bag-of-words vectors with a vocabulary of length V
 
         Outputs:
             local_params  : [Params] the local parameters of the probabilistic model
 
         '''
-        local_params = self.train(data, iter_all=iter_all, is_train=False, is_initial_local=is_initial_local)
+        local_params = self.train(data, num_epochs=num_epochs, is_train=False, is_initial_local=is_initial_local)
 
         return local_params
 
 
     def save(self, model_path: str = '../save_models'):
         '''
         Save the model to the specified directory.
```

### Comparing `pydpm-4.0.2/pydpm/model/bayesian_gm/wedtm.py` & `pydpm-5.0.0/pydpm/model/bayesian_pm/wedtm.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,20 +70,20 @@
                 _model_setting.V        : [int] scalar, the length of the vocabulary
 
         '''
         self._model_setting.V = data.shape[0]
         self.global_params.Phi = np.zeros((self._model_setting.K[0], self._model_setting.V)).astype(int)
 
 
-    def train(self, embeddings: np.ndarray, data: np.ndarray, S: int, iter_all: int=1, is_train: bool = True, is_initial_local: bool=True):
+    def train(self, embeddings: np.ndarray, data: np.ndarray, S: int, num_epochs: int=1, is_train: bool = True, is_initial_local: bool=True):
         '''
         Inputs:
             embeddings     : [np.ndarray] V*D, word embedding of training words
             S              : [int] sub topics
-            iter_all       : [np.ndarray] scalar, the iterations of gibbs sampling
+            num_epochs       : [np.ndarray] scalar, the iterations of gibbs sampling
             dataset           : [np.ndarray] V*N_train matrix, N_train bag-of-words vectors with a vocabulary length of V
             is_train       : [bool] True or False, whether to update the global params in the probabilistic model
 
         Attributes:
             @public:
 
                 local_params.Theta : [np.ndarray] N_train*K matrix, the topic propotions of N_train documents
@@ -94,15 +94,15 @@
 
         Outputs:
                 local_params  : [Params] the local parameters of the probabilistic model
 
         '''
         assert type(data) is np.ndarray, 'Data type error: the input dataset should be a 2-D np.ndarray'
 
-        self._model_setting.Iteration = [iter_all] * self._model_setting.T
+        self._model_setting.Iteration = [num_epochs] * self._model_setting.T
         self._model_setting.N = data.shape[1]
 
         # initial local paramters
         if is_initial_local or not hasattr(self.local_params, 'Theta'):
             self.local_params.Theta = np.zeros((self._model_setting.K[0], self._model_setting.N)).astype(int)
 
         # WS the trained words' word index
@@ -256,27 +256,27 @@
             paraGlobal[Tcurrent]['cjmedian'] = []
             for t in range(Tcurrent + 1):
                 paraGlobal[Tcurrent]['cjmedian'].append(np.median(c_j[t]))
 
         return copy.deepcopy(self.local_params)
 
 
-    def test(self, embeddings: np.ndarray, data: np.ndarray, S: int, iter_all: int=1, is_initial_local: bool=True):
+    def test(self, embeddings: np.ndarray, data: np.ndarray, S: int, num_epochs: int=1, is_initial_local: bool=True):
         '''
         Inputs:
             embeddings     : [np.ndarray] V*D, word embedding of training words
             S              : [int] number of sub topics
-            iter_all       : [np.ndarray] scalar, the iterations of gibbs sampling
+            num_epochs       : [np.ndarray] scalar, the iterations of gibbs sampling
             dataset           : [np.ndarray] V*N_train matrix, N_train bag-of-words vectors with a vocabulary length of V
 
         Outputs:
                 local_params  : [Params] the local parameters of the probabilistic model
 
         '''
-        local_params = self.train(embeddings, data, S, iter_all=iter_all, is_train=False, is_initial_local=is_initial_local)
+        local_params = self.train(embeddings, data, S, num_epochs=num_epochs, is_train=False, is_initial_local=is_initial_local)
 
         return local_params
 
 
     def save(self, model_path: str = '../save_models'):
         '''
         Save the model to the specified directory.
```

### Comparing `pydpm-4.0.2/pydpm/model/deep_learning_gm/gan.py` & `pydpm-5.0.0/pydpm/model/deep_learning_pm/wgan.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,113 +1,131 @@
 """
 ===========================================
-GAN
-Generative Adversarial Networks
-IJ Goodfellow，J Pouget-Abadie，M Mirza，B Xu，D Warde-Farley，S Ozair，A Courville，Y Bengio
-Publihsed in 2014
+WGAN
+Wasserstein GAN
+Martin Arjovsky, Soumith Chintala, and Leon Bottou,
+Publihsed in 2017
 
 ===========================================
 """
 
-# Author: Muyao Wang <flare935694542@163.com>, Xinyang Liu <lxy771258012@163.com>
+# Author: Bufeng Ge <20009100138@stu.xidian.edu.cn>, Xinyang Liu <lxy771258012@163.com>
 # License: BSD-3-Clause
 
 import numpy as np
 import torch.nn as nn
 import torch
 from torch.autograd import Variable
 from torchvision.utils import save_image
 from tqdm import tqdm
 import os
 
-class GAN(nn.Module):
-    def __init__(self, img_shape, g_latent_dim=100, z_dim=128, d_latent_dim=512, device='cuda:0'):
+class WGAN(nn.Module):
+    def __init__(self, img_shape, g_z_dim: int=100, g_hid_dims: list=[100, 200, 400, 800], d_hid_dims: list=[200, 100], device='cuda:0'):
         """
         The basic model for GAN
         Inputs:
             img_shape : [tuple] the size of input
-            g_latent_dim : [int] generator latent dimension;
-            z_dim : [int] the noise dimension
-            d_latent_dim : [int] discriminator latent dimension
+            g_z_dim : [int] the noise dimension
+            g_latent_dim : [list] generator latent dimension;
+            d_latent_dim : [list] discriminator latent dimension
             device : [str] 'cpu' or 'gpu';
         """
-        super(GAN, self).__init__()
-        setattr(self, '_model_name', 'GAN')
+        super(WGAN, self).__init__()
+        setattr(self, '_model_name', 'WGAN')
         self.img_shape = img_shape
-        self.g_latent_dim = g_latent_dim
-        self.d_latent_dim = d_latent_dim
-        self.generator = Generator(latent_dim = g_latent_dim, z_dim = z_dim, img_shape = self.img_shape).to(device)
-        self.discriminator = Discriminator(latent_dim = d_latent_dim, img_shape = self.img_shape).to(device)
-        self.adversarial_loss = torch.nn.BCELoss().to(device)
+        self.g_z_dim = g_z_dim
+        self.g_hid_dims = g_hid_dims
+        self.d_hid_dims = d_hid_dims
+        self.generator = Generator(img_shape=self.img_shape, z_dim=self.g_z_dim, hid_dims=self.g_hid_dims).to(device)
+        self.discriminator = Discriminator(img_shape=self.img_shape, hid_dims=self.d_hid_dims).to(device)
         self.device = device
         self.Tensor = torch.FloatTensor if self.device == 'cpu' else torch.cuda.FloatTensor
 
 
     def sample(self, batch_size):
         """
         Sample from generator
         Inputs:
             batch_size : [int] number of img which you want;
         Outputs:
             gen_imgs : [tensor] a batch of images
         """
         # Sample noise as generator input
-        z = torch.tensor(np.random.normal(0, 1, (batch_size, self.g_latent_dim))).to(self.device)
+        z = torch.tensor(np.random.normal(0, 1, (batch_size, self.g_z_dim))).to(self.device)
         # Generate a batch of images
         gen_imgs = self.generator(z)
         return gen_imgs
 
 
-    def train_one_epoch(self, model_opt_G, model_opt_D, dataloader, sample_interval, epoch, n_epochs):
+    def train_one_epoch(self, args, model_opt_G, model_opt_D, dataloader, epoch, n_epochs):
         '''
         Train for one epoch
         Inputs:
             model_opt_G     : Optimizer for generator
             model_opt_D     : Optimizer for discriminator
             dataloader      : Train dataset with form of dataloader
             sample_interval : interval betwen image samples while training
             epoch           : Current epoch on training stage
             n_epoch         : Total number of epochs on training stage
         '''
         G_loss_t, D_loss_t = 0, 0
-        g_loss_interval = 4
+        batches_done = 0
         train_bar = tqdm(iterable=dataloader)
         for i, (imgs, _) in enumerate(train_bar):
             train_bar.set_description(f'Epoch [{epoch}/{n_epochs}]')
-            train_bar.set_postfix(loss=G_loss_t / (i / g_loss_interval + 1), KL_loss=D_loss_t / (i + 1))
+            train_bar.set_postfix(G_loss=G_loss_t / (i / args.n_critic + 1), D_loss=D_loss_t / (i + 1))
 
             # Adversarial ground truths
-            valid = Variable(self.Tensor(imgs.size(0), 1).fill_(1.0), requires_grad=False).to(self.device)
-            fake = Variable(self.Tensor(imgs.size(0), 1).fill_(0.0), requires_grad=False).to(self.device)
             real_imgs = Variable(imgs.type(self.Tensor))
 
+            model_opt_D.zero_grad()
+
+            # Sample noise as generator input
+            fake_imgs = self.sample(imgs.shape[0])
+            # z = Variable(self.Tensor(np.random.normal(0, 1, (imgs.shape[0], self.g_z_dim))))
+            # # Generate a batch of images
+            # fake_imgs = self.generator(z)
+            # Adversarial loss
+            loss_D = -torch.mean(self.discriminator(real_imgs)) + torch.mean(self.discriminator(fake_imgs))
+
+            loss_D.backward()
+            model_opt_D.step()
+            D_loss_t += -loss_D.item()
+
             # Train Generator
             # Sample noise as generator input
-            z = Variable(self.Tensor(np.random.normal(0, 1, (imgs.shape[0], self.g_latent_dim))))
+            z = Variable(self.Tensor(np.random.normal(0, 1, (imgs.shape[0], self.g_z_dim))))
             # Generate a batch of images
             gen_imgs = self.generator(z)
-            if (i % g_loss_interval == 0):
+
+            # Clip weights of discriminator
+            for p in self.discriminator.parameters():
+                p.data.clamp_(-args.clip_value, args.clip_value)
+
+            if i % args.n_critic == 0:
+                # -----------------
+                #  Train Generator
+                # -----------------
+
                 model_opt_G.zero_grad()
-                g_loss = self.adversarial_loss(self.discriminator(gen_imgs), valid)
-                g_loss.backward()
+
+                # Generate a batch of images
+                gen_imgs = self.generator(z)
+                # Adversarial loss
+                loss_G = -torch.mean(self.discriminator(gen_imgs))
+
+                loss_G.backward()
                 model_opt_G.step()
-                G_loss_t += g_loss.item()
+                G_loss_t += -loss_G.item()
 
-            # Train Discriminator
-            model_opt_D.zero_grad()
-            real_loss = self.adversarial_loss(self.discriminator(real_imgs), valid)
-            fake_loss = self.adversarial_loss(self.discriminator(gen_imgs.detach()), fake)
-            d_loss = (real_loss + fake_loss) / 2
-            d_loss.backward()
-            model_opt_D.step()
-            D_loss_t += d_loss.item()
+            if batches_done % args.sample_interval == 0:
+                save_image(gen_imgs.data[:25], "../../output/images/%d.png" % batches_done, nrow=5, normalize=True)
+            batches_done += 1
 
-            batches_done = epoch * len(dataloader) + i
-            if batches_done % sample_interval == 0:
-                save_image(gen_imgs.data[:25], "../output/images/%d.png" % batches_done, nrow=5, normalize=True)
 
 
     def save(self, model_path: str = '../save_models'):
         """
         save model
         Inputs:
             model_path : [str] the path to save the model, default '../save_models/GAN.pth';
@@ -124,44 +142,51 @@
             model_path : [str] the path to load the model;
         """
         assert os.path.exists(model_path), 'Path Error: can not find the path to load the model'
         # Load the model
         checkpoint = torch.load(model_path)
         self.load_state_dict(checkpoint['state_dict'])
 
-
 class Generator(nn.Module):
-    def __init__(self, img_shape, latent_dim = 100, z_dim = 128):
+    def __init__(self, img_shape, z_dim: int=100, hid_dims: list=[100, 200, 400, 800]):
         """
         The basic model for generator
         Inputs:
             img_shape : [tuple] the size of input
             latent_dim : [int] generator latent dimension;
             z_dim : [int] the noise dimension
         """
         super(Generator, self).__init__()
-        self.latent_dim = latent_dim
-        self.z_dim = z_dim
         self.img_shape = img_shape
+        self.z_dim = z_dim
+        self.hid_dims = hid_dims
+        self.num_layers = len(self.hid_dims)
         def block(in_feat, out_feat, normalize=True):
             layers = [nn.Linear(in_feat, out_feat)]
             if normalize:
                 layers.append(nn.BatchNorm1d(out_feat, 0.8))
             layers.append(nn.LeakyReLU(0.2, inplace=True))
             return layers
 
+        self.Block = nn.ModuleList()
+        for layer_index in range(self.num_layers):
+            if layer_index == 0:
+                latent_layers = block(self.z_dim, self.hid_dims[layer_index], normalize=False)
+            else:
+                latent_layers = block(self.hid_dims[layer_index - 1], self.hid_dims[layer_index])
+            for i in range(len(latent_layers)):
+                self.Block.append(latent_layers[i])
+
         self.model = nn.Sequential(
-            *block(self.latent_dim, self.z_dim, normalize=False),
-            *block(self.z_dim, self.z_dim*2),
-            *block(self.z_dim*2, self.z_dim*4),
-            *block(self.z_dim*4, self.z_dim*8),
-            nn.Linear(self.z_dim*8, int(np.prod(self.img_shape))),
-            nn.Tanh()
+            *self.Block,
+            nn.Linear(self.hid_dims[-1], int(np.prod(self.img_shape))),
+            nn.Tanh(),
         )
 
+
     def forward(self, z):
         """
         Forward process of generator
         Inputs:
             z : [tuple] the size of input
         Outputs；
             img : [tensor] return the generated image
@@ -169,31 +194,38 @@
         z = z.float()
         img = self.model(z)
         img = img.view(img.size(0), *self.img_shape)
         return img
 
 
 class Discriminator(nn.Module):
-    def __init__(self, img_shape, latent_dim = 256):
+    def __init__(self, img_shape, hid_dims: list=[512, 256]):
         """
         The basic model for discriminator
         Inputs:
             img_shape : [tuple] the size of input
             latent_dim : [int] discriminator latent dimension;
         """
         super(Discriminator, self).__init__()
-        self.latent_dim = latent_dim
         self.img_shape = img_shape
+        self.hid_dims = hid_dims
+        self.num_layers = len(self.hid_dims)
+        self.Block = nn.ModuleList()
+
+        for layer_index in range(self.num_layers):
+            if layer_index == 0:
+                self.Block.append(nn.Linear(int(np.prod(self.img_shape)), self.hid_dims[layer_index]))
+            else:
+                self.Block.append(nn.Linear(self.hid_dims[layer_index - 1], self.hid_dims[layer_index]))
+            self.Block.append(nn.LeakyReLU(0.2, inplace=True))
+
+        self.Block.append(nn.Linear(self.hid_dims[-1], 1))
+
         self.model = nn.Sequential(
-            nn.Linear(int(np.prod(self.img_shape)), self.latent_dim*2),
-            nn.LeakyReLU(0.2, inplace=True),
-            nn.Linear(self.latent_dim*2, self.latent_dim ),
-            nn.LeakyReLU(0.2, inplace=True),
-            nn.Linear(self.latent_dim, 1),
-            nn.Sigmoid(),
+            *self.Block,
         )
 
     def forward(self, img):
         """
         Forward process of discriminator
         Inputs:
             img : [tensor] input image
```

### Comparing `pydpm-4.0.2/pydpm/model/deep_learning_gm/rbm.py` & `pydpm-5.0.0/pydpm/model/deep_learning_pm/rbm.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,32 +3,38 @@
 RBM
 A Practical Guide to Training
 Restricted Boltzmann Machines
 Geoffrey Hinton
 Publihsed in 2010
 ===========================================
 """
+# Author: Muyao Wang <flare935694542@163.com>, Xinyang Liu <lxy771258012@163.com>
+# License: BSD-3-Clause
+
+import os
+import numpy as np
+
 import torch
 import torch.utils.data
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.autograd import Variable
 
 
-
 class RBM(nn.Module):
     def __init__(self, n_vis=784, n_hin=500, k=5):
         """
-        The basic model for VAE
+        The basic model for RBM
         Inputs:
             n_vis : [int] number of visible units;
             n_hin : [int] number of latent units;
             k : [int] layers of RBM;
         """
         super(RBM, self).__init__()
+        setattr(self, '_model_name', 'RBM')
         self.W = nn.Parameter(torch.randn(n_hin, n_vis) * 1e-2)
         self.v_bias = nn.Parameter(torch.zeros(n_vis))
         self.h_bias = nn.Parameter(torch.zeros(n_hin))
         self.k = k
 
     def sample_from_p(self, p):
         """
@@ -93,36 +99,48 @@
             free_energy : [tensor] free energy of whole system
         """
         vbias_term = v.mv(self.v_bias)
         wx_b = F.linear(v, self.W, self.h_bias)
         hidden_term = wx_b.exp().add(1).log().sum(1)
         return (-hidden_term - vbias_term).mean()
 
-    def save(self, epoch, checkpoints):
+    # train and test
+    def train_one_epoch(self, dataloader, model_opt, epoch_idx, args):
+        loss_ = []
+        for batch_idx, (data, target) in enumerate(dataloader):
+            data = Variable(data.view(-1, 784))
+            sample_data = data.bernoulli()
+
+            v, v1 = self(sample_data)
+            loss = self.free_energy(v) - self.free_energy(v1)
+            loss_.append(loss.item())
+            model_opt.zero_grad()
+            loss.backward()
+            model_opt.step()
+        print('Train Epoch: {} Loss: {:.6f}'.format(epoch_idx, np.mean(loss_)))
+        return v, v1
+
+    # save and load
+    def save(self, model_path: str = '../save_models'):
         """
         save model
         Inputs:
-            epoch     : [int] train epoch;
-            checkpoints : [str] trained model path;
+            model_path : [str] the path to save the model, default '../save_models/RBM.pth';
         """
-        '======>>saving'
-        torch.save({'epoch': epoch ,
-                    'state_dict': self.state_dict()},
-                   checkpoints + '_epochs{}.pth'.format(epoch))
+        # create the directory path
+        if not os.path.isdir(model_path):
+            os.mkdir(model_path)
+
+        # Save the model
+        torch.save({'state_dict': self.state_dict()}, model_path + '/' + self._model_name + '.pth')
+        print('model has been saved by ' + model_path + '/' + self._model_name + '.pth')
 
-    def load(self, start_ep, checkpoints):
+    def load(self, model_path):
         """
         load model
         Inputs:
-            start_ep : [int] the epoch of checkpoint;
-            checkpoints : [str] trained model path;
+            model_path : [str] the path to load the model;
         """
-        try:
-            print("Loading Chechpoint from ' {} '".format(checkpoints + '_epochs{}.pth'.format(start_ep)))
-            checkpoint = torch.load(checkpoints + '_epochs{}.pth'.format(start_ep))
-            self.start_epoch = checkpoint['epoch']
-            self.load_state_dict(checkpoint['state_dict'])
-            print("Resuming Training From Epoch {}".format(self.start_epoch))
-            self.start_epoch = 0
-        except:
-            print("No Checkpoint Exists At '{}'".format(checkpoints))
-            self.start_epoch = 0
+        assert os.path.exists(model_path), 'Path Error: can not find the path to load the model'
+        # Load the model
+        checkpoint = torch.load(model_path)
+        self.load_state_dict(checkpoint['state_dict'])
```

### Comparing `pydpm-4.0.2/pydpm/model/deep_learning_gm/vae.py` & `pydpm-5.0.0/pydpm/model/deep_learning_pm/vae.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,206 +7,229 @@
 
 ===========================================
 """
 
 # Author: Muyao Wang <flare935694542@163.com>, Xinyang Liu <lxy771258012@163.com>
 # License: BSD-3-Clause
 
+import os
+import copy
+import numpy as np
+from tqdm import tqdm
+
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-import numpy as np
-from tqdm import tqdm
-import copy
-import os
 
 class VAE(nn.Module):
-    def __init__(self, x_dim, h_dim1, h_dim2, z_dim, device='cpu'):
+    def __init__(self, in_dim: int, z_dim: int, encoder_hid_dims: list, decoder_hid_dims: list, device: str='cpu'):
         """
         The basic model for VAE
         Inputs:
-            x_dim : [int] the size of input;
-            h_dim1 : [int] latent dimension1;
-            h_dim2 : [int] latent dimension2;
-            z_dim : [int] the normal distribution dimension;
+            in_dim : [int] dimension of input
+            encoder_hid_dims : [list] list of dimension in encoder
+            decoder_hid_dims : [list] list of dimension in decoder
+            z_dim : [int] dimension of the latent variable
             device : [str] 'cpu' or 'gpu';
         """
         super(VAE, self).__init__()
         setattr(self, '_model_name', 'VAE')
+        self.in_dim = in_dim
         self.z_dim = z_dim
-        self.x_dim = x_dim
+        self.encoder_hid_dims = encoder_hid_dims
+        self.decoder_hid_dims = decoder_hid_dims
         self.device = device
-        self.vae_encoder = VAE_Encoder(x_dim=x_dim, h_dim1=h_dim1, h_dim2=h_dim2, z_dim=z_dim, device=device)
-        self.vae_decoder = VAE_Decoder(x_dim=x_dim, h_dim1=h_dim1, h_dim2=h_dim2, z_dim=z_dim, device=device)
 
-    def compute_loss(self, recon_x, x, mu, log_var):
-        BCE = F.binary_cross_entropy(recon_x, x, reduction='sum')
-        KLD = -0.5 * torch.sum(1 + log_var - mu.pow(2) - log_var.exp())
-        return BCE, KLD
+        self.vae_encoder = VAE_Encoder(in_dim=self.in_dim, hid_dims=self.encoder_hid_dims, z_dim=self.z_dim, device=self.device)
+        self.vae_decoder = VAE_Decoder(in_dim=self.in_dim, hid_dims=self.decoder_hid_dims, z_dim=self.z_dim, device=self.device)
 
+    # forward
     def forward(self, x):
         """
         Forward process of VAE
         Inputs:
             x : [tensor] input tensor;
         Outputs:
             recon_x : [tensor] reconstruction of x
             mu : [tensor] mean of posterior distribution;
             log_var : [tensor] log variance of posterior distribution;
         """
         z, mu, log_var = self.vae_encoder(x.view(x.shape[0], -1))
         recon_x = self.vae_decoder(z)
         return recon_x, mu, log_var
 
-    def sample(self, batch_size):
-        """
-        Sample from generator
-        Inputs:
-            batch_size : [int] number of img which you want;
-        Outputs:
-            recon_x : [tensor] reconstruction of x
-        """
-        z = torch.randn(batch_size, self.z_dim).to(self.device)
-        recon_x = self.decoder(z)
-        return recon_x
-
-    def show(self):
-        """
-        Show the learned latent variables' effect
-        Outputs:
-            recon_x : [tensor] reconstruction of x
-        """
-        x, y = torch.meshgrid([torch.arange(-3, 3, 0.5), torch.arange(-3, 3, 0.5)])
-        z = torch.stack((x, y), 2).view(x.shape[0]**2, 2).to(self.device)
-        # z = torch.randn(batch_size, self.z_dim).to(self.device)
-        recon_x = self.decoder(z)
-        # print(recon_x.shape)
-        return recon_x
+    # loss
+    def compute_loss(self, recon_x, x, mu, log_var):
+        BCE = F.binary_cross_entropy(recon_x, x, reduction='sum')
+        KLD = -0.5 * torch.sum(1 + log_var - mu.pow(2) - log_var.exp())
+        return BCE, KLD
 
-    def train_one_epoch(self, model_opt, dataloader, epoch, n_epochs):
+    # train and test
+    def train_one_epoch(self, dataloader, model_opt, epoch_idx, args):
         '''
         Train for one epoch
         Inputs:
             model_opt  : Optimizer for model
             dataloader : Train dataset with form of dataloader
-            epoch      : Current epoch on training stage
-            n_epoch    : Total number of epochs on training stage
+            epoch_idx  : Current epoch on training stage
+            args       : Argument dict
 
         Attributes:
             local_mu      : Concatenation of mu with total dataset
             local_log_var : Concatenation of log_var with total dataset
         '''
-        self.train()
-        self.local_mu = None
-        self.local_log_var = None
+        local_mu = None
+        local_log_var = None
         loss_t, kl_loss_t, likelihood_t = 0, 0, 0
+
+        self.train()
         train_bar = tqdm(iterable=dataloader)
-        for i, (data, _) in enumerate(train_bar):
-            train_bar.set_description(f'Epoch [{epoch}/{n_epochs}]')
-            train_bar.set_postfix(loss=loss_t / (i + 1), KL_loss=kl_loss_t / (i + 1), likelihood=likelihood_t / (i + 1))
-            data = data.view(data.size(0), self.x_dim).to(self.device)
-            recon_x, mu, log_var = self.forward(data)
-            llh, kl_loss = self.compute_loss(recon_x, data, mu, log_var)
+        for batch_idx, (batch_x, _) in enumerate(train_bar):
+            # forward
+            batch_x = batch_x.view(batch_x.shape[0], self.in_dim).to(self.device)
+            recon_x, mu, log_var = self.forward(batch_x)
+            llh, kl_loss = self.compute_loss(recon_x, batch_x, mu, log_var)
             loss = llh + kl_loss
 
+            # backward
             loss.backward()
             model_opt.step()
             model_opt.zero_grad()
 
+            # accumulate loss
             loss_t += loss.item()
             kl_loss_t += kl_loss.item()
             likelihood_t += llh.item()
 
-            if self.local_mu is None:
-                self.local_mu = mu.cpu().detach().numpy()
-                self.local_log_var = log_var.cpu().detach().numpy()
+            # collect output
+            if local_mu is None:
+                local_mu = mu.cpu().detach().numpy()
+                local_log_var = log_var.cpu().detach().numpy()
             else:
-                self.local_mu = np.concatenate((self.local_mu, mu.cpu().detach().numpy()))
-                self.local_log_var = np.concatenate((self.local_log_var, log_var.cpu().detach().numpy()))
+                local_mu = np.concatenate((local_mu, mu.cpu().detach().numpy()))
+                local_log_var = np.concatenate((local_log_var, log_var.cpu().detach().numpy()))
 
-        return copy.deepcopy(self.local_mu), copy.deepcopy(self.local_log_var)
+            # tqdm
+            train_bar.set_description(f'Epoch [{epoch_idx}/{args.num_epochs}]')
+            train_bar.set_postfix(loss=loss_t / (batch_idx + 1), KL_loss=kl_loss_t / (batch_idx + 1), likelihood=likelihood_t / (batch_idx + 1))
+
+        return copy.deepcopy(local_mu), copy.deepcopy(local_log_var)
 
     def test_one_epoch(self, dataloader):
         '''
         Test for one epoch
         Inputs:
             dataloader : Train dataset with form of dataloader
 
         Attributes:
             local_mu      : Concatenation of mu with total dataset
             local_log_var : Concatenation of log_var with total dataset
         '''
-        self.eval()
         local_mu = None
         local_log_var = None
         loss_t, kl_loss_t, likelihood_t = 0, 0, 0
+
+        self.eval()
         with torch.no_grad():
             test_bar = tqdm(iterable=dataloader)
-            for i, (data, _) in enumerate(test_bar):
+            for i, (batch_x, _) in enumerate(test_bar):
                 test_bar.set_description(f'Testing stage: ')
                 test_bar.set_postfix(loss=loss_t / (i + 1), KL_loss=kl_loss_t / (i + 1), likelihood=likelihood_t / (i + 1))
-                data = data.view(data.size(0), self.x_dim).to(self.device)
-                recon_x, mu, log_var = self.forward(data)
-                llh, kl_loss = self.compute_loss(recon_x, data, mu, log_var)
+
+                # forward
+                batch_x = batch_x.view(batch_x.shape[0], self.in_dim).to(self.device)
+                recon_x, mu, log_var = self.forward(batch_x)
+                llh, kl_loss = self.compute_loss(recon_x, batch_x, mu, log_var)
+
+                # accumulate loss
                 loss_t += (llh.item() + kl_loss.item())
                 kl_loss_t += kl_loss.item()
                 likelihood_t += llh.item()
 
+                # collect output
                 if local_mu is None:
                     local_mu = mu.cpu().detach().numpy()
                     local_log_var = log_var.cpu().detach().numpy()
                 else:
                     local_mu = np.concatenate((local_mu, mu.cpu().detach().numpy()))
                     local_log_var = np.concatenate((local_log_var, log_var.cpu().detach().numpy()))
 
         return local_mu, local_log_var
 
+    # save and load
     def save(self, model_path: str = '../save_models'):
         """
         save model
         Inputs:
             model_path : [str] the path to save the model, default '../save_models/VAE.pth';
         """
+        # create the directory path
+        if not os.path.isdir(model_path):
+            os.mkdir(model_path)
+
         # Save the model
         torch.save({'state_dict': self.state_dict()}, model_path + '/' + self._model_name + '.pth')
         print('model has been saved by ' + model_path + '/' + self._model_name + '.pth')
 
-
     def load(self, model_path):
         """
         load model
         Inputs:
             model_path : [str] the path to load the model;
         """
         assert os.path.exists(model_path), 'Path Error: can not find the path to load the model'
         # Load the model
         checkpoint = torch.load(model_path)
         self.load_state_dict(checkpoint['state_dict'])
 
-class VAE_Encoder(nn.Module):
-    def __init__(self, x_dim: int, h_dim1: int, h_dim2: int, z_dim: int, device: str='cpu'):
-        super(VAE_Encoder, self).__init__()
-        self.device = device
-        self.fc1 = nn.Linear(x_dim, h_dim1).to(self.device)
-        self.fc2 = nn.Linear(h_dim1, h_dim2).to(self.device)
-        self.fc31 = nn.Linear(h_dim2, z_dim).to(self.device)
-        self.fc32 = nn.Linear(h_dim2, z_dim).to(self.device)
-
-    def encoder(self, x):
+    # visualization
+    def sample(self, batch_size):
         """
-        Encode x to latent distribution
+        Sample from generator
         Inputs:
-            x : [tensor] the input tensor;
+            batch_size : [int] number of img which you want;
         Outputs:
-            mu : [tensor] mean of posterior distribution;
-            log_var : [tensor] log variance of posterior distribution;
+            recon_x : [tensor] reconstruction of x
         """
-        h = F.relu(self.fc1(x))
-        h = F.relu(self.fc2(h))
-        return self.fc31(h), self.fc32(h)  # mu, log_var
+        z = torch.randn(batch_size, self.z_dim).to(self.device)
+        recon_x = self.vae_decoder(z)
+        return recon_x
+
+    # def show(self):
+    #     """
+    #     Show the learned latent variables' effect
+    #     Outputs:
+    #         recon_x : [tensor] reconstruction of x
+    #     """
+    #     x, y = torch.meshgrid([torch.arange(-3, 3, 0.5), torch.arange(-3, 3, 0.5)])
+    #     z = torch.stack((x, y), 2).view(x.shape[0]**2, 2).to(self.device)
+    #     # z = torch.randn(batch_size, self.z_dim).to(self.device)
+    #     recon_x = self.vae_decoder(z)
+    #     # print(recon_x.shape)
+    #     return recon_x
+
+class VAE_Encoder(nn.Module):
+    def __init__(self, in_dim: int, hid_dims: list, z_dim: int, device: str='cpu'):
+        super(VAE_Encoder, self).__init__()
+
+        self.in_dim = in_dim
+        self.hid_dims = hid_dims
+        self.z_dim = z_dim
+        self.device = device
+        self.num_layers = len(self.hid_dims)
+
+        self.fc_encoder = nn.ModuleList()
+        self.fc_mu = nn.Linear(self.hid_dims[-1], self.z_dim, device=self.device)
+        self.fc_var = nn.Linear(self.hid_dims[-1], self.z_dim, device=self.device)
+
+        for layer_index in range(self.num_layers):
+            if layer_index == 0:
+                self.fc_encoder.append(nn.Linear(self.in_dim, self.hid_dims[layer_index]).to(device))
+            else:
+                self.fc_encoder.append(nn.Linear(self.hid_dims[layer_index - 1], self.hid_dims[layer_index]).to(device))
 
     def reparameterize(self, mu, log_var):
         """
         Gaussian re_parameterization
         Inputs:
             mu : [tensor] mean of posterior distribution;
             log_var : [tensor] log variance of posterior distribution;
@@ -223,43 +246,52 @@
         Inputs:
             x : [tensor] input tensor;
         Outputs:
             z : [tensor] latent variable of x
             mu : [tensor] mean of posterior distribution;
             log_var : [tensor] log variance of posterior distribution;
         """
-        mu, log_var = self.encoder(x.view(x.shape[0],-1))
+        x = x.view(x.shape[0], -1)
+        for layer_index in range(self.num_layers):
+            if layer_index == 0:
+                x = F.relu(self.fc_encoder[layer_index](x))
+            else:
+                x = F.relu(self.fc_encoder[layer_index](x))
+        mu = self.fc_mu(x)
+        log_var = self.fc_var(x)
+
         z = self.reparameterize(mu, log_var)
 
         return z, mu, log_var
 
 
 class VAE_Decoder(nn.Module):
-    def __init__(self, x_dim, h_dim1, h_dim2, z_dim, device: str='cpu'):
+    def __init__(self, in_dim: int, hid_dims: list, z_dim: int, device: str='cpu'):
         super(VAE_Decoder, self).__init__()
+
+        self.in_dim = in_dim
+        self.hid_dims = hid_dims
+        self.z_dim = z_dim
+        self.num_layers = len(self.hid_dims)
         self.device = device
-        self.fc4 = nn.Linear(z_dim, h_dim2).to(self.device)
-        self.fc5 = nn.Linear(h_dim2, h_dim1).to(self.device)
-        self.fc6 = nn.Linear(h_dim1, x_dim).to(self.device)
 
-    def decoder(self, z):
-        """
-        Reconstruct from the z
-        Inputs:
-            z : [tensor] latent variable of x
-        Outputs:
-            recon_x : [tensor] the reconstruction of x
-        """
-        h = F.relu(self.fc4(z))
-        h = F.relu(self.fc5(h))
-        return torch.sigmoid(self.fc6(h))  # recon_x
+        self.fc_decoder = nn.ModuleList()
+        for layer_index in range(self.num_layers):
+            if layer_index == 0:
+                self.fc_decoder.append(nn.Linear(self.z_dim, self.hid_dims[layer_index]).to(device))
+            else:
+                self.fc_decoder.append(nn.Linear(self.hid_dims[layer_index - 1], self.hid_dims[layer_index]).to(device))
+        self.fc_decoder.append(nn.Linear(self.hid_dims[-1], self.in_dim).to(device))
 
     def forward(self, z):
         """
         Forward process of VAE_Decoder
         Inputs:
             z : [tensor] latent variable of x;
         Outputs:
             recon_x : [tensor] reconstruction of x
         """
-        recon_x = self.decoder(z)
+        for layer_index in range(self.num_layers):
+            z = F.relu(self.fc_decoder[layer_index](z))
+        recon_x = torch.sigmoid(self.fc_decoder[-1](z))
+
         return recon_x
```

### Comparing `pydpm-4.0.2/pydpm/model/hybrid_gm/wgaae.py` & `pydpm-5.0.0/pydpm/model/hybrid_pm/wgaae.py`

 * *Files identical despite different names*

### Comparing `pydpm-4.0.2/pydpm/model/hybrid_gm/whai.py` & `pydpm-5.0.0/pydpm/model/hybrid_pm/whai.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from ..basic_model import Basic_Model
 from ...sampler import Basic_Sampler
 from ...utils import *
 
 warnings.filterwarnings("ignore")
 
 class WHAI(Basic_Model, nn.Module):
-    def __init__(self, in_dim: int, z_dims: list, hid_dims: list, device: str='cpu'):
+    def __init__(self, in_dim: int, z_dims: list, hid_dims: list, device: str='cpu', encode_prior=False):
         """
         The basic model for WHAI
         Inputs:
             in_dims     : [int] Length of the vocabulary for convolutional layers in WHAI;
             z_dims      : [list] Number of topics at different layers in WHAI;
             h_dims      : [list] Size of dimension at different hidden layers in WHAI;
             device      : [str] 'cpu' or 'gpu';
@@ -58,26 +58,28 @@
         super(WHAI, self).__init__()
         setattr(self, '_model_name', 'WHAI')
         self._model_setting.in_dim = in_dim
         self._model_setting.z_dims = z_dims
         self._model_setting.hid_dims = hid_dims
         self._model_setting.num_layers = len(self._model_setting.z_dims)
         self._model_setting.device = device
+        self.encode_prior = encode_prior
 
         self.real_min = torch.tensor(2.2e-10, device=self._model_setting.device)
 
         self.initial()
 
     def initial(self):
         _model_setting = self._model_setting
-        self.whai_encoder = WHAI_Encoder(_model_setting.in_dim, _model_setting.z_dims, _model_setting.hid_dims, _model_setting.device)
+        self.whai_encoder = WHAI_Encoder(_model_setting.in_dim, _model_setting.z_dims, _model_setting.hid_dims, _model_setting.device, encode_prior=self.encode_prior)
         self.whai_decoder = WHAI_Decoder(_model_setting.in_dim, _model_setting.z_dims, _model_setting.device)
         self.global_params = self.whai_decoder.global_params
         self._hyper_params = self.whai_decoder._hyper_params
 
+    # loss
     def log_max(self, x: torch.Tensor):
         '''
         return log(x+eps)
         '''
         return torch.log(torch.max(x, self.real_min))
 
     def KL_GamWei(self, Gam_shape: torch.Tensor, Gam_scale: torch.Tensor, Wei_shape: torch.Tensor, Wei_scale: torch.Tensor):
@@ -111,138 +113,123 @@
 
         x = x.permute([1, 0])
         re_x = torch.matmul(torch.tensor(phi[0], dtype=torch.float32, device=self._model_setting.device), theta[0])
         likelihood = torch.sum(x * self.log_max(re_x) - re_x - torch.lgamma(x + 1))
 
         return -(likelihood + kl_term) / x.shape[1], likelihood, likelihood + kl_term
 
-    def train_one_epoch(self, dataloader: DataLoader, optim: Optimizer, epoch_index, args=None, is_train=True):
+    # train and test
+    def train_one_epoch(self, dataloader: DataLoader, optim: Optimizer, epoch_idx: int, is_train=True, args=None):
         '''
         Train for one epoch
         Inputs:
             dataloader  : Train dataset with form of dataloader
             optim       : Optimizer for model
             epoch_index : [int] Current epoch on training stage
             args        : Hyper-parameters
             is_train    : [bool] True or False, whether to update the global params in the probabilistic model
 
         Attributes:
             local_params.theta : Concatenation of theta with total dataset
         '''
         loss_t, likelihood_t, elbo_t = 0.0, 0.0, 0.0
-
-        # if is_train:
-        #     self.train()
-        # else:
-        #     self.eval()
-        self.train()
         if hasattr(self.local_params, 'Theta'):
             delattr(self.local_params, 'Theta')
 
+        if is_train:
+            self.train()
+        else:
+            self.eval()
         train_bar = tqdm(iterable=dataloader)
-        for i, (train_data, train_label) in enumerate(train_bar):
-
+        for batch_idx, (train_data, train_label) in enumerate(train_bar):
+            # forward
             theta, k, l = self.whai_encoder(torch.tensor(train_data, dtype=torch.float, device=self._model_setting.device), self.global_params.Phi, self.training)
 
             if is_train:
                 args.MBratio = len(dataloader)
                 self.global_params.Phi = self.whai_decoder.update_phi(np.transpose(train_data), theta, args)
 
             loss, likelihood, elbo = self.loss(torch.tensor(train_data, dtype=torch.float, device=self._model_setting.device), self.global_params.Phi, theta, k, l)
 
+            # backward
             optim.zero_grad()
             loss.backward()
             optim.step()
 
+            # accumulate loss
             loss_t += loss.item()
             likelihood_t += likelihood.item()
             elbo_t += elbo.item()
 
+            # collect output
             if not hasattr(self.local_params, 'Theta'):
                 self.local_params.Theta = [0 for _ in range(self._model_setting.num_layers)]
                 for t in range(self._model_setting.num_layers):
                     self.local_params.Theta[t] = theta[t].cpu().detach().numpy().T
             else:
                 for t in range(self._model_setting.num_layers):
                     self.local_params.Theta[t] = np.concatenate((self.local_params.Theta[t], theta[t].cpu().detach().numpy().T))
 
-            train_bar.set_description(f'Epoch [{epoch_index}/{args.num_epochs}]')
-            train_bar.set_postfix(loss=loss_t / (i + 1), likelihood=likelihood_t / (i + 1), elbo=elbo_t / (i + 1))
+            # tqdm
+            train_bar.set_description(f'Epoch [{epoch_idx}/{args.num_epochs}]')
+            train_bar.set_postfix(loss=loss_t / (batch_idx + 1), likelihood=likelihood_t / (batch_idx + 1), elbo=elbo_t / (batch_idx + 1))
 
         return copy.deepcopy(self.local_params)
 
     def test_one_epoch(self, dataloader: DataLoader, args=None):
         '''
         Test for one epoch
         Inputs:
             dataloader : Test dataset with form of dataloader
 
         Attributes:
             local_params.data  : Concatenation of total dataset
             local_params.theta : Concatenation of theta with total dataset
             local_params.label : Concatenation of label with total dataset
         '''
-        self.eval()
         if hasattr(self.local_params, 'data'):
             delattr(self.local_params, 'Theta')
             delattr(self.local_params, 'data')
             delattr(self.local_params, 'label')
         loss_t, likelihood_t, elbo_t = 0.0, 0.0, 0.0
 
+        self.eval()
         test_bar = tqdm(iterable=dataloader)
         with torch.no_grad():
-            for i, (test_data, test_label) in enumerate(test_bar):
-                test_bar.set_description(f'Testing stage: ')
-                test_bar.set_postfix(loss=loss_t / (i + 1), likelihood=likelihood_t / (i + 1), elbo=elbo_t / (i + 1))
-
-
+            for batch_idx, (test_data, test_label) in enumerate(test_bar):
+                # forward
                 theta, k, l = self.whai_encoder(torch.tensor(test_data, dtype=torch.float, device=self._model_setting.device), self.global_params.Phi, self.training)
-
                 loss, likelihood, elbo = self.loss(torch.tensor(test_data, dtype=torch.float, device=self._model_setting.device), self.global_params.Phi, theta, k, l)
 
+                # accumulate loss
                 loss_t += loss.item()
                 likelihood_t += likelihood.item()
                 elbo_t += elbo.item()
 
+                # collect output
                 if not hasattr(self.local_params, 'Theta') or not hasattr(self.local_params, 'data') or not hasattr(self.local_params, 'label'):
                     self.local_params.Theta = [0 for _ in range(self._model_setting.num_layers)]
                     self.local_params.data = test_data.cpu().detach().numpy()
                     self.local_params.label = test_label.cpu().detach().numpy()
                     for t in range(self._model_setting.num_layers):
                         self.local_params.Theta[t] = theta[t].cpu().detach().numpy().T
                 else:
                     for t in range(self._model_setting.num_layers):
                         self.local_params.Theta[t] = np.concatenate(
                             (self.local_params.Theta[t], theta[t].cpu().detach().numpy().T))
                     self.local_params.data = np.concatenate((self.local_params.data, test_data.cpu().detach().numpy()))
                     self.local_params.label = np.concatenate((self.local_params.label, test_label.cpu().detach().numpy()))
 
-        return copy.deepcopy(self.local_params)
-
-
-    def load(self, checkpoint_path: str, directory_path: str):
-        '''
-        Load the model parameters from the checkpoint and the specified directory.
-        Inputs:
-            model_path : [str] the path to load the model.
-
-        '''
-        assert os.path.exists(checkpoint_path), 'Path Error: can not find the path to load the checkpoint'
-        assert os.path.exists(directory_path), 'Path Error: can not find the path to load the directory'
-
-        # load parameters of neural network
-        checkpoint = torch.load(checkpoint_path)
-        self.load_state_dict(checkpoint['state_dict'])
+                # tqdm
+                test_bar.set_description(f'Testing stage: ')
+                test_bar.set_postfix(loss=loss_t / (batch_idx + 1), likelihood=likelihood_t / (batch_idx + 1), elbo=elbo_t / (batch_idx + 1))
 
-        # load parameters of basic model
-        model = np.load(directory_path, allow_pickle=True).item()
-        for params in ['global_params', 'local_params', '_model_setting', '_hyper_params']:
-            if params in model:
-                setattr(self, params, model[params])
+        return copy.deepcopy(self.local_params)
 
+    # save and load
     def save(self, model_path: str = '../save_models'):
         '''
         Save the model to the checkpoint the specified directory.
         Inputs:
             model_path : [str] the path to save the model, default '../save_models/WHAI.npy' and '../save_models/WHAI.pth'
         '''
         # create the trained model path
@@ -259,14 +246,34 @@
             if params in dir(self):
                 model[params] = getattr(self, params)
         model['_model_setting'].device = self._model_setting.device
 
         np.save(model_path + '/' + self._model_name + '.npy', model)
         print('parameters of basic model have been saved by ' + model_path + '/' + self._model_name + '.npy')
 
+    def load(self, checkpoint_path: str, directory_path: str):
+        '''
+        Load the model parameters from the checkpoint and the specified directory.
+        Inputs:
+            model_path : [str] the path to load the model.
+
+        '''
+        assert os.path.exists(checkpoint_path), 'Path Error: can not find the path to load the checkpoint'
+        assert os.path.exists(directory_path), 'Path Error: can not find the path to load the directory'
+
+        # load parameters of neural network
+        checkpoint = torch.load(checkpoint_path)
+        self.load_state_dict(checkpoint['state_dict'])
+
+        # load parameters of basic model
+        model = np.load(directory_path, allow_pickle=True).item()
+        for params in ['global_params', 'local_params', '_model_setting', '_hyper_params']:
+            if params in model:
+                setattr(self, params, model[params])
+
 
 class Conv1D(nn.Module):
     def __init__(self, in_dim: int, out_dim: int, kernel_size: int=1, device: str='cpu'):
         '''
         convolutional layer
         Inputs:
             in_dim      : [int] Number of channels in the input image
@@ -310,15 +317,15 @@
             x = torch.mm(x.view(-1, x.size(-1)), self.W) + self.b
             x = x.view(x.size()[:-1] + (self.out_dim,))
         else:
             raise NotImplementedError
         return x
 
 class WHAI_Encoder(nn.Module):
-    def __init__(self, in_dim: int, z_dims: list, hid_dims: list, device: str = 'cpu'):
+    def __init__(self, in_dim: int, z_dims: list, hid_dims: list, device: str = 'cpu', encode_prior=False):
         '''
         Inputs:
             in_dims     : [int] Length of the vocabulary for convolutional layers in WHAI;
             z_dims      : [list] Number of topics at different layers in WHAI;
             h_dims      : [list] Size of dimension at different hidden layers in WHAI;
             device      : [str] 'cpu' or 'gpu';
 
@@ -331,14 +338,15 @@
 
         self.in_dim = in_dim
         self.z_dims = z_dims
         self.hid_dims = hid_dims
         self.num_layers = len(z_dims)
         self.device = device
         self.real_min = torch.tensor(2.2e-10, device=self.device)
+        self.encode_prior = encode_prior
 
         self.h_encoders = nn.ModuleList([Conv1D(in_dim, out_dim, 1, self.device) for in_dim, out_dim in zip([self.in_dim] + self.hid_dims[:-1], self.hid_dims)])
         self.shape_encoders = nn.ModuleList([Conv1D(h_dim, 1, 1, self.device) for h_dim in self.hid_dims])
         self.scale_encoders = nn.ModuleList([Conv1D(h_dim, z_dim, 1, self.device) for z_dim, h_dim in zip(self.z_dims, self.hid_dims)])
 
     def log_max(self, x: torch.Tensor):
         '''
@@ -373,16 +381,18 @@
             k           : [Tensor] Shape parameter of Weibull distribution
             l           : [Tensor] Scale parameter of Weibull distribution
         '''
         k_tmp = torch.max(torch.exp(self.shape_encoders[layer_index](x)), self.real_min).view(-1, 1)
         k_tmp = k_tmp.repeat(1, self.z_dims[layer_index])
         l = torch.max(torch.exp(self.scale_encoders[layer_index](x)), self.real_min)
         if layer_index != self.num_layers - 1:
-            # k = torch.max(k_tmp + torch.matmul(torch.tensor(phi, dtype=torch.float32, device=self.device), theta).permute(1, 0), self._real_min).to(self.device)
-            k = torch.max(k_tmp, self.real_min)
+            if self.encode_prior:
+                k = torch.max(k_tmp + torch.matmul(torch.tensor(phi, dtype=torch.float32, device=self.device), theta).permute(1, 0), self.real_min)
+            else:
+                k = torch.max(k_tmp, self.real_min)
         else:
             k = torch.max(k_tmp, self.real_min)
         return k.permute(1, 0), l.permute(1, 0)
 
     def reparameterize(self, Wei_shape: torch.Tensor, Wei_scale: torch.Tensor, layer_index: int):
         '''
         Reparameterization trick for Weibull distribution
```

### Comparing `pydpm-4.0.2/pydpm/sampler/basic_sampler.py` & `pydpm-5.0.0/pydpm/sampler/basic_sampler.py`

 * *Files identical despite different names*

### Comparing `pydpm-4.0.2/pydpm/sampler/distribution_sampler_cpu.py` & `pydpm-5.0.0/pydpm/sampler/distribution_sampler_cpu.py`

 * *Files identical despite different names*

### Comparing `pydpm-4.0.2/pydpm/sampler/distribution_sampler_gpu.py` & `pydpm-5.0.0/pydpm/sampler/distribution_sampler_gpu.py`

 * *Files identical despite different names*

### Comparing `pydpm-4.0.2/pydpm/sampler/model_sampler_cpu.py` & `pydpm-5.0.0/pydpm/sampler/model_sampler_cpu.py`

 * *Files identical despite different names*

### Comparing `pydpm-4.0.2/pydpm/sampler/model_sampler_gpu.py` & `pydpm-5.0.0/pydpm/sampler/model_sampler_gpu.py`

 * *Files identical despite different names*

### Comparing `pydpm-4.0.2/pydpm/sampler/pre_process.py` & `pydpm-5.0.0/pydpm/sampler/pre_process.py`

 * *Files identical despite different names*

### Comparing `pydpm-4.0.2/pydpm/utils/utils.py` & `pydpm-5.0.0/pydpm/utils/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -43,7 +43,13 @@
     cos_AB[(np.arange(N), np.arange(N))] = 1
     return cos_AB
 
 def standardization(data):
     mu = np.mean(data, axis=1, keepdims=True)
     sigma = np.std(data, axis=1, keepdims=True)
     return (data - mu) / (sigma + 2.2e-8)
+
+def normalize_to_neg_one_to_one(img):
+    return img * 2 - 1
+
+def unnormalize_to_zero_to_one(t):
+    return (t + 1) * 0.5
```

### Comparing `pydpm-4.0.2/setup.py` & `pydpm-5.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 
 from setuptools import setup, find_packages
 
 
 setup(
     name='pydpm',
-    version='4.0.2',
+    version='5.0.0',
     description='A python library focuses on constructing deep probabilistic models on GPU.',
     py_modules=['pydpm'],
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Chaojie Wang, Wei Zhao, Xinyang Liu, Jiawen Wu',
     author_email='xd_silly@163.com',
     maintainer='BoChenGroup',
```

