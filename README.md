# AI-Powered Phishing Detection System

An AI-powered cybersecurity system for detecting phishing URLs using Machine Learning and Deep Learning techniques.

The project is designed to identify whether a URL is **legitimate or potentially phishing** by extracting URL-based features, applying trained AI models, comparing multiple classification algorithms, and evaluating their ability to generalize to previously unseen datasets.

---

## 1. Project Overview

Phishing is one of the most common forms of cybercrime. Attackers create deceptive URLs and websites that imitate legitimate services such as banking platforms, social-media websites, e-commerce platforms, email services, and other trusted organizations.

Traditional phishing detection systems commonly depend on:

* Blacklists
* Rule-based detection
* Signature matching
* Manually maintained threat databases

These approaches can struggle with newly created or previously unseen phishing URLs.

This project proposes an **AI-powered phishing detection system** that uses machine-learning and deep-learning techniques to identify suspicious URLs automatically.

The project focuses on:

* URL feature extraction
* Machine-learning classification
* Deep-learning comparison
* Model performance evaluation
* Cross-dataset validation
* Risk scoring
* Explainable predictions
* Web-based phishing detection

---

# 2. Research Motivation

The project is based on five IEEE Access research papers covering different aspects of AI-based phishing detection.

| No. | Research Area                    | Main Technique               |
| --- | -------------------------------- | ---------------------------- |
| 1   | Hybrid phishing detection        | LR + SVC + Decision Tree     |
| 2   | Deep-learning phishing detection | AutoEncoder + ResNet + GRU   |
| 3   | Adversarial phishing detection   | GAN/WGAN + multimodal models |
| 4   | Early phishing detection         | LightGBM                     |
| 5   | Cross-dataset validation         | XGBoost                      |

The selected literature demonstrates that high accuracy on a single dataset does not necessarily guarantee good real-world performance.

The 2026 IEEE Access study is particularly important because its XGBoost model achieved approximately **90.7% accuracy on its custom test dataset but 77.8% average accuracy across three independent datasets**, demonstrating the importance of dataset shift and generalization.

---

# 3. Problem Statement

Phishing attacks continue to evolve as attackers create new malicious URLs and websites designed to bypass traditional security mechanisms.

Existing blacklist and rule-based systems may fail to identify newly generated phishing URLs because the URLs may not yet exist in known threat databases.

Machine-learning and deep-learning approaches can learn patterns from phishing and legitimate URLs. However, existing AI-based systems still face several challenges:

1. Dataset dependency
2. Poor generalization to unseen datasets
3. False-positive predictions
4. Computational complexity
5. Adversarial attacks
6. Changing phishing URL structures
7. Lack of explainability

Therefore, this project aims to develop an **AI-powered phishing detection system capable of classifying URLs while evaluating model reliability across different datasets**.

---

# 4. Objectives

## Primary Objective

To develop an AI-powered system that automatically detects phishing URLs using machine-learning and deep-learning techniques.

## Secondary Objectives

* Extract meaningful features from URLs.
* Train multiple machine-learning models.
* Compare different classification algorithms.
* Evaluate model performance using multiple metrics.
* Perform cross-dataset validation.
* Generate a phishing risk score.
* Provide interpretable prediction results.
* Develop a web interface for URL analysis.
* Investigate the limitations of AI-based phishing detection.
* Provide a foundation for future adversarial and multimodal detection.

---

# 5. Literature Survey

## Paper 1

### Phishing Detection System Through Hybrid Machine Learning Based on URL

**Authors:** Abdul Karim, Mobeen Shahroz, Khabib Mustofa, Samir Brahim Belhaouari, S. Ramana Kumar Joga

**Year:** 2023

**Journal:** IEEE Access

**DOI:** 10.1109/ACCESS.2023.3252366

### Methodology

The study evaluates several machine-learning models:

* Decision Tree
* Logistic Regression
* Random Forest
* Naive Bayes
* Gradient Boosting
* KNN
* Support Vector Classifier

The proposed **LSD ensemble** combines:

```text
Logistic Regression
        +
Support Vector Classifier
        +
Decision Tree
```

The study additionally uses:

