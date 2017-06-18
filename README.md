Improved Training of Wasserstein GANs
=====================================

Code for reproducing experiments in ["Improved Training of Wasserstein GANs"](https://arxiv.org/abs/1704.00028).


## Prerequisites

- Python, NumPy, TensorFlow, SciPy, Matplotlib
- A recent NVIDIA GPU

## Models

Configuration for all models is specified in a list of constants at the top of
the file. Two models should work "out of the box":

- `python gan_toy.py`: Toy datasets (8 Gaussians, 25 Gaussians, Swiss Roll). 
- `python gan_mnist.py`: MNIST

For the other models, edit the file to specify the path to the dataset in
`DATA_DIR` before running. Each model's dataset is publicly available; the
download URL is in the file.

- `python gan_64x64.py`: 64x64 architectures (this code trains on ImageNet instead of LSUN bedrooms in the paper)
- `python gan_language.py`: Character-level language model
- `python gan_cifar.py`: CIFAR-10


## Installation Windows

Install anaconda
https://www.continuum.io/downloads#windows


# Install tensorflow with GPU Support
    Install tensorflow
    Requirements to run TensorFlow with GPU support

    If you are installing TensorFlow with GPU support using one of the mechanisms described in this guide, then the following NVIDIA software must be installed on your system:

    CUDA® Toolkit 8.0. For details, see NVIDIA's documentation Ensure that you append the relevant Cuda pathnames to the %PATH% environment variable as described in the NVIDIA documentation.
    The NVIDIA drivers associated with CUDA Toolkit 8.0.
    cuDNN v5.1. For details, see NVIDIA's documentation. Note that cuDNN is typically installed in a different location from the other CUDA DLLs. Ensure that you add the directory where you installed the cuDNN DLL to your %PATH% environment variable.
    GPU card with CUDA Compute Capability 3.0 or higher. See NVIDIA documentation for a list of supported GPU cards.
    
    conda install Pillow
    conda install -c anaconda scipy=0.19.0
    conda install scikit-learn
    conda install matplotlib
