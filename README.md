# **Network Intrusion Detection Kaggle Competition Predictive Modeling and F1-Score Optimization**
Engaged in a [Kaggle competition](https://www.kaggle.com/competitions/elg7186-assignment-2-is-this-an-intrusion/overview) on network intrusion detection, I crafted a predictive model leveraging the provided training dataset. The task involved submitting CSV solutions (ID, Class) for the test set, with ID aligning with test data and Class presenting predicted labels. The competition's evaluation metric was the F1-score. Notably, this undertaking was a component of my 2023 master's program at the University of Ottawa, specializing in AI for Cyber Security.

- Required libraries: scikit-learn, pandas, matplotlib.
- Execute cells in a Jupyter Notebook environment.
- The uploaded code has been executed successfully within the [Google Colab](https://colab.google/) environment.

## Binary Classification Problem
Task is to classify the connection is intrusive (1) or not (0)

### Independent Variables:
  Include features such as duration, protocol type, service, flags, and numerical attributes related to net work activities. These variables provide a comprehensive representation of network behavior for intrusion detection.

### Target variable:
   +	'Class': classify the connection is intrusive (1) or not (0)

## **Key Tasks Undertaken**
1. **Data Loading and Exploration:**
   - Loaded and explored the train and test datasets.
   - Checked data information, null values, duplicates, and unique values.

2. **Data Cleaning:**
   - Handled missing values and duplicates.
   - Dropped unnecessary columns ("ID", "duration").

3. **Data Preprocessing:**
   - Separated features (X_train) and target variable (y_train).
   - Applied one-hot encoding to categorical variables.

4. **Model Training:**
   - Utilized CatBoostClassifier with hyperparameter tuning after applying differnet Classifiers.
   - Applied class weights for imbalanced classes.
   - Employed soft voting with a threshold for ensemble predictions.

5. **Model Evaluation and Prediction:**
   - Evaluated the model using the F1-score metric.
   - Generated predictions for the test data.

6. **Submission File Creation:**
   - Formatted the predictions into a CSV file with columns (ID, Class).
   - Saved the submission file as "Result of CatBoostClassifier model.csv".


![image](https://github.com/RimTouny/Network-Intrusion-Detection-Kaggle-Competition-Predictive-Modeling-and-F1-Score-Optimization/assets/48333870/6e9124a7-2e65-4c56-95c7-52c3f448641e)
