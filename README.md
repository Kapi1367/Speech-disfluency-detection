# 🎙️ Stuttering Event Detection using SEP-28k Dataset

A deep learning pipeline for **automatic detection of stuttering events** in spontaneous speech using the **Apple SEP-28k (Stuttering Events in Podcasts)** dataset.  
This project builds a full workflow from **data acquisition → preprocessing → feature extraction → CNN-based classification**, identifying stuttered vs non-stuttered speech clips.

---

## 🧠 Project Overview

This project demonstrates an end-to-end audio analysis system designed to detect **stuttering events** in podcast audio.  
It leverages **MFCC (Mel-Frequency Cepstral Coefficients)** and **temporal dynamics** to train a **1D Convolutional Neural Network (CNN)** capable of classifying stuttered vs fluent speech.

### 🔍 Pipeline Summary

1. **Dataset Setup**
   - Downloads and organizes podcast audio episodes from SEP-28k.
   - Extracts labeled speech clips with stuttering annotations.

2. **Audio Preprocessing**
   - Converts and normalizes `.mp3` files into `.wav` clips.
   - Filters out poor-quality or irrelevant clips.

3. **Feature Extraction**
   - Computes MFCCs, deltas, delta-deltas, and temporal fluctuation metrics.
   - Generates robust, flattened feature vectors per clip.

4. **Modeling**
   - Builds a CNN classifier using TensorFlow/Keras.
   - Balances data with class weighting and early stopping.
   - Evaluates performance using Accuracy, AUC, Precision, and Recall.

5. **Visualization**
   - Waveform and spectrogram plotting for clips.
   - Dataset distribution analysis (stutter type, source, etc.).
   - Confusion matrix and training curves for evaluation.

---

## 🧩 Key Features

- 🎧 End-to-end speech processing for stutter detection  
- 🧮 MFCC-based acoustic feature extraction  
- ⚙️ Robust audio preprocessing and clip generation  
- 🧠 CNN model with attention to stutter vs non-stutter classification  
- 📊 Rich data visualization and metrics tracking 
