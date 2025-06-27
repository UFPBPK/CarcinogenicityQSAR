# CarcinogenicityQSAR

# Toxicophore-Informed Machine Learning Integrating Tox21 Assay Readouts for Organ System–Specific Carcinogenicity Prediction  
Created by Chi-Yun Chen |  Date: June 16, 2025

***Welcome to the carcinogenicity project!***

## Guidelines
This repository provides all code, curated data, trained models, and results for predicting carcinogenicity across five main organ systems using both traditional machine-learning algorithms and neural networks.  


📂 **Repository Structure**  

***Data***  
- Unique_CANCER.csv: Curated carcinogenicity data with 957 CAS labeled compounds

***Notebooks***  
- Carcinogen_data_preprocessing.ipynb: Data cleaning and filtering, featurization, analyses (e.g., PCA and applicability domain), visualizations
- Model_training_and_evaluation_7models.ipynb: Seven classifiers (AdaBoost, CatBoost, KNN, LR, RF, SVC, XGBoost), train/test split, hyperparameter optimization, performance evaluation
- Model_training_and_evaluation_NN_model.ipynb: Neural networks, train/validation/test split, hyperparameter optimization, performance evaluation
- Carcinogenicity_best_F1.ipynb: Top models (F1-optimized) for each organ system, visualizations including feature permutation, probability distribution, ROC curves
- Carcinogenicity_best_ROC.ipynb: Top models (ROC-AUC-optimized) for each organ system, visualizations including feature permutation, probability distribution, ROC curves


🌟 **Key Features**
- Pythonic: Open-source 
- Robust cancer data: Collated from EPA IRIS, NTP CEBS, and Lhasa Vitic; low-confidence entries filtered out  
- Organ system identification: Cover ten organ systems, enabling targeted carcinogenicity predictions
- Interpretable features: Combine chemoinformatics with Tox21 in vitro bioactivity profiles
- Mutiple algorithms: Evaluates seven classical machine-learning methods alongside neural-network approaches
- Various scenarios:  Supports combinations of SMOTE application, feature-selection strategies, and Tox21 data inclusion
- Comprehensive analyses & visualization: From raw data exploration through detailed model performance assessments, complete with publication-quality figures


📝 **Requirements**  
These notebooks are intended to run on HiPerGator via Slurm/Open OnDemand, which launches a Jupyter Notebook server on a compute node.
> CPU >= 16 cores  
> RAM >= 120 GB

- **Python:** 3.10.12  
- **Libraries:** `pandas`, `numpy`, `scikit-learn`, `rdkit-pypi`, `seaborn`, `keras-tuner`, `tensorflow`, `shap`

> **Note:** If you’re using Python < 3.10, you may encounter syntax errors where f-strings are used. These can be fixed easily by rebuilding the strings using your preferred formatting method.


## Questions and Feedback
I welcome questions and feedback. Please email Dr. Zhoumeng Lin (linzhoumeng@ufl.edu) or me (chen.chiyun@ufl.edu), or share them in GitHub Discussions.

## Citation
If you find this data or code useful for your research, please consider citing it. 
_To be submitted._
