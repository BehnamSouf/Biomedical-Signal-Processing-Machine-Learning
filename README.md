# 🧠 Biomedical Signal Processing & Machine Learning

## 📄 Project Overview
This repository contains implementations of machine learning algorithms applied to biomedical datasets. The project is divided into two main modules:
1.  **Classic ML Classifiers:** Implementing algorithms from scratch to classify Breast Cancer data.
2.  **EEG Signal Analysis:** Advanced feature extraction and classification of In-Ear EEG signals using Deep Learning techniques.

## 🛠️ Tech Stack
- **Languages:** Python (NumPy, Pandas, Scikit-learn, SciPy)
- **Signal Processing:** PyWavelets (Wavelet Transform), FFT, Bandpass Filters
- ** Techniques:** Mixup Data Augmentation, Parzen Window, Gaussian Naive Bayes

## 📂 Modules

### 1. ML Classifiers (Breast Cancer) 🎗️
- Implemented **KNN**, **Nearest Mean**, **Gaussian Naive Bayes**, and **Parzen Window** classifiers from scratch.
- Evaluated performance using Accuracy and F1-Score on the sklearn Breast Cancer dataset.
- Analyzed the effect of training data size on model performance.

### 2. EEG Signal Classification 📉
- **Preprocessing:** Applied Bandpass filters (Delta, Theta, Alpha, Beta) to isolate brainwave frequencies.
- **Feature Extraction:** Extracted statistical features (Mean, Std) and **Wavelet Transform (db4)** coefficients.
- **Handling Imbalance:** Implemented **Mixup Oversampling** to balance the dataset.
- **Classification:** Used SVM/Random Forest pipelines with GridSearch for optimal performance.

## 📊 Results
- **EEG Analysis:** Successfully differentiated between mental states using extracted frequency-domain features.
- **ML Models:** Achieved high accuracy comparisons between parametric (Naive Bayes) and non-parametric (KNN) models.

## 🚀 How to Run
1. Install dependencies:
   ```bash
   pip install numpy pandas scikit-learn scipy pywavelets matplotlib
Robust Classical Machine Learning for Biomedical Diagnosis: A Dual Evaluation on Breast Cancer Prediction and Ear-EEG Emotion Recognition

Behnam Soufi Sharvenien

Abstract
Reliable analysis of biomedical data is essential for diagnostic support and human-state monitoring. This study investigates the performance and robustness of classical machine-learning models across two different biomedical tasks: breast-cancer classification using the Wisconsin Diagnostic dataset and emotion recognition using in-ear EEG signals. For the cancer dataset, four traditional classifiers were evaluated under clean conditions, reduced training sets, and multiple noise intensities. The results show that KNN provides the highest stability, while Naive Bayes is strongly affected by severe noise, indicating fundamental sensitivity to distributional perturbations.
For the EEG task, handcrafted temporal–spectral features were extracted from two channels and combined with Fisher Score and Mutual Information for feature selection. A grid-search procedure optimized each classifier, and an enhanced feature set was developed by incorporating db4 wavelet-based descriptors. This augmentation substantially increased performance, with SVM showing the largest improvement, raising its mean F1-score from about 0.67 to 0.79.
Overall, the findings demonstrate that classical machine-learning algorithms remain effective for structured clinical data and low-channel EEG recordings. The wavelet-enhanced feature extraction significantly strengthens EEG emotion classification, highlighting its suitability for practical, lightweight biomedical systems.
Keywords
Classical Machine Learning; Biomedical Signal Processing; Breast Cancer Classification; Ear-EEG Emotion Recognition; Supervised Classification.
result 
<img width="976" height="836" alt="image" src="https://github.com/user-attachments/assets/cb3682bb-d1e4-46a8-ab50-06e5ab2e65ff" />
<img width="975" height="395" alt="image" src="https://github.com/user-attachments/assets/f19bd099-64fd-4ab1-afc5-82a1ff1f2a4f" />
