# Automatic Pain Recognition System for Dental Patients Using Machine Learning

🚧 **Status:** Completed Research 📄 Publication: 🔗 https://perintis.org.my/ejournalperintis/index.php/PeJ/article/view/164


<img width="1024" height="1536" alt="image" src="https://github.com/user-attachments/assets/357a80ee-28a3-42c2-bf10-9c3f889d782d" />

---

## Overview
This project presents a machine learning-based system for automatic pain recognition in dental patients using bio-signals. The system objectively classifies pain levels into **High Pain, Mild Pain, and No Pain**, reducing reliance on subjective patient feedback during treatment. 

---

## Problem Statement
- Patients struggle to communicate pain accurately during dental procedures  
- Self-reporting is subjective and inconsistent  
- Misinterpretation of pain disrupts treatment efficiency 

---

## System Architecture


- Sensors collect physiological signals  
- Raspberry Pi acts as processing unit  
- Python (Jupyter Notebook) used for model training/testing  
- Output delivered via visual + voice interface 

---

## System Flow (Actual Flow from Paper)



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

Signals are sampled, filtered, and preprocessed before training. 

---

## Signal Processing
- ECG sampled at **500 Hz**  
- Filtering using **MATLAB (bandpass filters)**  
- Feature extraction from ECG, EEG, EMG  
- Normalization before ML input 

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
- Multinomial Naive Bayes 

### Training Setup
- **80% training / 20% testing split**  
- Input: Bio-signals  
- Output: Pain classification 

---

## Results
- **Best Model:** Random Forest  
- **Accuracy:** 65.1%  
- **Precision:** 0.56  
- **Recall:** 0.56  
- **F1 Score:** 0.56 

### Insight 
- Random Forest performed best across all metrics  
- KNN showed highest recall  
- Other models underperformed due to nonlinear signal complexity 

---

## Output System


- Graph showing probability of pain levels  
- Voice output announcing predicted pain  
- Combined visual + auditory feedback for better usability 

---

## Key Contributions
- Low-cost, non-invasive pain detection system  
- Multi-modal bio-signal integration (ECG + EEG + EMG)  
- Objective alternative to subjective pain reporting  
- Real-time classification capability 

---

## Tech Stack
- **Hardware:** Arduino, Raspberry Pi 4, AD8232, BITalino  
- **Software:** Python, MATLAB, Jupyter Notebook, Arduino IDE  
- **ML Libraries:** Scikit-learn  

---

## Vision
To develop an intelligent, real-time, and reliable pain assessment system for clinical environments, improving decision-making and patient care in dentistry. 

> ⚠️ **Data Availability**  
> As real human bio-signals were used, the dataset and backend processing details are **not publicly available** but can be **accessed upon reasonable request**.
