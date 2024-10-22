# Multispectral Remote Sensing Projects

**Institution**: Faculdade de Ciências da Universidade de Lisboa  
**Course**: Multispectral Remote Sensing  
**Project Date**: 2022  
**Project Language**: Portuguese/English  

## Table of Contents

- [Overview](#overview)
- [Projects](#projects)
  - [1. Machine Learning Land Use Classification (Project1)](#1-machine-learning-land-use-classification-project1)
  - [2. Article Analysis on Land Use Classification (Project2)](#2-article-analysis-on-land-use-classification-project2)
- [Folder Structure](#folder-structure)
- [Conclusion](#conclusion)

## Overview

This repository contains two projects developed for the Multispectral Remote Sensing class. The main project involves using machine learning algorithms to classify land use in a region southeast of Lisbon, based on **Sentinel-2** multispectral data. A smaller project analyzes an article about the use of deep convolutional neural networks for land use classification with high spatial resolution multispectral imagery.

## Projects

### 1. Machine Learning Land Use Classification (Project1)

- **Objective**: The goal of this project was to classify land use in a section of Portugal southeast of Lisbon using **Sentinel-2** satellite imagery and compare the performance of different machine learning algorithms.
  
- **Algorithms Used**:
  - **Random Forest (RF)**: Uses 200 decision trees for classification based on majority voting.
  - **Decision Trees**: Non-parametric algorithm based on hierarchical if/else questions with a tree having 10 branches.
  - **Naive Bayes Classifier**: A probabilistic model based on Bayes' Theorem assuming strong independence between features.

- **Image Data**:
  - Includes spectral **bands**, **indices**, **Principal Component Analysis (PCA)** components, and **textures** to improve classification accuracy.
  - Band combinations tested: 
    1. Bands only
    2. Bands + Indices
    3. Bands + Indices + Textures

- **Results**:
  - The best overall accuracy (83%) was obtained using **Naive Bayes** with bands only.
  - **Random Forest** performed well, but excluding underrepresented classes like class 323 (Other Conifers) improved results slightly.
  - **Decision Trees** had a lower accuracy compared to Naive Bayes and Random Forest.
  
- **Limitations**:
  - The study's small area size limited the ability to generalize the models for all land use classes.
  - High computational effort constrained the choice of algorithms, preventing the use of **SVM** and **KNN**.

### 2. Article Analysis on Land Use Classification (Project2)

- **Objective**: Analyze an academic article focused on the application of machine learning or neural networks for land use classification using multispectral images.
  
- **Article**: "Urban land-use mapping using a deep convolutional neural network with high spatial resolution multispectral remote sensing imagery" by Bo Huang, Bei Zhao, and Yimeng Song.  
- **Methodology**: The project involved critically analyzing the methodology, results, and challenges presented in the paper.
  
- **Deliverables**:
  - **Analysis Report**: A detailed written review of the article.
  - **Presentation**: Summarizes key findings and insights from the article analysis.

## Folder Structure

- `/Article_Analysis/`: Contains the files related to the analysis of an academic article.
  - `Analysis.docx`: Report on the article analysis.
  - `Analysis_presentation.pptx`: Presentation of the article analysis.
  - `Urban land-use mapping... .pdf`: The article analyzed.
  
- `/Machine_Learning_LU_Classification/`: Contains files for the land use classification project.
  - `classification_report.pdf`: Final report with results and findings.
  - `confusion_matrices.xlsx`: Confusion matrices for each classification method.
  - `presentation_classification.pptx`: Presentation of the project findings.

## Conclusion

These projects highlight the application of machine learning algorithms in land use classification using multispectral remote sensing data. The results illustrate the effectiveness of different classifiers and the challenges in working with unbalanced classes and computational limitations. The analysis of the article offers insights into the use of neural networks for urban land-use mapping.
