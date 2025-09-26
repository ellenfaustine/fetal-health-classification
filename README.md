# Deep Learning for Fetal Health Classification

This repository contains my CM3015 Machine Learning and Neural Networks final project, where I apply deep learning to classify fetal health status into three categories using Cardiotocography (CTG) data.

## Project Overview
This project explores the application of deep neural networks for multiclass classification of fetal health. Using CTG data, the model classifies fetal health status as **Normal**, **Suspect**, or **Pathological**, demonstrating how machine learning can assist in supporting clinical decision-making during pregnancy.

The notebook follows the workflow from *Deep Learning with Python* (Chollet, 1st edition), restricted to Part I layers (Dense and Dropout). The project was implemented exclusively in a Jupyter Notebook structured as a report, combining narrative explanations, code, and experimental results. This project highlights how deep learning can support early detection of fetal health risks and assist clinicians in decision-making.

## Problem Statement
The aim of this project was to design and evaluate a deep learning model for fetal health classification using CTG data. Following the design constraints of the project, the model:  
- Uses only Sequential Dense and Dropout layers.  
- Is trained and evaluated on a multiclass dataset.  
- Presents the notebook as a complete report, with headings, subheadings, tables, and visualizations.  

## Dataset
- **Fetal Health Classification Dataset** (UCI Machine Learning Repository).  
- 2,126 samples of CTG recordings.  
- 21 features, including fetal heart rate patterns, accelerations, and uterine contraction signals.  
- 3 target classes:  
  - Normal  
  - Suspect  
  - Pathological  
- Challenges: imbalanced class distribution and noisy signals.  

## Methodology
1. **Preprocessing**  
   - Normalization of input features.  
   - Train-validation-test split.  
   - Addressing class imbalance through stratified sampling.  

2. **Model Design**  
   - Sequential model built with Dense and Dropout layers.  
   - Hyperparameter tuning for number of units, dropout rate, batch size, and epochs.  

3. **Evaluation Metrics**  
   - Accuracy  
   - Precision, Recall, F1-score (macro-average)  
   - Confusion matrix  

## Results
- The final model achieved:  
  - Test Accuracy: ~94%  
  - Macro Precision: ~93%  
  - Macro Recall: ~92%  
  - Macro F1-score: ~92%  

**Summary:** The deep learning model successfully classified fetal health status with high accuracy. While results were strong overall, performance was lower for the minority class (Pathological), highlighting the need for further work on handling class imbalance.

## Files in This Repository
- `fetal_health_classification.html` – Exported Jupyter Notebook (main report with code, explanations, and results).  
- `fetal_health_classification.ipynb` – Raw Jupyter Notebook for reproducibility and re-running the code.  
- `README.md` – Project overview and instructions (this file).  

## How to Use
- Open `fetal_health_classification.html` in a browser to view the complete analysis.  
- Open `fetal_health_classification.ipynb` in Jupyter or Colab to re-run and extend the code.  

## View Online
You can also view the rendered notebook directly through GitHub Pages here:  
👉 [Fetal Health Classification Notebook](https://ellenfaustine.github.io/fetal-health-classification/fetal_health_classification.html)
