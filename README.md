# GAN, VAE, WGAN, and SSGAN Project

## Introduction

This project explores various generative models including GAN, VAE, WGAN, and SSGAN. The goal is to understand and implement these models using PyTorch and evaluate their performance on image datasets.

## Models Implemented

### 1. Generative Adversarial Network (GAN)
- **Objective:** To generate realistic images by training a generator and discriminator in a competitive setting.
- **Components:**
  - **Generator:** Produces images from random noise.
  - **Discriminator:** Distinguishes between real and generated images.

### 2. Variational Autoencoder (VAE)
- **Objective:** To encode images into a latent space and decode them back to images.
- **Components:**
  - **Encoder:** Maps input images to a latent space.
  - **Decoder:** Reconstructs images from latent vectors.

### 3. Wasserstein GAN (WGAN)
- **Objective:** To improve GAN training stability using the Wasserstein distance.
- **Components:**
  - Similar to GAN but with a different loss function to ensure smoother training.

### 4. Semi-Supervised GAN (SSGAN)
- **Objective:** To leverage both labeled and unlabeled data for training.
- **Components:**
  - Combines the principles of GAN with semi-supervised learning techniques.

## Dataset

The project uses a custom dataset loaded from `.npz` files. The dataset is preprocessed and split into training and testing sets.

## Installation

To run the project, ensure you have the following dependencies installed:
- PyTorch
- torchvision
- pytorch-fid
- torchinfo

You can install the required packages using pip:
```bash
pip install torch torchvision pytorch-fid torchinfo
```

## Usage

1. **Data Preparation:**
   - Load the dataset using the provided functions.
   - Save a subset of real images for FID calculation.

2. **Model Training:**
   - Train each model using the respective training scripts.
   - Monitor the training process and evaluate the models using FID scores.

3. **Evaluation:**
   - Generate images using the trained models.
   - Calculate FID scores to assess the quality of generated images.

## Results

The project demonstrates the effectiveness of different generative models in producing realistic images. The FID scores indicate the quality of the generated images, with lower scores representing better quality.

## Conclusion

This project provides insights into the implementation and evaluation of various generative models. By experimenting with different architectures and training techniques, we can improve the quality of generated images.
