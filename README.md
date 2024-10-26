# Heart Disease Prediction Project

A machine learning web application for predicting heart disease using deep learning techniques.

## Features

- Deep neural network model for heart disease prediction
- Web interface built with Flask
- REST API for programmatic access
- Comprehensive data preprocessing
- Real-time predictions with confidence scores

## Project Structure

```
Heart Disease Prediction/
├── app.py                  # Main Flask application
├── config.py              # Configuration settings
├── requirements.txt        # Python dependencies
├── setup.py               # Automated setup script
├── run.py                 # Application runner
├── wsgi.py                # WSGI entry point
├── generate_synthetic_data.py  # Data generation script
├── data/
│   └── ECG-Dataset.csv    # Dataset
├── models/
│   ├── heart_disease_model.h5  # Trained model
│   ├── scaler.pkl         # Data scaler
│   └── train_model.py     # Model training script
├── templates/             # HTML templates
├── static/               # CSS and JavaScript
└── utils/
    └── preprocessing.py  # Data preprocessing utilities
```

## Quick Start

1. Clone the repository
2. Install dependencies: `pip install -r requirements.txt`
3. Generate data (if needed): `python generate_synthetic_data.py`
4. Train model (if needed): `python models/train_model.py`
5. Run the application: `python app.py`
6. Open http://127.0.0.1:5000 in your browser

## Model Performance

- Algorithm: Deep Neural Network
- Architecture: 16 → 8 → 1 neurons with dropout layers
- Accuracy: 63% on test data

## Dependencies

- Flask 2.3.3
- TensorFlow 2.20.0
- Pandas, NumPy, Scikit-learn
- Matplotlib, Seaborn
