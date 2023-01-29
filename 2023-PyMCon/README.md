## PyMCon Web Series 2023

### Topic: An introduction to multi-output Gaussian processes using PyMC

Multi-output Gaussian processes have recently gained strong attention from researchers and have become an active research topic in machine learning’s multi-task learning. The advantage of multi-output Gaussian processes is their capacity to simultaneously learn and infer many outputs which have a similar source of uncertainty from inputs.

This talk presents to audiences how to build multi-output Gaussian processes in PyMC. It first introduces the concept of Gaussian processes (GPs) and multi-output GPs and how they can address real problems in several domains. It then shows how to implement multi-output GPs models such as the intrinsic coregionalization model (ICM) and the linear model of coregionalization (LCM) in Python using PyMC with real-world datasets.

### Run on Google Colab


| Notebook | Content | Colab link |
| --- | --- | --- |
| [1. Intro to PyMC GP](./01_Intro_PyMC_GP.ipynb) | This notebook introduces the basic concept of Gaussian Process (GP) 
- Bayesian linear regression
- Gaussian Process Regression
- GP Mean and Covariance Functions
| [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/danhphan/workshops/blob/main/2023-PyMCon/01_Intro_PyMC_GP.ipynb) |
| [2. Intro to PyMC MoGP](./02_Intro_PyMC_MOGP.ipynb) | This notebook demonstrates Multi-output Gaussian Process (MoGP) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/danhphan/workshops/blob/main/2023-PyMCon/02_Intro_PyMC_MOGP.ipynb) |



### Run on a local environment


**Set up the environment**

```
git clone git@github.com:danhphan/workshops.git
cd ./workshops/2023-PyMCon
conda create --name pymcon -c conda-forge python=3.9
conda activate pymcon
conda install -c conda-forge mamba
mamba install -c conda-forge "pymc>=5.0.0" nutpie
pip install -r requirements.txt

```