* Canopy Feature Selection
* Grid Search
* Cross-Fold Validation
* Soft voting
* Hard voting

The research uses URL-based phishing features.

### Advantages

* Compares multiple ML algorithms.
* Uses ensemble learning.
* Uses feature selection.
* Applies hyperparameter optimization.
* Uses cross-validation.
* Provides multiple evaluation metrics.

### Limitations

* Primarily URL-feature based.
* Limited multimodal information.
* Evaluation is mainly dataset-dependent.
* Does not primarily address adversarial phishing.
* Cross-dataset generalization is not the central focus.

---

# 6. Paper 2

## Enhancing Phishing Detection: A Novel Hybrid Deep Learning Framework for Cybercrime Forensics

**Authors:** Faisal S. Alsubaei, Abdulwahab Ali Almazroi, Nasir Ayub

**Year:** 2024

**Journal:** IEEE Access

**DOI:** 10.1109/ACCESS.2024.3351946

### Methodology

The paper proposes a hybrid deep-learning framework using:

* SMOTE
* Ensemble AutoEncoder
* ResNet
* GRU
* Attention mechanism
* Jaya Algorithm

The architecture includes an **Ensemble AutoEncoder with ResNet (EARN)** and a **ResNeXt/GRU-based component**.

SMOTE is used to address class imbalance.

The study reports approximately **98% accuracy with SMOTE** compared with 83% without SMOTE.

### Advantages

* Uses deep learning.
* Learns complex nonlinear representations.
* Addresses class imbalance.
* Combines multiple neural architectures.
* Uses optimization for model tuning.
* Achieves strong experimental performance.

### Limitations

* More computationally expensive than conventional ML.
* More difficult to implement and maintain.
* Requires more training resources.
* Performance may depend on the training dataset.
* Cross-dataset generalization requires further investigation.

---

# 7. Paper 3

## A Study on Adversarial Sample Resistance and Defense Mechanism for Multimodal Learning-Based Phishing Website Detection

**Authors:** Phan The Duy, Vo Quang Minh, Bui Tan Hai Dang, Ngo Duc Hoang Son, Nguyen Huu Quyen, Van-Hau Pham

**Year:** 2024

**Journal:** IEEE Access

**DOI:** 10.1109/ACCESS.2024.3436812

### Methodology

The study evaluates 15 ML, DL and multimodal models.

The authors propose:

**AWG — Adversarial Website Generation**

The framework uses:

* GAN
* WGAN
* Transfer-based black-box attacks
* Adversarial examples
* Multimodal learning
* Adversarial training

Datasets include sources such as:

* OpenPhish
* PhishTank
* Phishing Database
* Alexa

The study reports adversarial examples capable of bypassing several models with evasion rates of up to **88%**.

### Advantages

* Addresses adversarial attacks.
* Evaluates multiple ML/DL models.
* Uses multimodal learning.
* Uses realistic phishing sources.
* Investigates model robustness.
* Provides defense mechanisms.
* Provides source code for the AWG framework.

### Limitations

* Real adversarial phishing websites are scarce.
* GAN-based generation increases complexity.
* Requires significant computational resources.
* Primarily focuses on adversarial scenarios.
* More complex than a basic URL classifier.

---

# 8. Paper 4

## Machine Learning for Early Detection of Phishing URLs in Parked Domains: An Approach Applied to a Financial Institution

**Authors:** Jaqueline D. Duarte, Pedro Chagas Junior, João Paulo Javidi da Costa, Elena J. da Costa, Laerte Peotta de Melo, Rafael Rabelo Nunes, Carlos Gabriel V. N. Soares, Thiago Erivan da Cunha Silva

**Year:** 2025

**Journal:** IEEE Access

**DOI:** 10.1109/ACCESS.2025.3599454

### Methodology

The research proposes **Phishing Hunter**, a machine-learning framework for early phishing URL detection.

The system focuses particularly on:

* Newly registered domains
* Parked domains
* SSL certificate monitoring
* Popular domain information
* Phishing incident reports

The dataset contains **211,659 URLs**.

The study evaluates machine-learning models and identifies **LightGBM** as a strong-performing classifier.

Reported performance includes:

