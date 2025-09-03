# Network Traffic Anomaly Detection System

## 📌 Overview
A **PyTorch-based anomaly detection system** using the **CICIDS 2017 dataset**, featuring a **contrastive autoencoder** for network traffic analysis.

---

## ✨ Key Features

### 🔹 Contrastive Autoencoder Architecture
- Multi-layer encoder-decoder with configurable hidden dimensions  
- Projection head for contrastive learning  
- Dropout and regularization for improved generalization  

### 🔹 Optimization Techniques
- Contrastive pretraining with **InfoNCE loss** and data augmentation  
- **Sparsity regularization** using L1 penalty on latent representations  
- **Early stopping** based on validation loss with patience mechanism  
- Learning rate scheduling with **reduction on plateau**  

### 🔹 Loss Function Components
- **Reconstruction Loss**: Mean Squared Error (MSE)  
- **Contrastive Loss**: InfoNCE for self-supervised learning  
- **Sparsity Loss**: L1 regularization on latent space  

### 🔹 Comprehensive Visualization
- Training progress with **loss component tracking**  
- Reconstruction error distributions (**normal vs. anomaly**)  
- Performance metrics: **ROC curves, PR curves, confusion matrix**  
- Box plots and cumulative distributions  

---

## 📊 Evaluation Metrics
- Accuracy, Precision, Recall, F1-Score  
- AUC-ROC and Average Precision  
- Confusion matrix visualization  

---

## 📂 Dataset
- Uses the **CICIDS 2017 dataset** for network traffic anomaly detection.  
- [Dataset Link](https://www.unb.ca/cic/datasets/ids-2017.html)  

---

## ⚙️ Requirements
- PyTorch  
- NumPy, Pandas  
- Matplotlib, Seaborn  
- Scikit-learn  

Install dependencies:
```bash
pip install -r requirements.txt
