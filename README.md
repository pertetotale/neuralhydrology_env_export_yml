# NeuralHydrology package management:  exported yml to build an up to date conda environment. 

The neuralhydrology project provides some yaml files to create a virtual (conda) environment.

However, these yaml files still have some pip dependencies which, after pip pkg installs later on, can break conda environments. 
Since the latest NH yaml versions are from 2022, it was time for an updated version. 

The starting point was the yaml file *neuralhydrology_environment_cuda11_8.yml*. 

This file is the exported yaml file with minimal pip dependencies: only neuralhydrology and torchvision. 

The new env. was tested, and it runs and trains a **custom** model on a "GenericDataset" with a python 3.11 kernel. 