* Accuracy: 97.28%
* Recall: 96.02%
* 10-fold cross-validation

Feature selection is also used to reduce model complexity.

### Advantages

* Focuses on early detection.
* Uses a large dataset.
* Uses real-world sources.
* Suitable for proactive phishing prevention.
* Uses feature selection.
* Uses cross-validation.
* Strong recall is useful for cybersecurity.

### Limitations

* Focuses strongly on parked/new domains.
* May not cover every phishing technique.
* Depends on availability of domain and SSL-related information.
* Cross-dataset generalization is not the primary objective.
* Real-time deployment may require continuous feature updates.

---

# 9. Paper 5

## XGBoost-Based URL Phishing Detection Method With Cross-Dataset Validation

**Authors:** Milosz Misiek, Tomasz Hyla

**Year:** 2026

**Journal:** IEEE Access

**DOI:** 10.1109/ACCESS.2026.3672690

### Methodology

The paper proposes **X-PHIDE**, an XGBoost-based phishing URL detection system.

The system combines:

```text
URL
 ↓
Feature Extraction
 ↓
Allowlist / Blocklist
 ↓
XGBoost
 ↓
Prediction
```

The research uses:

* XGBoost
* Feature selection
* Bayesian hyperparameter optimization
* 5-fold stratified cross-validation
* Cross-dataset validation

Three datasets are used:

* Custom dataset — 75,738 samples
* GramBeddings — 639,723 samples
* PhiUSIIL — 47,103 compatible test samples

The study reports:

* 90.7% accuracy on the custom test dataset
* 77.8% average accuracy across three independent datasets
* 91.2% F1 score on the custom dataset
* Average F1 around 77.93% across datasets

The paper also reports that XGBoost trained substantially faster than the compared neural network.

### Advantages

* Strong tabular-data performance.
* Efficient training.
* Feature importance provides interpretability.
* Uses multiple datasets.
* Explicitly evaluates dataset shift.
* Suitable for real-time URL classification.
* Practical browser-extension architecture.

### Limitations

* Cross-dataset performance is considerably lower than single-dataset performance.
* Dataset shift remains a significant challenge.
* URL-based features cannot capture all webpage characteristics.
* False positives remain an issue.
* Current implementation is browser-specific.

---

# 10. Research Gap

The literature indicates several important research gaps.

## 10.1 Dataset Dependency

A model that performs well on one dataset may perform poorly on another.

The 2026 XGBoost research clearly demonstrates this issue through cross-dataset testing.

---

## 10.2 Generalization

Phishing URLs continuously change.

Therefore, the model must be capable of detecting URLs that were not represented in the training dataset.

---

## 10.3 Adversarial Robustness

Attackers can deliberately modify phishing URLs or websites to evade machine-learning models.

The adversarial study demonstrates that such modifications can successfully bypass several existing models.

---

## 10.4 Explainability

A practical phishing detector should not only return:

```text
PHISHING
```

It should ideally explain:

```text
Prediction: PHISHING

Risk Score: 94.6%

Major Risk Factors:
- Excessive URL length
- Suspicious keyword
- Multiple subdomains
- High URL entropy
- Unusual special characters
```

---

## 10.5 Real-Time Detection

The system should provide predictions quickly enough to be useful while a user is browsing.

---

# 11. Proposed System

```text
                         USER
                           |
                           v
                    Enter URL
                           |
                           v
                 URL Validation
                           |
                           v
                  Feature Extraction
                           |
             +-------------+-------------+
             |             |             |
             v             v             v
         URL Features  Domain Features  Text Features
             |             |             |
             +-------------+-------------+
                           |
                           v
                   Feature Selection
                           |
                           v
                 +-------------------+
                 |   AI Classifiers  |
                 +-------------------+
                    /      |       \
                   /       |        \
                  v        v         v
              XGBoost   LightGBM   Random Forest
                  \        |        /
                   \       |       /
                    v      v      v
                   Model Comparison
                           |
                           v
                    Risk Prediction
                           |
              +------------+------------+
              |                         |
              v                         v
          LEGITIMATE                 PHISHING
              |                         |
              +------------+------------+
                           |
                           v
                    Risk Assessment
                           |
                           v
                     Web Dashboard
```

