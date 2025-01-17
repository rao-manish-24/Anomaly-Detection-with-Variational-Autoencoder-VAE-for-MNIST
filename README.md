
# Anomaly Detection with Variational Autoencoder (VAE) for MNIST

This project demonstrates anomaly detection using a Variational Autoencoder (VAE) on the MNIST dataset. 

## Overview

The goal is to train a VAE to learn the distribution of "normal" handwritten digits (0-4) and then use it to identify "anomalous" digits (5-9). 

The project follows these key steps:
1. **Data Preparation:** Loads the MNIST dataset, splits it into train, validation, and test sets. Normal digits (0-4) are used for training and validation, while the test set includes both normal and anomalous digits.
2. **VAE Model:** Defines a simple VAE architecture with an encoder and a decoder.
3. **Training:** Trains the VAE using the reconstruction loss and KL divergence.
4. **Validation & Threshold:** Computes reconstruction errors on the validation set to determine a threshold for anomaly detection.
5. **Testing & Evaluation:** Evaluates the model's performance on the test set using metrics like precision, recall, F1-score, and ROC AUC.
6. **Visualization:** Visualizes original and reconstructed images for qualitative analysis.

## Requirements

* Python 3.6+
* PyTorch 1.7+
* Torchvision
* Scikit-learn
* Matplotlib
* NumPy
