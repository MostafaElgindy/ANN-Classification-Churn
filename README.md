# Customer Churn Prediction using ANN

A deep learning project that predicts customer churn using Artificial Neural Networks built with TensorFlow and Keras.

## Overview

This project uses an Artificial Neural Network to analyze customer data and predict whether a customer will leave the service (churn) or not.

## Project Structure

```
ANN-Project/
├── app.py                              # Streamlit web application
├── experiments.ipynb                   # Model development notebook
├── prediction.ipynb                    # Prediction testing notebook
├── Churn_Modelling.csv                # Dataset
├── churn_model.h5                     # Trained model
├── label_encoder_gender.pkl           # Gender encoder
├── onehot_encoder_geography.pkl       # Geography encoder
├── scaler.pkl                         # Feature scaler
├── requirements.txt                   # Dependencies
└── README.md                          # Documentation
```

## Installation

1. Clone the repository
   ```bash
   git clone <repository-url>
   cd ANN-Project
   ```

2. Install dependencies
   ```bash
   pip install -r requirements.txt
   ```

## Usage

### Train the Model
```bash
jupyter notebook experiments.ipynb
```

### Run Web Application
```bash
streamlit run app.py
```

### Make Predictions
```bash
jupyter notebook prediction.ipynb
```

## Model Architecture

```
Input Layer:  12 features
    ↓
Hidden Layer 1: 64 neurons (ReLU)
    ↓
Hidden Layer 2: 32 neurons (ReLU)
    ↓
Output Layer: 1 neuron (Sigmoid)
```

**Hyperparameters:**
- Optimizer: Adam (lr=0.01)
- Loss: Binary Crossentropy
- Epochs: 100 (with early stopping)
- Validation Split: 20%

## Technologies Used

- Python 3.11
- TensorFlow/Keras
- Pandas & NumPy
- Scikit-learn
- Streamlit
- Jupyter Notebook

## Results

- Training Accuracy: ~86%
- Validation Accuracy: ~85%

---

Made with ❤️ for learning deep learning