---

# 12. Proposed AI Models

The initial project should compare:

| Model               | Purpose                   |
| ------------------- | ------------------------- |
| Logistic Regression | Baseline                  |
| SVM                 | Classical ML comparison   |
| Decision Tree       | Interpretable baseline    |
| Random Forest       | Ensemble baseline         |
| XGBoost             | Primary model             |
| LightGBM            | High-performance boosting |
| Neural Network      | Deep-learning comparison  |

---

# 13. URL Features

Potential features include:

### URL Structure

* URL length
* Domain length
* Path length
* Number of dots
* Number of hyphens
* Number of slashes
* Number of special characters
* Number of digits
* Number of parameters

### Domain

* Number of subdomains
* IP address usage
* Domain entropy
* Domain age
* Suspicious TLD
* HTTPS availability

### Suspicious Patterns

* Login-related keywords
* Banking keywords
* Account keywords
* Verification keywords
* Security-related keywords
* URL shortening

---

# 14. System Architecture

```text
                 +----------------+
                 |    Frontend    |
                 | HTML/CSS/JS    |
                 +-------+--------+
                         |
                         v
                 +----------------+
                 |   REST API     |
                 | Flask/FastAPI  |
                 +-------+--------+
                         |
                         v
              +----------------------+
              | URL Feature Extractor|
              +----------+-----------+
                         |
                         v
              +----------------------+
              | Feature Preprocessor |
              +----------+-----------+
                         |
                         v
              +----------------------+
              |     ML Pipeline      |
              +----------+-----------+
                         |
        +----------------+----------------+
        |                |                |
        v                v                v
     XGBoost          LightGBM       Random Forest
        |                |                |
        +----------------+----------------+
                         |
                         v
                  Prediction Engine
                         |
                         v
                   Risk Assessment
                         |
                         v
                     Database
```

---

# 15. Dataset Strategy

The project should avoid depending on only one dataset.

Possible datasets include:

* PhishTank
* OpenPhish
* PhiUSIIL
* GramBeddings
* Other publicly available legitimate URL datasets

The 2026 IEEE Access study demonstrates the value of combining training data with independent test datasets.

### Recommended experiment

```text
Dataset A
   |
   +----> Training
   |
   v
Dataset A
   |
   +----> Internal Test
   |
   v
Dataset B
   |
   +----> Cross-Dataset Test
   |
   v
Dataset C
   |
   +----> Generalization Test
```

---

# 16. Evaluation Metrics

The system should calculate:

### Accuracy

```text
Accuracy =
(TP + TN) / (TP + TN + FP + FN)
```

### Precision

```text
Precision =
TP / (TP + FP)
```

### Recall

```text
Recall =
TP / (TP + FN)
```

### F1 Score

```text
F1 =
2 × Precision × Recall
-----------------------
Precision + Recall
```

### Additional Metrics

* Specificity
* False Positive Rate
* False Negative Rate
* ROC-AUC
* Confusion Matrix
* Inference Time
* Model Size

---

# 17. Project Structure

Recommended structure:

```text
AI-Phishing-Detection/
│
├── README.md
│
├── data/
│   ├── raw/
│   ├── processed/
│   └── external/
│
├── notebooks/
│   ├── data_analysis.ipynb
│   ├── feature_analysis.ipynb
│   ├── model_training.ipynb
│   └── model_comparison.ipynb
│
├── src/
│   ├── data/
│   │   ├── preprocessing.py
│   │   └── dataset_loader.py
│   │
│   ├── features/
│   │   └── url_features.py
│   │
│   ├── models/
│   │   ├── xgboost_model.py
│   │   ├── lightgbm_model.py
│   │   ├── random_forest.py
│   │   ├── svm_model.py
│   │   └── neural_network.py
│   │
│   ├── evaluation/
│   │   └── metrics.py
│   │
│   └── prediction/
│       └── predictor.py
│
├── models/
│   ├── xgboost/
│   ├── lightgbm/
│   └── random_forest/
│
├── backend/
│   ├── app.py
│   ├── routes/
│   │   └── prediction.py
│   └── services/
│       └── phishing_detector.py
│
├── frontend/
│   ├── index.html
│   ├── style.css
│   └── script.js
│
├── tests/
│   ├── test_features.py
│   ├── test_models.py
│   └── test_api.py
│
├── requirements.txt
│
└── LICENSE
```

