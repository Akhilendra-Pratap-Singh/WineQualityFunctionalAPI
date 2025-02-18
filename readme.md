# Wine Quality Prediction Using Multi-Task Learning

This project involves predicting the quality and type of wine using machine learning techniques. We approach this problem by using a multi-output neural network model built with TensorFlow and Keras, which predicts two outcomes: the wine type (classification) and the wine quality (regression).

---

### Project Overview

- **Objective**: The goal of this project is to build a multi-task model to predict both the type and quality of wines based on various features such as acidity, alcohol content, etc.
- **Dataset**: The project uses the **Wine Quality Dataset** from the UCI Machine Learning Repository, which includes various physicochemical properties of red and white wines, with the aim to predict:
  - **Wine Type**: Red or White (classification problem).
  - **Wine Quality**: A score between 0 and 10 (regression problem).

---

### Technologies Used

- **Programming Language**: Python
- **Libraries**:
  - TensorFlow / Keras
  - Pandas
  - Numpy
  - Scikit-learn
- **Model**:
  - Multi-task neural network using the **Keras Functional API**.
  - **Binary Crossentropy** for classification (wine type).
  - **Mean Squared Error (MSE)** and **Root Mean Squared Error (RMSE)** for regression (wine quality).


### Key Features

- **Multi-Output Model**: Predicts both wine type (classification) and wine quality (regression) in one model.
- **Keras Functional API**: Leveraged for custom architecture to handle multiple outputs.
- **Data Preprocessing**:
  - Split dataset into training, validation, and test sets.
  - Scaled data using standardization to improve model performance.
- **Model Evaluation**:
  - Classification accuracy for wine type prediction.
  - RMSE for evaluating the wine quality prediction.

---

### Model Architecture

- **Input Layer**: Takes in 11 features from the wine dataset.
- **Hidden Layers**: Two dense layers with ReLU activation for feature learning.
- **Output Layers**:
  - **Wine Type**: Single unit, sigmoid activation (binary classification).
  - **Wine Quality**: Single unit, linear activation (regression).

---

Results
Wine Type Prediction (Classification)
Accuracy on Training Set: 99.56%
Loss on Training Set: 0.0331
Accuracy on Validation Set: 99.23%
Loss on Validation Set: 0.0270
Accuracy on Test Set: 99.49%
Loss on Test Set: 0.0179
Wine Quality Prediction (Regression)
MSE on Training Set: 0.3965
RMSE on Training Set: 0.6296
MSE on Validation Set: 0.5283
RMSE on Validation Set: 0.7295
MSE on Test Set: 0.5360
RMSE on Test Set:0.7320


