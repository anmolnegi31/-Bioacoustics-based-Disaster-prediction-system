#  Bioacoustics-Based Disaster Prediction System

This project leverages **bioacoustic data** and **machine learning** to predict natural disasters like storms and floods. By analyzing environmental sound patterns and animal vocalizations using AI models, the system offers an innovative, data-driven early warning approach aligned with **UN SDG 13: Climate Action**.

---

## Problem Statement

Climate-induced disasters are increasing in frequency and intensity, but existing forecasting systems often lack localization and ecological context. Animal behavior, especially vocal shifts in birds, can serve as natural indicators of environmental disturbances.

**Our goal:** Use existing bioacoustic data and machine learning to build a low-cost, scalable disaster prediction model.

---

## Core Idea

Instead of deploying new sensors, we use open-access databases like **[eBird](https://ebird.org/)** and **[Xeno-canto](https://www.xeno-canto.org/)**. The system detects acoustic anomalies through:

- **Spectrogram analysis**
- **MFCC (Mel-Frequency Cepstral Coefficients)**
- **ML classifiers (CNN, Random Forest, SVM)**

---

## 🛠Tools & Technologies

- **Language**: Python 3.10+
- **IDE**: Jupyter Notebook
- **Libraries**:
  - `Librosa` for audio processing
  - `Scikit-learn` for ML models
  - `TensorFlow/Keras` for deep learning (CNN)
  - `OpenCV` and `Matplotlib` for visualization
  - `NumPy`, `Pandas` for data wrangling

---

##  Methodology

1. **Data Collection**: Audio files from eBird & Xeno-canto  
2. **Preprocessing**: Resampling, trimming, noise reduction  
3. **Feature Extraction**: MFCCs, Spectrograms, Chroma  
4. **Model Training**:  
   - CNN on spectrograms  
   - Random Forest & SVM on extracted features  
5. **Evaluation**: Accuracy, Precision, Recall, F1 Score, Confusion Matrix  
6. **Visualization**: ROC curve, Heatmaps, Loss/Accuracy graphs  

---

## 🔍 Results

| Model          | Accuracy | F1 Score |
|----------------|----------|----------|
| CNN            | 87.2%    | 0.86     |
| Random Forest  | 83.5%    | 0.82     |
| SVM            | 81.7%    | 0.80     |

- 5-Fold Cross-validation: High stability with low variance
- CNN showed lowest false positives in classification

---

##  Visualization Samples

- Accuracy/Loss Curves
- Spectrogram Plots
- Confusion Matrices (Heatmaps)
- ROC and Precision-Recall Curves

> (Include visuals in `assets/` folder and reference them here)

---

## Future Scope

- Real-time acoustic streaming & analysis with edge devices (Raspberry Pi, etc.)
- Integration with meteorological and satellite data
- Geographic expansion to marine/forest biomes
- Community mobile app for local alerts

---

