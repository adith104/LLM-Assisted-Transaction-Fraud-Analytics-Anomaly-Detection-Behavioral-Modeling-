Here is a clean, professional **README.md** with no emojis—focused, technical, and suitable for GitHub.

---

# LLM-Assisted Transaction Fraud Analytics 

This repository contains an end-to-end fraud analytics framework integrating anomaly detection, behavioral modeling, graph features, and LLM-generated AML case narratives. The system is designed for research, prototyping, and educational use in financial crime analytics.

---

## Overview

This project builds a hybrid fraud-detection engine combining statistical anomaly models, temporal dynamics, and device-level graph analysis. It includes an LLM-based investigator that converts anomaly traces into structured AML-style narratives for compliance and forensic review.

---

## Key Features

### Anomaly Detection

* Isolation Forest, Local Outlier Factor, and One-Class SVM ensemble
* Sigmoid-calibrated fraud risk scores
* Auto-threshold tuning for optimal recall

### Behavioral Modeling

* Inter-arrival time (IAT) spikes
* Rolling temporal burst scores
* Transaction amount drift (rolling mean and std deviations)

### Graph-Based Features

* Synthetic device-linkage graph
* Degree centrality and community detection
* Network-based anomaly patterns

### LLM-Based AML Investigation

* GPT-4o integration for narrative generation
* Converts anomaly subsets into forensic summaries
* Highlights money-mule indicators, structuring, layering, and behavioral drift
* Stub mode available when no API key is provided

### Visualization Suite

* Risk distribution plots
* PCA projection of transaction embeddings
* Amount–risk scatter analysis
* Burst-score timeline
* Community graph visualization

---

## Notebook Version

The `ipynb` version includes:

* Interactive visualizations (Plotly)
* Ensemble model training and evaluation
* Auto-threshold selection
* GPT-4o narrative generation
* Community graph plots

---

## Dataset

This project uses the public **Credit Card Fraud Detection** dataset:

Kaggle: [https://www.kaggle.com/mlg-ulb/creditcardfraud](https://www.kaggle.com/mlg-ulb/creditcardfraud)

Place the dataset in the project directory as:

```
creditcard.csv
```

---

## Requirements

Install the dependencies:

```
pip install -r requirements.txt
```

Recommended libraries include:

* numpy
* pandas
* matplotlib
* seaborn
* plotly
* scikit-learn
* networkx
* openai
* scipy

---

## Running the Project

**Python script version:**

```
python fraud_main.py
```

**Jupyter notebook version:**

```
jupyter notebook Advanced_Fraud_Analytics.ipynb
```

---

## API Key Configuration

To enable GPT-4o narrative generation, insert your OpenAI API key directly in the code or store it in a `.env` file.

If no key is provided, the system runs in safe stub mode.

---

## Output

The pipeline produces:

* Risk-scored transaction dataset
* Flagged anomalies
* Visual diagnostics
* A full AML-style narrative for the highest-risk cases

---

## Disclaimer

This project is intended solely for research, education, and prototyping.
It is not a production fraud-detection system and must not be used for real financial decision-making.

---

If you'd like, I can also create:

* a `requirements.txt`
* a project folder structure
* a more formal technical documentation section
* or an architecture diagram.
