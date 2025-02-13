# Dog Breed Classifier

A machine learning model for classifying dog breeds from images.

## Overview

This Python-based model uses multiple machine learning techniques to classify images of dogs into specific breeds. The system compares the performance of Random Forest, Support Vector Machine (SVM), and K-Nearest Neighbors (KNN) algorithms.

## Features

- Multi-model comparison (Random Forest, SVM, KNN)
- Automated data preprocessing and normalization
- Performance visualization with confusion matrices
- Model persistence for future use

## Data Preparation

The system processes the input data through several steps:

1. Loads and validates image labels from CSV
2. Standardizes image formats for consistency
3. Normalizes pixel values for better model performance
4. Performs one-hot encoding on breed labels
5. Splits data into training, validation, and test sets

## Model Training

The training pipeline includes:

1. Random Forest Classifier
2. Support Vector Machine (SVM)
3. K-Nearest Neighbors (KNN)

Each model is trained on identical data splits for fair comparison.

## Evaluation

The system evaluates models using:

- Accuracy scores
- F1 scores
- Confusion matrices
- Performance comparison visualization

## Model Persistence

The best-performing Random Forest model is automatically saved using the Joblib library for future use.

## Usage

1. Configure breed selection:
```python
CLASS_NAMES = ['scottish_deerhound', 'maltese_dog', 'bernese_mountain_dog']
```

2. Set up your environment:
   - Ensure all required dependencies are installed
   - Verify dataset path and file structure
   - Check image format compatibility

3. Run the training pipeline:
```python
python train_model.py
```

4. Use the trained model:
```python
from joblib import load
model = load('random_forest_model.joblib')
predictions = model.predict(new_images)
```

## Requirements

- Python 3.8+
- scikit-learn
- numpy
- pandas
- matplotlib
- joblib
- PIL (Python Imaging Library)

## Directory Structure

```
DogClassifier/
├── README.md
├── train_model.py
├── data/
│   ├── images/
│   └── labels.csv
├── models/
│   └── random_forest_model.joblib
└── results/
    └── model_comparison.png
```

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request
