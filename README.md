# HRV-XKD

The official repository of HRV-XKD: A Cross-Window Attention-Based Knowledge Distillation Framework for Early Hypertension Detection via Temporal Drift Analysis in ECG-Derived HRV.

# 

### Overview

This project proposes an innovative approach to Early Hypertension Detection by analyzing the Temporal Drift in ECG-derived HRV signals. The model leverages a Cross-Window Attention-Based Knowledge Distillation Framework for accurate prediction of hypertension onset. Our project integrates three main components: (1) RR interval extraction and HRV segmentation from raw ECG signals, (2) modeling temporal dependencies across HRV windows using a Cross-Window Attention mechanism to capture subtle drift dynamics, and (3) transferring learned knowledge into a lightweight student model via Knowledge Distillation to enable real-time deployment in wearable devices. The project was evaluated on the publicly available MIMIC-IV Waveform Database. Specifically, our student model achieved an AUC of 0.93 and F1-score of 0.89 while reducing model complexity by more than 65% compared to the teacher model.



### Features

* Data Preprocessing: Data loading and preprocessing from the MIMIC-III database.
* Modeling: Implementation of a Cross-Window Attention Model for classification.
* Knowledge Distillation: Using a teacher-student approach for enhanced performance.
* Evaluation: Metrics such as Accuracy and F1-Score to evaluate model performance.

# 

### Data

This project uses multiple publicly available physiological signal datasets:



1\. MIMIC-III Waveform Database

The MIMIC-III Waveform Database contains over 67,000 records of physiological signals, such as ECG, ABP, and PPG, collected from ICU patients.



\- Data Source: \[MIMIC-III Waveform Database v1.0 on PhysioNet](https://physionet.org/content/mimic3wdb/1.0/)

\- License: Open Database License v1.0

\- For more information and to access the data, visit: \[MIMIC-III Waveform Database](https://physionet.org/content/mimic3wdb/1.0/)



---



2\. The PPG-BP Dataset

The PPG-BP Dataset contains recordings from 219 subjects with a total of 657 PPG-ECG records.

Each recording lasts between 2 to 5 minutes and is sampled at 125 Hz.



\- Data Source: \[The PPG-BP Dataset on PhysioNet](https://physionet.org/content/ppg-bp-dataset/)

\- License: Open Database License v1.0

# 

### Requirements

The following libraries are required:

* Python >= 3.7
* torch
* scikit-learn
* pandas
* numpy
* tqdm
* pyyaml
* wfdb

# 

##### You can install them using:

##### ```bash

##### pip install -r requirements.txt



