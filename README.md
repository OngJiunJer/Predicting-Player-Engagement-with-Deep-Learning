# Predicting-Player-Engagement-with-Deep-Learning
 Developed a deep learning model using Convolutional Neural Network (CNN) and Gated  Recurrent Unit (GRU) to classify player engagement levels based on online gaming behavior.  Achieved 90% prediction accuracy after evaluating multiple model architectures.

## Step 1: Data Understanding
  - Loaded and inspected the dataset.
  - Visualized both numerical and categorical feature distributions.
  - Checked for missing values, duplicate records, and outliers.

## Step 2: Data Preprocessing
  - Dropped irrelevant columns (e.g., player IDs or unrelated identifiers).
  - Encoded categorical features using one-hot encoding.
  - Normalized numerical features using standard scaling.
  - Balanced the dataset using random undersampling to handle class imbalance.
  - Converted the target variable (EngagementLevel) into a categorical format.
  - Split the dataset into training and test sets (typically 80/20).

## Step 3: Model Building
  - Build a CNN Model using Conv1D and Dense layers.
  - Build a GRU Model using GRU and Dense layers.

## Step 4: Hyperparameter Tuning
  - Used Keras Tuner with RandomSearch to find the best hyperparameters
  - Applied tuning on both CNN and GRU models for performance improvement
  - CNN Tuned the following hyperparameters:
    1) Filter size (e.g., 32 to 128) for Conv1D layer
    2) Kernel size (3 or 5) for Conv1D layer
    3) Number of units in multiple dense layers (64–256)
    4) Dropout rate in dense layers (0.2–0.5) to prevent overfitting
    5) Learning rate values: 1e-2, 1e-3, 5e-4, 1e-4
    6) Optimizer: either Adam or SGD
  - GRU Tuned the following hyperparameters:
    1) GRU units (e.g., 50–150)
    2) Dense layer units (64–256)
    3) Dropout rate in dense layers (0.2–0.5)
    4) Learning rate values: 1e-2, 1e-3, 5e-4, 1e-4
    5) Optimizer: Adam or SGD

## Step5: Evaluation
  - In this step will apply evaluation methods such as learning curve, classification report, and confusion matrix.
    1) CNN Model (First Version Without Applying Hyperparameter Tuning)
    2) CNN Model (Optimized Version With Applying Hyperparameter Tuning)
    3) GRU Model (First Version Without Applying Hyperparameter Tuning)
    4) GRU Model (Optimized Version With Applying Hyperparameter Tuning)
