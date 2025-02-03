# Data Preparation and Organization

## Overview
This document describes the data preparation process and how the data is structured in this repository.

## Data Sources
The dataset used in the experiment can be obtained in the website [Physionet](https://physionet.org/content/sufhsdb/1.0.1/). PhysioNet is a repository of freely-available medical research data, managed by the MIT Laboratory for Computational Physiology.

## Data Organization
Each folder should contain a set of `.wav` files. The Physionet dataset have `.wav` files, `.hea` files and a `.xlsx` file with information about the files in it. 

```
.
├── raw_database/ # Insert Physionet dataset here
├── denoized_database/
├── denoized_augmented_database/
└── README.md
```

- **raw_database**: Insert the Physionet dataset files here
- **denoized_database**: After you run `dataset_separation.ipynb` it should contain `.wav` files with 10 seconds filtered audio. 
- **denoized_augmented_database**: After you run `dataset_separation_augmented.ipynb` it should contain `.wav` files with 10 seconds filtered audio plus more segments with a data augmentation technique described in the `Paper.pdf`.