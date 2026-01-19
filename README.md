# Deep ResNIDS

This repository contains the implementation of **Deep ResNIDS**, a Two-Layer Network Intrusion Detection System (NIDS) designed to detect both **known** and **zero-day attacks**.

The system combines:
1. **Malicious Packet Detector (Supervised Layer)**  
   - Built using **Logistic Regression**  
   - Identifies malicious packets based on known attack patterns.  

2. **Anomaly Detector (Unsupervised Layer)**  
   - Implemented with an **Autoencoder**  
   - Detects **zero-day, adversarial, and automated attacks** by learning the distribution of normal traffic and flagging anomalies through **reconstruction error analysis**.  

---

## ✨ Key Features
- **100% detection rate** for known attacks.  
- **Robust anomaly detection** to capture novel threats.  
- Built in a **Jupyter Notebook** for clarity, experimentation, and reproducibility.  
- Modular and extendable to other machine learning and deep learning models.  

---

## 📂 Dataset

⚠️ The dataset used is **not for public use**.  
It consists of **network flow features (normalized) with labeled traffic samples**, used for supervised and unsupervised intrusion detection tasks.  

To replicate or extend this work, you can use publicly available datasets such as:  
- [NSL-KDD](https://www.unb.ca/cic/datasets/nsl.html) – Benchmark IDS dataset with normal and attack records.  
- [CICIDS 2017](https://www.unb.ca/cic/datasets/ids-2017.html) – Realistic modern traffic with various attack scenarios.  
- [UNSW-NB15](https://research.unsw.edu.au/projects/unsw-nb15-dataset) – Rich set of features with updated threats and normal traffic.  

---

## ⚙️ Dependencies

- Python 3.8+  
- NumPy  
- Pandas  
- Scikit-learn  
- TensorFlow / Keras  
- Matplotlib  

