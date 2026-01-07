# ECG Arrhythmia Classification Using Deep Learning

## 📌 Overview
This project implements an **advanced machine learning pipeline** for **automatic ECG arrhythmia classification** using deep learning.  
It leverages **signal processing techniques** and a **neural network model** to classify multiple heart rhythm abnormalities from ECG waveforms.

The system is built and evaluated using the **MIT-BIH Arrhythmia Dataset**, a widely used benchmark in medical signal analysis.

---

## 🧠 Problem Statement
Manual ECG analysis is time-consuming and prone to human error.  
This project aims to:
- Automatically classify ECG signals
- Detect multiple arrhythmia types
- Support clinical decision-making using AI

---

## 📊 Dataset
- **MIT-BIH Arrhythmia Database**
- ECG signals sampled at 360 Hz
- Annotated heartbeat classes

### Classes Used
- **N** – Normal
- **L** – Left bundle branch block
- **R** – Right bundle branch block
- **A** – Atrial premature beat
- **S** – Supraventricular ectopic beat
- **V** – Premature ventricular contraction

---

## ⚙️ Technologies Used
- **Python**
- **TensorFlow / Keras** – Deep learning model
- **NumPy & Pandas** – Data processing
- **SciPy** – Signal filtering (Butterworth bandpass)
- **WFDB** – ECG data handling
- **Scikit-learn** – Encoding, cross-validation, metrics
- **Matplotlib** – Visualization

---

## 🔄 Pipeline Overview

### 1️⃣ Data Acquisition
- Downloaded MIT-BIH Arrhythmia dataset directly from PhysioNet
- Parsed ECG signals and annotations using WFDB

### 2️⃣ Signal Preprocessing
- Applied **Butterworth bandpass filtering** to remove noise
- Normalized ECG signals
- Segmented ECG signals into fixed-length beats

### 3️⃣ Feature Encoding
- Encoded heartbeat labels using **One-Hot Encoding**
- Prepared data for deep learning input format

### 4️⃣ Model Architecture
- Deep neural network using **Keras Sequential API**
- Regularization using **L2 penalties**
- Optimized using **Adam optimizer**

### 5️⃣ Training & Validation
- Used **K-Fold Cross-Validation** for robust evaluation
- Model checkpoints to save best-performing weights
- Monitored loss and accuracy during training

### 6️⃣ Evaluation
- Generated **confusion matrix**
- Evaluated multi-class classification performance
- Visualized ECG samples and model predictions

---

## 📈 Results & Findings
- Successfully classified multiple arrhythmia classes
- Demonstrated strong performance on clean, filtered ECG signals
- Highlighted the importance of signal preprocessing in medical ML

---

## 📁 Project Structure
