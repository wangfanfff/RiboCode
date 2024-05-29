#  Deep Generative Optimization of mRNA Codon Sequences for Enhanced Protein Production and Therapeutic Efficacy

This is the official PyTorch implementation of **RidoDecode** .

# Get Started

## Environment
- Python=3.8  
- torch=1.12.0
- viennarna=2.4.18 
- numpy=1.24.3  
- pandas=1.4.4  
- matplotlib=3.6.2 
- seaborn=0.12.2

The required dependency packages will be automatically downloaded the first time you run the program.

## Installation and Usage

- **translation model**

To install the translation model program, execute the following command:

```
pip install TranslationModel-0.1.0-py3-none-any.whl
```

After installation, use the following command to perform local testing:

```
pred-translation --cds ATGGACGGGTAG --env HEK293T
```

The maximum length of the coding sequence (CDS) should not exceed 4500. The current environment supports HEK293T, A549, and BJ. Support for additional environments will be added gradually.

Following these instructions, you can obtain the ribosome profiling (RPF) expression value for a specific CDS sequence in a particular environment.

- **RidoDecode**

To install the RidoDecode program, execute the following command:

```
pip install RiboDecode-0.1.0-py3-none-any.whl
```

After installation, use the following command to perform local testing:

```
ribo-decode --cds gluc --env HEK293T --mfe_weight 0 --optim_epoch 10
```

The cds options include gluc, NGF, H1N1, with additional sequences to be made available later. Similarly, the 'env' parameter can be set to HEK293T, A549, BJ, with support for additional environments planned for future releases. 

**Stay tuned !!!**

The parameter 'mfe_weight' can be assigned a constant value ranging from 0 to 1, while the optim_epoch can be specified as an integer as required.

## Citation
