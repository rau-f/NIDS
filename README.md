# Network Intrusion Detection System

A machine learning-based approach to network intrusion detection using the KNN algorithm for classification of network traffic patterns.

## Quick Start

1. **Set environment:**
   ```bash
   cd nids
   python3 -m venv venvNIDS
   source venvNIDS/bin/activate
   pip install -r requirements.txt
   ```
2. **Launch Jupyter:**
   ```bash
   jupyter notebook
   ```

3. **Open the notebook:**
   Navigate to `source/notebook.ipynb` in your browser.

## Project Structure

- `source/notebook.ipynb` — Model training and evaluation pipeline
- `dataset/network_traffic.csv` — Network traffic dataset
- `requirements.txt` — Python dependencies

## Features

- Data preprocessing and feature extraction
- KNN-based classification model
- Performance metrics and evaluation

## Requirements

See `requirements.txt` for dependencies. Use Python 3.12+.