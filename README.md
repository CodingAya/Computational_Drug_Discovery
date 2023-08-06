# Computational Drug Discovery

## Context
Alzheimer’s disease is the most common cause of dementia among the elderly and is characterized by loss of memory and other cognitive functions. In Alzheimer's disease, there is a decrease in the level of `acetylcholine`, a neurotransmitter that plays an important role in the normal function of the brain and body. `Acetylcholinesterase` is an enzyme, a specialized protein, that breaks down `acetylcholine` after it has completed its job of transmitting messages between neurons. This decrease in `acetylcholine` contributes to the cognitive and memory problems associated with Alzheimer's disease.

Treatment of Alzheimer's disease has been dominated by the use of `acetylcholinesterase` (AChE) inhibitors. These drugs compensate for the death of cholinergic neurons and offer symptomatic relief by inhibiting `acetylcholine` (ACh) turnover and restoring synaptic levels of this neurotransmitter.

## Dataset
The dataset used in this project is the ChEMBL dataset. ChEMBL is a manually curated database of bioactive molecules with drug-like properties. It brings together chemical, bioactivity, and genomic data to aid the translation of genomic information into effective new drugs. It is compiled from more than 88,000 documents, 1.6 million assays, and the data spans 15,000 targets and 2,000 cells, and 45,000 indications. [[Data as of August 3, 2023; ChEMBL version 33].](https://www.ebi.ac.uk/chembl/) 

## Goal:

## Part 1:
Download and pre-process biological activity data of the target protein 'Acetylcholinesterase' from the ChEMBL database to perform Computational Drug Discovery.

## Part 2:
Computing Lipinski's molecular descriptors (molecular weight, LogP, number of hydrogen bond donors, and number of hydrogen bond acceptors) and performing exploratory data analysis to discern differences between the active and inactive sets of compounds.

## Part 3:
Computing the molecular descriptors using the PADEL-Descriptor software and preparing the dataset for Model Building.

## Additional info
### RDKit
RDKit is a cheminformatics toolkit with bindings for Python. It's packed with functionality, deployed within multiple open-source projects, and is widely used in machine learning applications. 

After installing Anaconda, as per the RDKit Installation page, we can create a new Anaconda environment to be used with RDKit as follows:

```bash
$ conda create -c rdkit -n my-rdkit-env rdkit
```

Jupyter is not accessible by default from new Anaconda environments. It can be made accessible with the nb_conda_kernels extension, which can be installed into an existing environment:

```bash
$ conda install -n my-rdkit-env nb_conda_kernels
```

Jupyter is not accessible by default from new Anaconda environments. It can be made accessible with the nb_conda_kernels extension, which can be installed into an existing environment:

```bash
$ conda install -n my-rdkit-env nb_conda_kernels
```

Now activate the environment and run Jupyter Notebook with:

```bash
$ conda activate my-rdkit-env
(my-rdkit-env) $ jupyter notebook
```
For more details about the RDKit toolkit you can refer to this [website.](https://depth-first.com/articles/2020/08/17/getting-started-rdkit-and-jupyter/)


### PADEL-Descriptor software
[PaDEL-Descriptor](http://www.yapcwsoft.com/dd/padeldescriptor/) is a software developed in Java for calculating molecular descriptors and fingerprints. The software currently calculates 797 descriptors (663 1D, 2D descriptors, and 134 3D descriptors) and 10 types of fingerprints. These descriptors and fingerprints are calculated mainly using The Chemistry Development Kit. 
- `padel.sh` is the shell script file that contains instructions on how to run PaDEL calculations.
