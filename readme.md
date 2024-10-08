# MuDLBL

MuDLBL: Mutation-based Deep Learning Bug Localization to locate the faulty statements of a DL bug residing in a DL program. 

## Overview of MuDLBL

![overview](figures/overview.png)

### Step 1: Mutant Generation

After configuring the buggy DL program successfully,  run the tool to be able to get different Mutants.

### Step 2: Bug Localization

After DL mutant generation, MuDLBL will run the DL mutants to evaluate DL mutation behavioral differences as the suspiciousness of a statement being faulty.

## How to use?

### Requirements

- numpy~=1.18.5
- tensorflow~=2.3.0
- tensorflow-gpu~=2.3.0->2.4.1
- Keras~=2.4.3
- matplotlib~=3.3.0
- progressbar~=2.5
- scikit-learn~=0.23.1
- termcolor~=1.1.0
- h5py~=2.10.0
- pandas~=1.1.0
- statsmodels~=0.11.1
- opencv-python~=4.3.0.36
- networkx~=2.5.1
- patsy~=0.5.1
- scipy~=1.4.1

### Configure the model

Just put the buggyDL model program in the MuDLBL path: `./prepared_model/model_saved.py`

## Project structure

```
├───datasets
├───logs
├───mutated_models
│   └───model
│       ├───results
│       │   └───stats
│       └───results_test
│           └───stats
├───operators
├───prepared_models
├───test_models
├───trained_models
└───utils
    └───properties

```

