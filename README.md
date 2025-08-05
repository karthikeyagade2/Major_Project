# Major_Project
# DLIDF: Deep Learning-Based Intrusion Detection Framework for Industrial IoT

![License](https://img.shields.io/badge/license-MIT-green)
![Python](https://img.shields.io/badge/Python-3.8+-blue)

> An advanced, scalable, and accurate deep learning-based intrusion detection framework built for real-time security in Industrial IoT environments.

---

## Overview

DLIDF is a modular, AI-powered Intrusion Detection System (IDS) that leverages a **Convolution2D (Conv2D)** based deep learning model to detect malicious network traffic in Industrial IoT (IIoT) systems. Built using Python, TensorFlow, and Gradio, this framework offers an intuitive GUI and provides high detection accuracy (up to **99%**) using the **UNSW-NB15** dataset.

Key Features:
- High Accuracy Intrusion Detection (99%+)
- Real-time attack prediction
- Performance comparison with baseline AutoEncoder-CNN
- Automatic feature extraction using Conv2D
- Web UI powered by Gradio
- Model saving/loading for reuse

---

##  Project Structure

```text
 DLIDF/
├── models/          # Saved models (Conv2D & AutoEncoder)
├── utils/           # Helper scripts (preprocessing, evaluation)
├── notebooks/       # Colab-compatible notebooks
├── app/             # Gradio UI components
├── datasets/        # Example datasets (UNSW-NB15 format)
├── results/         # Confusion matrices, metrics, visualizations
├── requirements.txt
└── README.md
```

---

##  Installation

### Prerequisites

- Python 3.8+
- pip
- A GPU-enabled environment (recommended)

###  Setup

```bash
git clone https://github.com/yourusername/DLIDF.git
cd DLIDF
pip install -r requirements.txt
```
Usage
#### Option 1: Run via Google Colab (Recommended)

Upload the dataset (e.g. UNSW-NB15.csv) and launch the Colab notebook.

#### Option 2: Local Execution

```bash
python app/main.py
```
This launches the Gradio web UI. You can:

Upload your dataset (CSV format)

Train models (AutoEncoder / Conv2D)

Detect intrusions

View accuracy, precision, recall, F1-score, and confusion matrix

| Model       | Accuracy | Precision | Recall | F1-Score |
| ----------- | -------- | --------- | ------ | -------- |
| AutoEncoder | \~92%    | 0.89      | 0.91   | 0.90     |
| Conv2D CNN  | **99%**  | 0.98      | 0.99   | 0.98     |

## Datasets
The model was trained using the [UNSW-NB15 Dataset](https://research.unsw.edu.au/projects/unsw-nb15-dataset), which contains diverse and labeled IoT network traffic.


Format: CSV with labeled traffic as "Normal" or "Attack"

Max size handled: ~90,000 samples (adjustable)

## Security & Ethical Considerations
The tool is meant strictly for educational and ethical research purposes.

Do not use this system on real networks without authorization.

All models and logs are locally stored and not uploaded to any external servers.


