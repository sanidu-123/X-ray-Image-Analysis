# X-Ray Disease Classification & LLM-Assisted Interpretation
## A Hybrid Deep Learning Framework for Automated Chest X-Ray Analysis

This repository contains the complete implementation of a hybrid diagnostic-support system that integrates:

* CNN-based chest X-ray disease classification
* LLM-based medical explanation generation
  
The project is derived from the final research thesis:
### “X-Ray Image Classification of Multiple Diseases and LLM-Assisted Interpretation Using Deep Learning Architectures for Optimized Radiology Image Analysis.”

The goal is to build an interpretable, accurate, and resource-efficient AI tool to support radiologists and improve diagnostic workflow speed.

### 🚀 Key Features
🔍 1. Chest X-Ray Disease Classification

Multi-label predictions for 5 thoracic diseases:
* Lung Opacity
* Pleural Effusion
* Edema
* Atelectasis
* Cardiomegaly

🧠 2. Hybrid Model Architecture

* DenseNet-121 & ResNet-50 trained independently
* Integrated through weighted ensemble voting
* Improves recall, stability, and overall prediction reliability

🗣️ 3. LLM-Assisted Explanation (FLAN-T5)

* Generates clinical-style text explanations
* Uses disease-specific templates and a medical knowledge base
* Improves interpretability and user trust

🛡️ 4. Safety Features

* Detects non-X-ray images
* Includes clinical-use disclaimer
* Validated on CheXpert dataset

### 📊 Model Performance (Summary)
| Disease          | Accuracy | Weighted F1 | Notes                           |
| ---------------- | -------- | ----------- | ------------------------------- |
| Lung Opacity     | 0.77     | 0.77        | Strong recall                   |
| Pleural Effusion | 0.84     | 0.84        | Most consistent                 |
| Edema            | 0.81     | 0.82        | Good sensitivity                |
| Atelectasis      | 0.70     | 0.70        | Moderate performance            |
| Cardiomegaly     | 0.72     | 0.73        | Balanced after threshold tuning |

### Workflow

1. Upload chest X-ray image
2. CNN ensemble classifies 5 diseases
3. LLM generates an explanation
4. System outputs a full structured report

### 🧪 Evaluation Metrics Used

* Accuracy
* Precision
* Recall
* F1-score (Macro & Weighted)
* Confusion Matrix
* Class imbalance handling

### ⚠️ Disclaimer

This project is for research and academic purposes only.
It is not intended for clinical diagnosis and must not be used in medical decision-making.

### 👨‍💻 Author
Sanidu S. Hewage - BSc (Hons) in Data Science – NSBM Green University
