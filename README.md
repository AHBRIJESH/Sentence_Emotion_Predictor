# Sentence Emotion Predictor

![Naive Bayes](https://img.shields.io/badge/Implementation-Nural%20Network%20-darkblue)

## Overview

The Sentence Emotion Predictor is a tool designed to analyze and predict the emotional tone of a given sentence. It employs natural language processing techniques to identify and classify the emotions expressed in text, providing valuable insights for applications such as sentiment analysis, customer feedback analysis, and emotion-aware chatbots.

## Features

- **Emotion Classification:** The predictor categorizes sentences into different emotions, such as joy, sadness, anger, fear, and more.
  
- **Multi-language Support:** The model supports multiple languages, allowing users to analyze text in various linguistic contexts.

- **High Accuracy:** Built on state-of-the-art natural language processing models, the predictor delivers accurate and reliable emotion predictions.

- **User-Friendly Interface:** The tool offers a simple and intuitive interface, making it easy for users to input sentences and receive emotion predictions.

## Getting Started

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/sentence-emotion-predictor.git
   cd sentence-emotion-predictor
   ```
# Project Contents

## Model.ipynb

The `model.ipynb` notebook contains the code for training and evaluating the Sentence Emotion Predictor model. It covers the entire process, from data preprocessing to model architecture design, training, and evaluation. The notebook provides insights into the choices made during the development of the model and includes comments to enhance understanding.

### Contents:
- **Data Loading:** The notebook includes code to load and preprocess the labeled dataset (`emotions.csv`) used for training the model.
- **Model Architecture:** Details about the architecture of the deep learning model, including layers, activation functions, and any specific configurations.
- **Training:** Code for training the model on the provided dataset, with information on hyperparameters and training procedures.
- **Evaluation:** Metrics and techniques used to evaluate the model's performance, ensuring it effectively predicts emotions in sentences.
- **Save Model:** Instructions on saving the trained model in the Hierarchical Data Format (HDF5) format (`model.h5`) for later use.

## Dependencies
- The notebook may rely on various libraries such as TensorFlow, Keras, or other machine learning and deep learning frameworks. Ensure that the necessary dependencies are installed before running the notebook.

## Emotions.csv

The `emotions.csv` file is a dataset used for training and evaluating the Sentence Emotion Predictor model. It contains labeled sentences with corresponding emotion labels. Each row in the CSV file represents a sentence and its associated emotion category.

### Data Columns:
1. **Content:** The textual content of the sentence.
2. **Emotion:** The labeled emotion category for the corresponding sentence.


## Model.h5

The `model.h5` file is the saved model in the Hierarchical Data Format (HDF5). This file contains the trained weights, architecture, and configuration of the Sentence Emotion Predictor model. The model can be loaded from this file for making predictions on new sentences without the need to retrain the model.

## Usage
```python
from tensorflow.keras.models import load_model

# Load the model
model = load_model('model.h5')

# Make predictions
sentence = "I can't believe we won!"
predictions = model.predict([sentence])
```

Ensure that you have the required dependencies installed to load and use the model.

**Note:** It's important to use the same version of libraries and dependencies when loading the model to avoid compatibility issues.
## Contributing

We welcome contributions to enhance and improve the Sentence Emotion Predictor. If you find any issues or have suggestions for new features, please open an issue or submit a pull request.

Happy predicting emotions! 🚀
