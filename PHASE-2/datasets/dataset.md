# Phishing Detection Datasets

This directory contains datasets used for the
AI-Powered Phishing Detection System.

## 1. PhiUSIIL

Source:
UCI Machine Learning Repository

Dataset ID:
967

Samples:
235,795

Classes:
- Legitimate
- Phishing

Features:
54

Official source:
https://archive.ics.uci.edu/dataset/967/phiusiil+phishing+url+dataset

---

## 2. UCI Phishing Websites

Source:
UCI Machine Learning Repository

Dataset ID:
327

Samples:
11,055

Features:
30

Classes:
- Legitimate
- Phishing

Official source:
https://archive.ics.uci.edu/dataset/327/phishing+websites

---

## 3. PILU-90K

Paper:
Phishing URL Detection:
A Real-Case Scenario Through Login URLs

Publisher:
IEEE Access

DOI:
10.1109/ACCESS.2022.3168681

Dataset size:
90,000 URLs

Classes:

30,000 legitimate homepage URLs
30,000 legitimate login URLs
30,000 phishing URLs

PILU-90K will be used as an independent
evaluation dataset where appropriate.

---

## Dataset Usage

The datasets are NOT automatically merged.

Each dataset should first be analyzed independently.

Experiments may include:

1. Within-dataset training/testing
2. Cross-dataset testing
3. Feature compatibility analysis
4. Model generalization analysis
5. Error analysis
