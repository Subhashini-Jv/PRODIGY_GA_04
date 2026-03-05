# Image-to-Image Translation using cGAN (pix2pix)
# Overview

This project implements an Image-to-Image Translation model using a Conditional Generative Adversarial Network (cGAN) based on the pix2pix architecture. The model learns to translate an input image from one domain to another using paired training data.

The generator network produces translated images, while the discriminator evaluates whether the generated images are realistic or fake. Both networks are trained simultaneously in an adversarial setting.

# Objectives

Implement Conditional GAN (cGAN) for image-to-image translation

Train a model that converts input images into corresponding target images

Understand adversarial training using generator and discriminator networks

# Dataset

This project uses the Facades dataset, commonly used for pix2pix models.

Dataset contains paired images:

Input Image: Building label map

Target Image: Real building photograph

Each dataset image contains the input and target images combined side-by-side.

# Model Architecture
# Generator

Based on U-Net architecture

Uses encoder-decoder layers with skip connections

Generates realistic translated images

# Discriminator

Uses PatchGAN architecture

Classifies small image patches as real or fake

Helps improve texture quality

# Training

The model is trained using two loss functions:

Adversarial Loss – encourages realistic image generation

L1 Loss – ensures generated images are close to the ground truth

# Technologies Used

Python

PyTorch

Google Colab

Matplotlib

Results

The model generates translated images from input images after training.

# Project Structure
PRODIGY_GA_04
│
├── pix2pix_model.ipynb
├── dataset
├── results
└── README.md

# Applications

Image-to-Image translation models can be used for:

Sketch to Image generation

Map to Satellite conversion

Semantic segmentation to photo generation

Image colorization

# Internship Task

This project was completed as part of the Prodigy InfoTech Generative AI Internship – Task 04.