---

# 18. Installation

Clone the repository:

```bash
git clone <YOUR-REPOSITORY-URL>
cd AI-Phishing-Detection
```

Create the Python environment:

```bash
python -m venv venv
```

Activate it:

### Windows

```bash
venv\Scripts\activate
```

### Linux/macOS

```bash
source venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

# 19. Example Requirements

```text
numpy
pandas
scikit-learn
xgboost
lightgbm
matplotlib
seaborn
joblib
flask
fastapi
uvicorn
requests
```

---

# 20. Model Training

Example:

```bash
python src/models/xgboost_model.py
```

Train LightGBM:

```bash
python src/models/lightgbm_model.py
```

Train Random Forest:

```bash
python src/models/random_forest.py
```

---

# 21. Run the Backend

For Flask:

```bash
python backend/app.py
```

For FastAPI:

```bash
uvicorn backend.app:app --reload
```

The API can expose an endpoint such as:

```text
POST /api/predict
```

Example request:

```json
{
  "url": "https://example.com/login"
}
```

Example response:

```json
{
  "prediction": "legitimate",
  "risk_score": 0.04,
  "risk_level": "LOW"
}
```

---

# 22. Web Application

The web interface should allow users to:

1. Enter a URL.
2. Submit the URL for analysis.
3. View the prediction.
4. View the risk score.
5. View important URL features.
6. View the selected model.
7. View explanation/risk factors.

Example:

```text
+--------------------------------------+
|       AI PHISHING DETECTOR           |
+--------------------------------------+
|                                      |
| URL: https://example.com/login       |
|                                      |
|          [ ANALYZE URL ]             |
|                                      |
+--------------------------------------+

Prediction
----------------------------------------
LEGITIMATE

Risk Score
----------------------------------------
4.2%

Risk Level
----------------------------------------
LOW
```

---

# 23. Experimental Plan

## Experiment 1

Train and test models using the same dataset.

```text
Dataset
   |
   +--> Train 80%
   |
   +--> Test 20%
```

Compare:

* Accuracy
* Precision
* Recall
* F1
* Specificity

---

## Experiment 2

Perform cross-dataset evaluation.

```text
Dataset A
   |
   v
Training
   |
   v
Model
   |
   +----> Dataset B
   |
   +----> Dataset C
```

This experiment is particularly important because it measures real generalization rather than only memorization of dataset-specific patterns.

---

## Experiment 3

Compare computational performance.

Measure:

* Training time
* Prediction time
* Memory usage
* Model size

---

## Experiment 4

Analyze feature importance.

For XGBoost:

```text
Feature
   |
   v
Importance Score
   |
   v
Top Risk Factors
```

---

## Experiment 5 — Advanced

Test adversarial robustness.

Inspired by the 2024 IEEE Access adversarial study:

```text
Original Phishing URL
          |
          v
Adversarial Modification
          |
          v
Modified URL
          |
          v
AI Detector
          |
     +----+----+
     |         |
     v         v
Detected    Evaded
```

This should be performed only in a controlled research environment.

---

# 24. Expected Outcome

The final system is expected to:

* Detect phishing URLs automatically.
* Classify legitimate and phishing URLs.
* Compare multiple AI models.
* Provide phishing probability.
* Identify important risk features.
* Evaluate model generalization.
* Perform cross-dataset testing.
* Provide a web-based interface.
* Establish a foundation for adversarially robust phishing detection.

---

# 25. Future Enhancements

Future versions can include:

### 1. HTML Analysis

Analyze:

* HTML structure
* Forms
* Scripts
* Iframes
* External resources

### 2. Screenshot-Based Detection

Use CNN/vision models to analyze webpage screenshots.

### 3. Multimodal Detection

Combine:

```text
URL
 +
HTML
 +
Screenshot
 +
