# Automatic Pain Recognition System for Dental Patients Using Machine Learning

🚧 **Status:** Completed Research / Extendable for Future Work

---

## Overview
This project presents a machine learning-based system for automatic pain recognition in dental patients using bio-signals. The system objectively classifies pain levels into **High Pain, Mild Pain, and No Pain**, reducing reliance on subjective patient feedback during treatment. :contentReference[oaicite:0]{index=0}

---

## Problem Statement
- Patients struggle to communicate pain accurately during dental procedures  
- Self-reporting is subjective and inconsistent  
- Misinterpretation of pain disrupts treatment efficiency :contentReference[oaicite:1]{index=1}

---

## System Architecture
(From *Figure 2 – Block Diagram, Page 5*)

- Sensors collect physiological signals  
- Raspberry Pi acts as processing unit  
- Python (Jupyter Notebook) used for model training/testing  
- Output delivered via visual + voice interface :contentReference[oaicite:2]{index=2}

---

## System Flow (Actual Flow from Paper)
(From *Figure 1 – Page 4*)
:contentReference[oaicite:3]{index=3}

---

## Data Collection
- **Subjects:** 8 individuals  
- **Pain Classes:** No Pain, Mild Pain, High Pain  
- **Sensors Used:**
  - ECG → AD8232 sensor (heart activity)  
  - EEG → BITalino (brain signals)  
  - EMG → BITalino (muscle activity)  

### Sensor Placement
- ECG: Arms + right leg  
- EEG: Forehead / scalp  
- EMG: Jaw muscles  

Signals are sampled, filtered, and preprocessed before training. :contentReference[oaicite:4]{index=4}

---

## Signal Processing
- ECG sampled at **500 Hz**  
- Filtering using **MATLAB (bandpass filters)**  
- Feature extraction from ECG, EEG, EMG  
- Normalization before ML input :contentReference[oaicite:5]{index=5}

---

## Machine Learning Models
- Random Forest  
- K-Nearest Neighbors  
- Bagging Classifier  
- Decision Tree  
- Logistic Regression  
- SGD Classifier  
- Linear SVC  
- AdaBoost  
- Multinomial Naive Bayes :contentReference[oaicite:6]{index=6}

### Training Setup
- **80% training / 20% testing split**  
- Input: Bio-signals  
- Output: Pain classification :contentReference[oaicite:7]{index=7}

---

## Results
- **Best Model:** Random Forest  
- **Accuracy:** 65.1%  
- **Precision:** 0.56  
- **Recall:** 0.56  
- **F1 Score:** 0.56 :contentReference[oaicite:8]{index=8}

### Insight (Page 10–11)
- Random Forest performed best across all metrics  
- KNN showed highest recall  
- Other models underperformed due to nonlinear signal complexity :contentReference[oaicite:9]{index=9}

---

## Output System
(From *Figure 13 – Page 12*)

- Graph showing probability of pain levels  
- Voice output announcing predicted pain  
- Combined visual + auditory feedback for better usability :contentReference[oaicite:10]{index=10}

---

## Key Contributions
- Low-cost, non-invasive pain detection system  
- Multi-modal bio-signal integration (ECG + EEG + EMG)  
- Objective alternative to subjective pain reporting  
- Real-time classification capability :contentReference[oaicite:11]{index=11}

---

## Limitations
- Small dataset (8 subjects)  
- No real dental patient data during treatment  
- Moderate accuracy (65.1%) :contentReference[oaicite:12]{index=12}

---

## Future Work
- Collect real patient data during dental procedures  
- Increase dataset size  
- Use advanced deep learning models  
- Integrate medical-grade sensors for better accuracy :contentReference[oaicite:13]{index=13}

---

## Tech Stack
- **Hardware:** Arduino, Raspberry Pi 4, AD8232, BITalino  
- **Software:** Python, MATLAB, Jupyter Notebook, Arduino IDE  
- **ML Libraries:** Scikit-learn  

---

## Vision
To develop an intelligent, real-time, and reliable pain assessment system for clinical environments, improving decision-making and patient care in dentistry. :contentReference[oaicite:14]{index=14}
