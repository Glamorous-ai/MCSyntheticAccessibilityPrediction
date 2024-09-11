# Molecular Feature Extraction and Model Ensembling

## Overview

This repository provides two Jupyter Notebooks focused on synthetic accessibility prediction through ensembling. The goal of the project is to streamline the process of converting molecular structures into machine learning-friendly features and to enhance model performance using multi-fold ensembling techniques.

### Notebooks

1. **1-feature-extraction.ipynb**:
   - Converts SMILES strings into Morgan Fingerprints. Morgan Fingerprints are a type of circular fingerprint used in cheminformatics to represent molecules as bit vectors, facilitating their use in machine learning models.
   
2. **2-fold-ensembling.ipynb**:
   - Implements a fold ensembling technique, combining the predictions of multiple models trained on different data folds to improve predictive accuracy. This method helps mitigate overfitting and enhances model robustness.

### Usage

1. Feature Extraction from SMILES Strings

To extract features from molecular data:

	1.	Input your dataset containing SMILES strings (a textual representation of chemical structures).
	2.	Follow the steps in the notebook to convert SMILES strings into Morgan Fingerprints.
	3.	The resulting features will be used for the second notebook.

2. Fold Ensembling for Model Improvement

To perform fold ensembling:

	1.	Once you have generated features using the previous notebook, proceed to 2-fold-ensembling.ipynb.
	2.	This notebook will guide you through the process of training multiple models on different folds of the dataset.
	3.	The predictions from each fold are ensembled to produce a robust prediction that mitigates class imbalance.
	4.	You can adjust the number of folds, models used, and other parameters as needed.


### Data
	•	A public set with 870k SMILES strings is stored in "/data/df_87w_five_classes.csv".
   	•	Training and testing split is store in "/data/split/df_87w_five_classes.json".