Domain information
```

This direction is motivated by the multimodal/adversarial research in the selected literature.

### 4. Adversarial Training

Generate controlled adversarial examples and train the detector to resist them.

### 5. Browser Extension

Integrate the trained model into:

* Chrome
* Firefox
* Edge

### 6. Real-Time Threat Intelligence

Integrate:

* PhishTank
* OpenPhish
* DNS information
* WHOIS information
* SSL information

### 7. Explainable AI

Use feature importance and explainability methods to show why a URL was classified as phishing.

---

# 26. Research Contribution

The primary contribution of this project is not simply achieving the highest possible accuracy.

The project focuses on:

```text
             AI PHISHING DETECTION
                     |
        +------------+------------+
        |            |            |
        v            v            v
    Detection    Generalization  Explainability
        |            |            |
        +------------+------------+
                     |
                     v
             Practical System
```

The project specifically addresses the research gap between **high single-dataset accuracy and reliable real-world phishing detection**.

---

# 27. Ethical Considerations

This project is intended for:

* Academic research
* Cybersecurity education
* Defensive security
* Controlled testing
* Phishing detection research

The system should not be used to create, distribute, or operate phishing websites.

Any adversarial testing should be performed only against controlled datasets, laboratory environments, or systems for which permission has been obtained.

---

# 28. Base Research Papers

### Paper 1

Abdul Karim et al.,
**"Phishing Detection System Through Hybrid Machine Learning Based on URL,"**
IEEE Access, 2023.

DOI:

```text
10.1109/ACCESS.2023.3252366
```

[IEEE Xplore paper](https://ieeexplore.ieee.org/document/10058201/?utm_source=chatgpt.com)

---

### Paper 2

Faisal S. Alsubaei et al.,
**"Enhancing Phishing Detection: A Novel Hybrid Deep Learning Framework for Cybercrime Forensics,"**
IEEE Access, 2024.

DOI:

```text
10.1109/ACCESS.2024.3351946
```

[IEEE Xplore paper](https://ieeexplore.ieee.org/document/10384876/?utm_source=chatgpt.com)

---

### Paper 3

Phan The Duy et al.,
**"A Study on Adversarial Sample Resistance and Defense Mechanism for Multimodal Learning-Based Phishing Website Detection,"**
IEEE Access, 2024.

DOI:

```text
10.1109/ACCESS.2024.3436812
```

[IEEE Xplore paper](https://ieeexplore.ieee.org/document/10620285/?utm_source=chatgpt.com)

---

### Paper 4

Jaqueline D. Duarte et al.,
**"Machine Learning for Early Detection of Phishing URLs in Parked Domains: An Approach Applied to a Financial Institution,"**
IEEE Access, 2025.

DOI:

```text
10.1109/ACCESS.2025.3599454
```

[IEEE Xplore paper](https://ieeexplore.ieee.org/document/11126023/?utm_source=chatgpt.com)

---

### Paper 5

Milosz Misiek and Tomasz Hyla,
**"XGBoost-Based URL Phishing Detection Method With Cross-Dataset Validation,"**
IEEE Access, 2026.

DOI:

```text
10.1109/ACCESS.2026.3672690
```

[IEEE Xplore paper](https://ieeexplore.ieee.org/document/11428202?utm_source=chatgpt.com)

---

# 29. License

This project is intended for academic and research purposes.

Add an appropriate open-source license before publishing the source code publicly.

---

# 30. Project Status

```text
Research        : Completed
Literature      : Completed
Problem         : Defined
System Design   : Defined
Dataset         : To be prepared
Feature Model   : To be implemented
ML Models       : To be implemented
Web Application : To be implemented
Evaluation      : To be conducted
Deployment      : Future stage
```

---

## Research Direction

The recommended implementation path is:

```text
Literature
    ↓
Dataset Collection
    ↓
Data Cleaning
    ↓
Feature Engineering
    ↓
Baseline ML
    ↓
XGBoost + LightGBM
    ↓
Model Comparison
    ↓
Cross-Dataset Validation
    ↓
Explainable Prediction
    ↓
Web Application
    ↓
Adversarial Testing
    ↓
Final Research Evaluation
```

This structure keeps the project closely connected to the five selected IEEE Access papers while giving it a clear **research contribution rather than being only a phishing-classification demo**.
