# HRV-XKD

The official repository of HRV-XKD: A Cross-Window Attention-Based Knowledge Distillation Framework for Early Hypertension Detection via Temporal Drift Analysis in ECG-Derived HRV.

# 

### Overview

Early detection of hypertension is challenging due to the gradual and subtle nature of neurocardiac dysregulation. Traditional Heart Rate Variability (HRV)-based methods often rely on static, single-window analyses and fail to capture temporal dynamics across multiple windows.

In this project, we propose HRV-XKD, a cross-window attention-based knowledge distillation framework designed to model gradual temporal drifts in HRV signals for accurate early hypertension detection. The framework was evaluated using two publicly available datasets: PPG-BP and MIMIC-IV Waveform. Raw biosignals were preprocessed to extract HRV features and segmented into overlapping windows to better capture temporal variations.

The proposed approach employs a high-capacity teacher network to model temporal dependencies using multi-head cross-window attention, while transferring its learned knowledge into a lightweight student model through a hybrid loss function combining cross-entropy, temperature-scaled soft-target alignment, and feature mimicry. The resulting student model is optimized for real-time deployment on wearable devices.

Experimental results demonstrate that HRV-XKD outperforms classical baselines and recent deep learning models, including ExHyptNet. On the MIMIC-IV dataset, the student model achieved an AUC of 0.93 and an F1-score of 0.89, while reducing model complexity by over 65% and improving inference speed by 3.2×. Comparable results on the PPG-BP dataset confirm the robustness and generalizability of the proposed framework.

Overall, HRV-XKD provides an accurate, explainable, and computationally efficient solution for early hypertension screening, bridging the gap between high-performance AI and resource-constrained deployment in real-world healthcare applications.


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



