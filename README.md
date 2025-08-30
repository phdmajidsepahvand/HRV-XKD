# HRV-XKD

The official repository of HRV-XKD: Early Hypertension Detection via Temporal Drift Analysis in ECG-Derived HRV: A Cross-Window Attention-Based Knowledge Distillation Framework.

# 

### Overview

This project proposes an innovative approach to Early Hypertension Detection by analyzing the Temporal Drift in ECG-derived HRV signals. The model leverages a Cross-Window Attention-Based Knowledge Distillation Framework for accurate prediction of hypertension onset.

# 

### Data



The data used in this project is obtained from the MIMIC-III Waveform Database. This database contains over 67,000 records of physiological signals, such as ECG, ABP, and PPG, collected from ICU patients.



\- Data Source: \[MIMIC-III Waveform Database v1.0 on PhysioNet](https://physionet.org/content/mimic3wdb/1.0/)

\- License: Open Database License v1.0



For more information and to access the data, visit: \[MIMIC-III Waveform Database](https://physionet.org/content/mimic3wdb/1.0/)



Please follow the instructions on the PhysioNet website to download the data.



### Features

\- Data Preprocessing: Data loading and preprocessing from the MIMIC-III database.

\- Modeling: Implementation of a Cross-Window Attention Model for classification.

\- Knowledge Distillation: Using a teacher-student approach for enhanced performance.

\- Evaluation: Metrics such as Accuracy and F1-Score to evaluate model performance.

# 

### Requirements

The following libraries are required:

\- Python >= 3.7

\- torch

\- scikit-learn

\- pandas

\- numpy

\- tqdm

\- pyyaml

\- wfdb

# 

##### You can install them using:

##### ```bash

##### pip install -r requirements.txt

