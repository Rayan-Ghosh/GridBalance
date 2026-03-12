# GridBalance: Applied Research in Continuous-Time Grid Stability ⚡

![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Research](https://img.shields.io/badge/Type-Applied_Research-purple)

## 📄 Abstract
This repository contains the research and implementation notebook for **GridBalance**, an exploratory model designed to predict smart grid instability in real-time. Traditional recurrent networks struggle with the continuous, high-frequency nature of sensor data. This research investigates the efficacy of **Liquid Time-Constant (LTC) neural networks** mapped via **Neural Circuit Policies (AutoNCP)** to maintain continuous-time states for anomaly detection.

## 🔬 Methodology
The research focuses on bypassing discrete-time limitations by leveraging fluid neural architectures:
* **Framework:** PyTorch combined with the `ncps` library.
* **Data Pipeline:** Analyzed and augmented a 60,000-sample time-series dataset simulating grid fluctuations. 
* **Algorithmic Concept:** The notebook explores a simulated self-healing algorithm designed to output non-Newtonian correction vectors when the probability of grid instability exceeds critical thresholds.

## 📊 Key Findings & Results
The applied LTC model demonstrated significant promise in handling streaming sequential data without severe memory decay:
* **Validation Accuracy:** 97.13%
* **Loss Optimization:** Binary Cross-Entropy (BCE) proved highly stable during the AutoNCP wiring phase.

## 📂 Repository Contents
* `GridBalance_Research.ipynb`: The primary Jupyter Notebook containing the data structuring, model architecture, training loops, and validation metrics. 
* `requirements.txt`: Environment dependencies required to reproduce the training and validation loops.

## ⚙️ Quick Start
To reproduce the research environment locally:
```bash
git clone [https://github.com/YourUsername/GridBalance.git](https://github.com/YourUsername/GridBalance.git)
cd GridBalance
pip install -r requirements.txt
