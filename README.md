Generating Medulloblastoma Images Using W-GAN

Overview
This repository contains the implementation and results of the research project titled "Generating Medulloblastoma Images Using W-GAN." The primary objective is to tackle the scarcity of high-quality medulloblastoma histopathology data by generating synthetic images at 10x and 100x magnifications using a Wasserstein GAN with Gradient Penalty (WGAN-GP).

These synthetic images enhance dataset diversity and improve the training of AI models used in medical diagnostics.

Features
Synthetic Image Generation

10x Magnification: Highlights tissue architecture and cellular patterns.
100x Magnification: Focuses on individual cell morphology and nuclear-cytoplasmic ratios.
Evaluation Metrics

Inception Score (IS): Evaluates image quality and diversity.
Fréchet Inception Distance (FID): Measures similarity to real-world data.
Repository Structure
plaintext
Copy code
.
├── code/
│   ├── 10x_magnification.py       # Code for generating 10x magnification images
│   ├── 100x_magnification.py      # Code for generating 100x magnification images
│   ├── utils.py                   # Utility functions (e.g., preprocessing, evaluation)
├── data/
│   ├── 10x/                       # Folder containing 10x magnification data samples
│   ├── 100x/                      # Folder containing 100x magnification data samples
│   └── README.md                  # Data description
├── results/
│   ├── generated_10x/             # Generated 10x images
│   ├── generated_100x/            # Generated 100x images
│   └── evaluation_metrics.txt     # Inception Score and FID values
├── figures/
│   ├── architecture_diagram.png   # W-GAN model architecture
│   ├── results_comparison.png     # GAN comparison graphs
│   └── training_curves.png        # Generator and Discriminator loss curves
├── LICENSE
└── README.md                      # This file
Requirements
Python >= 3.8
Deep Learning Framework: TensorFlow or PyTorch
Dependencies: NumPy, Matplotlib, Scikit-learn
Install the required packages using the following command:

bash
Copy code
pip install -r requirements.txt
Usage
Clone the Repository

bash
Copy code
git clone https://github.com/your-username/medulloblastoma-wgan.git
cd medulloblastoma-wgan
Run the Code for 10x Magnification

bash
Copy code
python code/10x_magnification.py
Run the Code for 100x Magnification

bash
Copy code
python code/100x_magnification.py
Check Generated Images
The generated images will be saved in the results/ directory.

Results
Generated Images
10x Magnification: Preserves tissue architecture with minimal artifacts.
100x Magnification: Highlights cell morphology and nuclear-cytoplasmic ratios.
Evaluation Metrics
Magnification	Inception Score	FID
10x	1.003 ± 0.001	4.464
100x	1.005 ± 0.001	2.383
Contributions
Parth Jariwala: Concept, Implementation, Documentation
VSS Nishwan: Code Development, Testing
Thomas Abraham: Guidance, Review
License
This project is licensed under the MIT License. See the LICENSE file for details.

Contact
Parth Jariwala: parth10.jariwala@gmail.com
VSS Nishwan: vssnishwan@gmail.com
Thomas Abraham: thomasabraham.jv@vit.ac.in
