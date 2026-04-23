# Distracted Driver Detection using YOLOv8

Final year BSc AI project — Anglia Ruskin University

## Overview
Real-time distracted driver detection using YOLOv8n classification 
on the State Farm dataset. Key finding: subject-independent dataset 
splitting reduces accuracy from 99.71% to 92.30%, revealing data 
leakage in random splits.

## Requirements
pip install -r requirements.txt

## Dataset
State Farm Distracted Driver Detection dataset  available on Kaggle:
https://www.kaggle.com/c/state-farm-distracted-driver-detection

## Notebooks
01 - Data preprocessing and subject split
02 - Model training
03 - Model evaluation
04 - Model comparison
05 - YOLOv8s rerun
06 - EigenCAM explainability
07 - Real-time alert system

## Results
YOLOv8n: 92.30% accuracy, 0.9220 F1, 2.8MB, 4.76ms inference

## How to Run

### Requirements
Python 3.12.9 is required. Install all dependencies with:
pip install -r requirements.txt

### Dataset
A Kaggle account is required to download the dataset. 
You will need to accept the competition rules before 
the download becomes available.
Download the State Farm Distracted Driver Detection dataset from:
https://www.kaggle.com/c/state-farm-distracted-driver-detection

Place the downloaded dataset in the following structure:
data/
  statefarm_subject_split/
    train/
      c0/ c1/ ... c9/
    val/
      c0/ c1/ ... c9/

Notebook 01 builds this folder structure automatically from the 
raw Kaggle download.

### Running the notebooks
Run the notebooks in order from 01 to 07. Each notebook depends 
on outputs from the previous one.

All paths are relative — no changes needed before running.
