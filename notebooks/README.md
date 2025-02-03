# Notebooks Guide

## Overview
This document describes the notebook scripts and how they interact with the datasets

## Notebooks Organization
Each notebook works individually with each dataset.

```
.
├── dataset_cleaning.ipynb
├── dataset_separation.ipynb
├── dataset_separation_augmented.ipynb
├── model_training.ipynb
└── README.md
```

- **dataset_cleaning.ipynb**: Reads the `.xlsx` file from the `raw_database/` folder and cleans it with the correct file names and exclude non important informaiton, and save the clean `.xlsx` file in the 
- **dataset_separation.ipynb**: Reads the `raw_database/` folder and the clean `.xlsx` file, pass the filters on the audio files and separate them in 10 seconds segments and put they in the `denoized_database/` with a `.xlsx` file with the segments information.
- **dataset_separation_augmented.ipynb**: Reads the `raw_database/` folder and the clean `.xlsx` file, pass the filters on the audio files and separate them in 10 seconds segments with a data augmented technique and put they in the `denoized_augmented_database/` with a `.xlsx` file.
- **model_training.ipynb**: Here you can select which dataset_separation you want to train the model with, and also the feature extraction parameters, the results of the model will be shown at the end of the notebook.