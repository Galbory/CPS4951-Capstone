# CPS4951-Capstone
Capstone code and database
## 🎬 IMDb Sentiment Analysis
## 1. Project Overview
This repository implements sentiment classification on the IMDb dataset and compares following model:
- **LDA + Logistic Regression**
- **BiLSTM**
- **BERT**
- **LDA-BERT**
- **BERT-BiLSTM**
Each model is trained and evaluated across multiple fixed random seeds to ensure experimental reproducibility.
After training, the framework automatically computes and records several key performance metrics, including Accuracy, Macro-F1, AUC, and Running Time.
To assess statistical significance, paired t-tests are conducted between models.
In addition, detailed error analysis is performed to identify false positives and false negatives, followed by the generation of confusion matrices and ROC curves for visual comparison.

Overall, this project aims to explore the performance, efficiency, and reliability trade-offs among classical, deep, and hybrid NLP models under a controlled experimental setting.

## 🧱 Project Structure 
### 📂 Before Running 
```bash
.
├── IMDB Dataset.zip          # Raw IMDb dataset 
├── bert-base-uncased.zip     # Offline BERT model snapshot
├── code.ipynb                # Main notebook for experiments 
├── environment.yml           # Conda environment definition
├── requirements.txt          # pip dependency list
└── README.md                 # Project documentation 
```

## ⚙️ Environment Setup
```bash
There are two ways to set up the environment for this project:  
1. Using **pip** with `requirements.txt`
2. Using **Conda** with the provided `environment.yml`

It is recommended to install dependencies using **pip** for simplicity and speed.  
If any environment conflicts occur (e.g., CUDA or PyTorch version issues), you may alternatively use **Conda**.
```
### 🔹 Option A — Using pip (Recommended)

```bash
# Install all dependencies
pip install -r requirements.txt
```

### 🔹 Option B — Using Conda
# Create a new environment
conda env create -f environment.yml
# Activate the environment
conda activate imdb-sentiment
```

