# Titanic-Survival

This project focuses on predicting passenger survival on the Titanic using machine learning techniques. The dataset includes features like gender, age, and passenger class, which are preprocessed by converting categorical variables into numerical values, handling missing data, and scaling the features. A Logistic Regression model is used to predict survival, and its performance is evaluated using accuracy scores on both training and test datasets. The model is further analyzed by inspecting the feature coefficients and making predictions for sample passengers.

### Requirements:
- Python 3.x
- Jupyter Notebook
- Libraries: pandas, numpy, scikit-learn, matplotlib

### **Features**

#### **Data Cleaning:**
- **Data Loading**: Loads passenger data from a CSV file hosted on Google Drive for analysis.
- **Column Transformation**: Converts the `Sex` column to numerical values (`1` for female, `0` for male) using a mapping.
- **Missing Value Handling**: Fills missing values in the `Age` column with the mean age to ensure no missing data.
- **Feature Creation**:
  - Creates a binary feature `FirstClass` to indicate whether a passenger was in the first class.
  - Creates a binary feature `SecondClass` to indicate whether a passenger was in the second class.

#### **Machine Learning Algorithms:**
- **Logistic Regression**: 
  - **Model Creation and Training**: A logistic regression model is created and trained using the features `Sex_num`, `Age`, `FirstClass`, and `SecondClass` to predict the binary survival outcome (`Survived`).
  - **Model Evaluation**: Evaluates the model's performance on both the training and test datasets using the `.score()` method, which returns the accuracy of the model.

#### **Feature Scaling:**
- **StandardScaler**: 
  - Scales the feature data (`X_train` and `X_test`) to have a mean of 0 and a standard deviation of 1, ensuring that the features are on the same scale and helping improve model performance.
  - Also scales the sample passenger data before making predictions.

#### **Model Evaluation:**
- **Model Scoring**: 
  - After training the logistic regression model, the `.score()` method is used to evaluate the accuracy of the model on both the training and test sets.
- **Coefficient Analysis**: The model’s **coefficients** are printed, which show the importance of each feature in the model.
- **Prediction**: Predicts survival (`Survived`), as well as the probability of survival, for sample passengers (Jack, Rose, and You) using the trained logistic regression model.

- ### Project Screenshot
![Alt text](https://github.com/brianwpiano/Titanic-Survival/blob/main/Screenshot%202024-11-15%20150329.png)
![Alt text](https://github.com/brianwpiano/Titanic-Survival/blob/main/Screenshot%202024-11-15%20150402.png)
![Alt text](https://github.com/brianwpiano/Titanic-Survival/blob/main/Screenshot%202024-11-15%20150418.png)

## Run the app

Clone this repo then `cd Titanic-Survival`.

Assuming you have Python3 installed on a Windows 10 or 11 or on MacOS, run this commands:

``` bash
Titanic Survival.ipynb
```

---
