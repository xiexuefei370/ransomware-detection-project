# ransomware-detection-project
# Early-Stage Ransomware Detection System

## Project Overview

This project presents an early-stage ransomware detection system that combines static analysis and dynamic behavioural analysis to identify malicious activity before encryption occurs.

Traditional ransomware detection methods are often reactive, detecting attacks only after damage has already been done. This project addresses this limitation by focusing on early-stage API call sequences and lightweight static features, enabling faster and more proactive detection.

---

## Objectives

The main objectives of this project are:

- To investigate whether ransomware can be detected during the early stages of execution
- To evaluate the effectiveness of static features in modern malware detection
- To analyse API call sequences as behavioural indicators
- To develop a hybrid detection framework combining static and dynamic features
- To compare machine learning models for early-stage detection performance

---

## System Architecture

The proposed system follows a structured pipeline:

1. Data Collection  
2. Feature Extraction  
3. Data Processing  
4. Model Training  
5. Evaluation  

The system integrates:
- Static features (PE file structure, imported libraries)
- Dynamic features (early-stage API call sequences)

---

## Technologies Used

- Python  
- scikit-learn  
- TensorFlow / PyTorch  
- pandas  
- NumPy  
- pefile  
- Cuckoo Sandbox  
- VirtualBox  

---

## Dataset

The dataset consists of:

- Ransomware samples collected from public repositories
- Benign software samples for comparison

Due to ethical and legal restrictions, the dataset is not included in this repository. Public datasets such as MalwareBazaar and VirusShare can be used.

---

## Feature Extraction

### Static Features
- PE header attributes  
- Imported DLLs and functions  
- File entropy and metadata  

### Dynamic Features
- API call sequences extracted from sandbox execution  
- Focus on early-stage execution behaviour  

---

## Models Implemented

### 1. Random Forest
- Efficient and interpretable
- Suitable for structured feature data
- Provides feature importance insights

### 2. Long Short-Term Memory (LSTM)
- Designed for sequential data
- Captures temporal dependencies in API call sequences
- Higher accuracy but increased computational cost

---

## Evaluation Metrics

The system is evaluated using:

- Accuracy  
- Precision  
- Recall  
- F1-score  
- Confusion Matrix  

---

## Key Findings

- Early-stage API call sequences contain meaningful behavioural patterns  
- Hybrid feature integration improves detection performance  
- Random Forest provides strong baseline performance  
- LSTM achieves better sequence modelling but requires more resources  
- A trade-off exists between detection speed and accuracy  

---

## Limitations

- Dataset imbalance affects minority class detection  
- Sandbox environments may not fully reflect real-world behaviour  
- LSTM introduces higher computational cost  
- Some ransomware may evade analysis using anti-sandbox techniques  

---

## Future Work

- Improve dataset balance using resampling techniques  
- Explore lightweight sequence models for real-time detection  
- Enhance robustness against evasion techniques  
- Evaluate system performance in real-world environments  

---

## Repository Structure
