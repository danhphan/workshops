## PyMCon Web Series 2023

### Topic: An introduction to multi-output Gaussian processes using PyMC

Multi-output Gaussian processes have recently gained strong attention from researchers and have become an active research topic in machine learning’s multi-task learning. The advantage of multi-output Gaussian processes is their capacity to simultaneously learn and infer many outputs which have a similar source of uncertainty from inputs.

This talk presents to audiences how to build multi-output Gaussian processes in PyMC. It first introduces the concept of Gaussian processes (GPs) and multi-output GPs and how they can address real problems in several domains. It then shows how to implement multi-output GPs models such as the intrinsic coregionalization model (ICM) and the linear model of coregionalization (LCM) in Python using PyMC with real-world datasets.

### Workshop content


| Notebooks/Slides | Content | Link |
| --- | --- | --- |
| [1. Intro to PyMC GP](./01_Intro_PyMC_GP.ipynb) | This notebook introduces the basic concept of Gaussian Process (GP) <ul><li>Bayesian linear regression</li><li>Gaussian Process Regression</li><li>GP Mean and Covariance Functions</li></ul> | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/danhphan/workshops/blob/main/2023-PyMCon/01_Intro_PyMC_GP.ipynb) |
| [2. Intro to multi-output GPs](./02_Intro_Multiouput_GPs.pdf) | This slides introduce Multi-output Gaussian Processes (MoGPs) <ul><li>Why we need MoGPs?</li><li>Intrinsic Coregionalization Model (ICM)</li><li>Linear Coregionalization Model (LCM)</li></ul> | [![Open In Pdf](https://img.shields.io/badge/PDF-View%20pdf-brightgreen)](./02_Intro_Multiouput_GPs.pdf) |
| [3. PyMC MoGP example](./02_PyMC_MOGP_Example.ipynb) | This notebook demonstrates how to implement a Multi-output Gaussian Process (MoGP) in PyMC | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/danhphan/workshops/blob/main/2023-PyMCon/02_PyMC_MOGP_Example.ipynb) |

### Run on Google Colab
Please create a new cell at the beginning of the notebooks and run these following commands to install the latest PyMC version and related packages

```
!pip install pymc==5.0.2 # the latest pymc version
!pip install graphviz
!pip install matplotlib==3.6.3
!pip install watermark
```


### Run on a local environment


**Set up the environment**

```
git clone git@github.com:danhphan/workshops.git
cd ./workshops/2023-PyMCon
conda create --name pymcon -c conda-forge python=3.9
conda activate pymcon
conda install -c conda-forge mamba
mamba install -c conda-forge "pymc>=5.0.0"
pip install -r requirements.txt
```

