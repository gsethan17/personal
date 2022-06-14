 # Create virtual environment
 `conda create -n {virtual environment name} python=3.8`
 
 # Activate created virtual environment
 `conda activate {virtual environment name}`
 
 # install pytorch
 `pip3 install --pre torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/nightly/cpu`
 
 # install common data science package
 `conda install jupyter pandas numpy matplotlib scikit-learn tqdm`
 
 # varify all the dependencies are available and check pytorch version/GPU access
 from [https://www.mrdbourke.com/pytorch-apple-silicon/](https://www.mrdbourke.com/pytorch-apple-silicon/)
 ```
 import torch
 import numpy as np
 import pandas as pd
 import sklearn
 import matplotlib.pyplot as plt
 
 print(f"PyTorch version: {torch.__version__}")

 # Check PyTorch has access to MPS (Metal Performance Shader, Apple's GPU architecture)
 print(f"Is MPS (Metal Performance Shader) built? {torch.backends.mps.is_built()}")
 print(f"Is MPS available? {torch.backends.mps.is_available()}")

 # Set the device      
 device = "mps" if torch.backends.mps.is_available() else "cpu"
 print(f"Using device: {device}")
 ```
 
