# Higgs Boson Event Detection using Deep Learning

##### Kaggle Notebook: https://www.kaggle.com/code/shirshmall/search-for-higgs-boson-decay-modes

### Higgs Boson Event Detection

**Introduction:**
The Higgs Boson Event Detection project focuses on analyzing particle collisions occurring at the Large Hadron Collider (LHC). Protons collide within the LHC, creating high-energy events that produce various particles. These particles quickly decay into lighter particles, and the properties of the original particles are inferred based on these decays. Machine learning algorithms are crucial for analyzing experimental data from these collisions, aiding in detecting significant events and understanding the nature of matter.

**Project Objective:**
The project involves classifying events as either signal or background noise in the decay process of Higgs particle acceleration. The provided dataset includes training and test sets containing features related to the events. The goal is to build a model that accurately identifies whether a given event is a signal or background noise.

**Dataset Description:**
- `training.csv`: Training set with 250000 events, including ID, 30 feature columns, a weight column, and a label column.
- `test.csv`: Test set with 550000 events, including ID and 30 feature columns.
- `random_submission`: Sample submission file format for the competition.
- `HiggsBosonCompetition_AMSMetric`: Python script to calculate the competition evaluation metric.

**Feature Semantics:**
- Variables are floating point, except `PRI_jet_num`, which is an integer.
- Variables with the prefix `PRI` (PRImitives) are raw quantities from bunch collisions as detected.
- Variables with the prefix `DER` (DERived) are computed from primitive features by ATLAS physicists.
- In some cases, variables have values of -999.0, signifying cases where the variables are meaningless or uncomputable.

**Model Development:**
- Initially, columns with missing values were identified and dropped due to high missing value counts.
- Utilized the PyTorch framework to set up a model for binary classification.
- The model achieved an impressive Accuracy Score and F1 Score of 0.98 on both the training and testing datasets.
- The PyTorch framework facilitated efficient model training and evaluation, contributing to the high performance achieved.

**Conclusion:**
The Higgs Boson Event Detection project demonstrates the application of machine learning in high-energy physics. By accurately classifying events as signal or background noise, this project aids in understanding particle collisions and the behavior of particles at the fundamental level. The utilization of PyTorch and careful data preprocessing contributes to the project's success in achieving high accuracy and performance scores.

