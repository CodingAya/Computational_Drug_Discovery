# Computational_Drug_Discovery

Goal:


RDKit is a cheminformatics toolkit with bindings for Python. It's packed with functionality, deployed within multiple open source projects, and is widely-used in machine learning applications. 

After installing Anaconda, as per the RDKit Installation page, we can create a new Anaconda environment to be used with RDKit as follows:

$ conda create -c rdkit -n my-rdkit-env rdkit

Jupyter is not accessible by default from new Anaconda environments. It can be made accessible with the nb_conda_kernels extension, which can be installed into an existing environment:

$ conda install -n my-rdkit-env nb_conda_kernels

Jupyter is not accessible by default from new Anaconda environments. It can be made accessible with the nb_conda_kernels extension, which can be installed into an existing environment:

$ conda install -n my-rdkit-env nb_conda_kernels
Now activate the environment and run Jupyter Notebook with:

$ conda activate my-rdkit-env
(my-rdkit-env) $ jupyter notebook

For more details about the RDKit toolkit you can refer to this [website](https://depth-first.com/articles/2020/08/17/getting-started-rdkit-and-jupyter/)
