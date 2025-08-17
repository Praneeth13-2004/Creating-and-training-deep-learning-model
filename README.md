🩺 Diabetes Prediction Using Neural Networks

📌 Problem Statement

Diabetes is a chronic health condition that affects how the body processes blood sugar (glucose). Early prediction and diagnosis of diabetes can help in timely treatment and better healthcare management. Traditional diagnostic methods require medical expertise and lab testing, which may not always be accessible.

This project aims to predict whether a patient has diabetes or not based on medical attributes using a neural network classifier. The dataset used is the Pima Indians Diabetes Dataset, a well-known dataset for binary classification problems in healthcare.

Output 0 → No Diabetes

Output 1 → Diabetes

💡 Concept

We use a feedforward neural network (Multi-Layer Perceptron) built with TensorFlow/Keras to perform binary classification.

🔹 Steps Involved:

Dataset Preparation

Load the dataset (CSV format) using NumPy.

Extract features (X) → 8 medical predictor variables.

Extract labels (y) → Binary values (0/1).

Neural Network Architecture

Input Layer: 8 neurons (for 8 medical features).

Hidden Layers:

Dense layer with 12 neurons (ReLU activation).

Dense layer with 8 neurons (ReLU activation).

Output Layer: 1 neuron (Sigmoid activation → outputs probability between 0 and 1).

Model Compilation

Loss Function: Binary Crossentropy.

Optimizer: Adam.

Metric: Accuracy.

Model Training

Trained for 150 epochs with a batch size of 10.

Learns to minimize loss by adjusting weights.

Evaluation & Prediction

Evaluated using accuracy on the dataset.

Predictions are made using a 0.5 threshold:

> 0.5 → 1 (Diabetes)

≤ 0.5 → 0 (No Diabetes)

📊 Results

The trained model achieves a decent level of accuracy on the dataset.

Predictions are compared with actual outcomes for the first 50 test cases.

⚠️ Disclaimer: This project is for educational purposes only. It should not be used as a substitute for professional medical advice or diagnosis.


📝 References

Pima Indians Diabetes Dataset: https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database?resource=download

TensorFlow/Keras Documentation
