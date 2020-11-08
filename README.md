# Respiratory Diseases Predictor

## Overview

The aim of this project is to build a model that predicts and diagnoses chronic inflammatory respiratory diseases. The model classifies the patient into one of the four groups: Chronic Obstructive Pulmonary Disease (COPD), asthma, infected, and Healthy Controls (HC). The used dataset to build the model is Exasens dataset and it is downloaded from [UCI ML](https://archive.ics.uci.edu/ml/datasets/Exasens#).
The Exasens dataset includes demographic information on four groups of saliva samples (COPD-Asthma-Infected-HC) collected in the frame of a joint research project at the Research Center Borstel, BioMaterialBank Nord (Borstel, Germany). A permittivity biosensor, developed at IHP Microelectronics (Frankfurt Oder, Germany), was used for the dielectric characterization of the saliva samples for classification purposes [[1]](https://www.mdpi.com/2227-9032/7/1/11).

Definition of four sample groups included within the Exasens dataset:
1. Outpatients and hospitalized patients with COPD without acute respiratory infection (COPD).
2. Outpatients and hospitalized patients with asthma without acute respiratory infections (Asthma).
3. Patients with respiratory infections, but without COPD or asthma (Infected).
4. Healthy controls without COPD, asthma, or any respiratory infection (HC).

## Data

The dataset contains 7 attributes:

1. Diagnosis (COPD-HC-Asthma-Infected)
2. ID
3. Age
4. Gender (1=male, 0=female)
5. Smoking Status (1=Non-smoker, 2=Ex-smoker, 3=Active-smoker)
6. Saliva Permittivity - Imaginary part (Min(Î”)=Absolute minimum value, Avg.(Î”)=Average)
7. Saliva Permittivity -  Real part (Min(Î”)=Absolute minimum value, Avg.(Î”)=Average)

## Tools

The model is built using two ways: *Python* and *RapidMiner*. 

## File Descriptions 

- `Exasens_dataset.csv`: the dataset file.
- `Respiratory_Diseases.ipynb`: notebook contains the Python code of data preparation and Gradient Boosting classifier. 
- `Respiratory Diseases Repository`: RapidMiner folder respiratory.
	- `Data`: data folder.
		- `Exasens_dataset.rmhdf5table`: data file.
	- `Process`: process folder.
		- `Grid search.rmp`: the file of a process that uses grid search to obtain optimal values of model hyperparameters.
		- `GB model.rmp`: the file of one model process (Gradient Boost Classifier). 
	 


