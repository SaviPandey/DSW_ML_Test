# Loan Default Prediction Machine Learning Model

## Project Overview
This repository contains the solution to the loan default prediction problem provided by **Data Science Wizards (DSW)** as part of their campus hiring process. The project focuses on developing a classification model to predict loan repayment behavior, specifically identifying potential defaulters and non-defaulters. This helps enhance risk assessment and improve the loan approval process for a trusted Non-Banking Financial Company (NBFC).

## Problem Statement
The primary goal is to predict the loan default status of applicants using historical and validation data. The dataset includes financial and demographic features, such as CIBIL score, annual income, loan amount, and employment length.

## Data Description
Two datasets were provided:
1. **train_data.xlsx**: Historic data containing loan disbursement applications and their default/non-default status for the past 2+ years.
2. **test_data.xlsx**: Validation data containing loan disbursement applications and their default/non-default status for the past 3 months.

### Key Features
- **customer_id**: Unique identifier for each application.
- **sub_grade**: Classification of customers based on geography, income, and age.
- **term**: Total loan tenure.
- **cibil_score**: Credit score of the applicants.
- **loan_amnt**: Total loan amount.
- **loan_status**: Target variable (1: default, 0: non-default).

For a full list of columns, refer to the project documentation.

## Deliverables
The repository includes the following components:

### 1. Exploratory Data Analysis (EDA)
- **File**: `eda.ipynb`
- Visual and statistical insights into the data.
- Charts and descriptive analysis with markdown explanations.

### 2. Modelling
- **File**: `model.py`
- Two different models implemented using an object-oriented approach.
- Functions:
  - `load()`: To load data.
  - `preprocess()`: To perform data preprocessing.
  - `train()`: To train the models.
  - `test()`: To evaluate models and generate summaries.
  - `predict()`: To make inferences.

### 3. Model Selection
- **File**: `model_selection.ipynb`
- Comparison of models based on evaluation metrics.
- Includes hyperparameter tuning and justification for the final model choice.

### 4. Final Submission
- The repository is structured according to DSW's guidelines, ensuring pre-run notebooks with output cells.

## Tools and Technologies
- Python 3.7+
- Libraries: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn

## How to Run
1. Clone the repository:
   ```bash
   git clone <repo-url>
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Explore the data analysis:
   ```bash
   jupyter notebook eda.ipynb
   ```
4. Run the training script:
   ```bash
   python model.py
   ```
5. Review model selection:
   ```bash
   jupyter notebook model_selection.ipynb
   ```

## Results
- The final model chosen was Logistic Regression and Random Forest.
- Achieved an accuracy of **76%** and an F1 score of **77%** on the test dataset.
- Detailed evaluation metrics can be found in `model_selection.ipynb`.

## Author
- **SAVINAY PANDEY**

## License
This project is licensed under the [MIT License](LICENSE).
