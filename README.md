# EEG-BCI-Lab

## Background
Individuals with amyotrophic lateral sclerosis (ALS) and tetraplegia relies on brain function, head, and eye movements to control human–machine interface (HMI). Many approaches utilize electroencephalography (EEG) combined with eye movements. 

## Objective
Evaluate the performance of Linear Discriminant Analysis (LDA), Quadratic Discriminant Analysis (QDA) and Naïve Bayes classifier in a BCI system derived from eyes closed (EC) and eyes open (EO) activities.

## Method
<img width="773" alt="image" src="https://github.com/learnindya/EEG-BCI-Lab/assets/105585813/6b4c41f1-38bb-4922-9d45-ab9dfd0e25a2">

Electrode placement:
<img width="310" alt="image" src="https://github.com/learnindya/EEG-BCI-Lab/assets/105585813/6aeb4cf3-1373-4223-b32e-b81d0ac68b0e">

## Preprocessing
* 4 band-pass filters to extract 4 EEG signals:
  - Delta: frequency <= 3 Hz
  - Theta: 3.5 <= frequency <= 7.5 Hz
  - Alpha: 7.5 <= frequency <= 13 Hz
  - Beta: 14 <= frequency <= 30 Hz

* Feature selection:
  - Based on discriminant power, 8-10 Hz and 10-12 Hz frequency bins were used as features

## Result
LDA:
- AUC: 78.4%
- Misclassification rate: 25% 
- K-fold error: 30.56%
