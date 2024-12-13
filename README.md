# Generating Medulloblastoma Images Using W-GAN

## Overview

This repository contains the implementation and results of the research project titled **"Generating Medulloblastoma Images Using W-GAN."**  
The primary objective is to tackle the scarcity of high-quality medulloblastoma histopathology data by generating synthetic images at **10x** and **100x magnifications** using a Wasserstein GAN with Gradient Penalty (**WGAN-GP**).  

These synthetic images enhance dataset diversity and improve the training of AI models used in medical diagnostics.

---

## Features

- **Synthetic Image Generation**  
  - **10x Magnification**: Highlights tissue architecture and cellular patterns.  
  - **100x Magnification**: Focuses on individual cell morphology and nuclear-cytoplasmic ratios.  

- **Evaluation Metrics**  
  - **Inception Score (IS)**: Evaluates image quality and diversity.  
  - **Fréchet Inception Distance (FID)**: Measures similarity to real-world data.  

---

## Repository Structure

├── code/
│   ├── 10x_magnification.py       # Code for generating 10x magnification images
│   ├── 100x_magnification.py      # Code for generating 100x magnification images
│   ├── utils.py                   # Utility functions (e.g., preprocessing, evaluation)

---

├── data/
│   ├── 10x/                       # Folder containing 10x magnification data samples
│   ├── 100x/                      # Folder containing 100x magnification data samples
│   └── README.md                  # Data description

---

├── results/
│   ├── generated_10x/             # Generated 10x images
│   ├── generated_100x/            # Generated 100x images
│   └── evaluation_metrics.txt     # Inception Score and FID values

---

├── figures/
│   ├── architecture_diagram.png   # W-GAN model architecture
│   ├── results_comparison.png     # GAN comparison graphs
│   └── training_curves.png        # Generator and Discriminator loss curves

