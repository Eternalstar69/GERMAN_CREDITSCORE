# German Credit Risk Classification Using Machine Learning

## Project Description

This project applies machine learning techniques to classify credit risk using the **German Credit Dataset**. The dataset contains various financial and personal attributes of individuals applying for credit. 

The goal is to **predict whether a customer is a good or bad credit risk** based on their financial history, employment status, and other factors.

## Dataset Information

- **Dataset Name:** German Credit Dataset  
- **File Location:** `dataset/german.data`  
- **File Format:** Space-separated (`sep="\s+"`)  
- **Number of Samples:** 1000  
- **Number of Features:** 20  
- **Target Variable:** `target` (1 = Good Credit, 2 = Bad Credit)  

### **Key Columns in the Dataset**
| Column Name | Description |
|-------------|------------|
| `duration` | Credit duration in months |
| `credit_amount` | Loan amount requested |
| `age` | Age of applicant |
| `num_of_existing_credits` | Number of existing credits for the applicant |
| `housing` | Housing status (Own, Rent, Free) |
| `job` | Job category |
| `saving_account_balance` | Savings account balance |
| `target` | 1 = Good Credit, 2 = Bad Credit |

---

## Installation & Setup

To run this project, install the required dependencies:

pip install numpy pandas matplotlib scikit-learn


### **README.md**  

```md
# German Credit Risk Classification Using Machine Learning

## Project Description

This project applies machine learning techniques to classify credit risk using the **German Credit Dataset**. The dataset contains various financial and personal attributes of individuals applying for credit. 

The goal is to **predict whether a customer is a good or bad credit risk** based on their financial history, employment status, and other factors.

## Dataset Information

- **Dataset Name:** German Credit Dataset  
- **File Location:** `dataset/german.data`  
- **File Format:** Space-separated (`sep="\s+"`)  
- **Number of Samples:** 1000  
- **Number of Features:** 20  
- **Target Variable:** `target` (1 = Good Credit, 2 = Bad Credit)  

### **Key Columns in the Dataset**
| Column Name | Description |
|-------------|------------|
| `duration` | Credit duration in months |
| `credit_amount` | Loan amount requested |
| `age` | Age of applicant |
| `num_of_existing_credits` | Number of existing credits for the applicant |
| `housing` | Housing status (Own, Rent, Free) |
| `job` | Job category |
| `saving_account_balance` | Savings account balance |
| `target` | 1 = Good Credit, 2 = Bad Credit |

---

## Installation & Setup

To run this project, install the required dependencies:

pip install numpy pandas matplotlib scikit-learn

Make sure you have the dataset in the `dataset/` directory before running the script.


## How to Run the Code

1. Clone the repository:
   git clone https://github.com/Eternalstar69/GERMAN_CREDITSCORE.git
   cd GERMAN_CREDITSCORE

2. Ensure the dataset file `german.data` is placed inside the `dataset/` folder.

3. Run the Python script:
   python script_name.py


The script will:
- Load and preprocess the dataset
- Handle missing values and outliers
- Perform one-hot encoding for categorical variables
- Apply feature selection
- Train and evaluate two models: **Logistic Regression** and **Support Vector Machine (SVM)**


## Data Preprocessing Steps

- **Outlier Detection & Removal**: Using the IQR method to filter extreme values.  
- **Feature Scaling**: Applying logarithmic transformation to numerical features.  
- **Categorical Encoding**: One-hot encoding for categorical variables.  
- **Feature Selection**: Using `SelectKBest` with **F-regression** to pick the 15 most important features.  

---

## Machine Learning Models

Two classification models were trained and tested:

1. **Logistic Regression**
   - Solver: `lbfgs`
   - Max iterations: `1000`
   
2. **Support Vector Machine (SVM)**
   - Kernel: `linear`
   - Tolerance: `0.01`

---

## Model Performance

Each model was evaluated using four metrics:

| Metric        | Logistic Regression | SVM |
|--------------|--------------------|-----|
| **Accuracy** | xx.xx%             | xx.xx% |
| **Precision** | xx.xx%            | xx.xx% |
| **Recall**   | xx.xx%             | xx.xx% |
| **F1-score** | xx.xx%             | xx.xx% |

**Note:** Replace "xx.xx%" with actual values after running the script.

---

## Results & Key Findings

- **Feature selection helped improve model performance** by reducing irrelevant data.  
- **Logistic Regression performed better/worse** than SVM in terms of accuracy and recall.  
- **Outliers and categorical encoding had a significant impact** on the results.  

---

## Author & Credits

- **Author:** Your Name  
- **GitHub:** [Your Profile](https://github.com/your-username)  
- **References:**  
  - German Credit Dataset: [UCI Repository](https://archive.ics.uci.edu/ml/datasets/statlog+(german+credit+data))  
  - Scikit-Learn Documentation: [scikit-learn.org](https://scikit-learn.org/)  

---

## Future Improvements

- Experiment with different feature selection techniques.  
- Tune hyperparameters for better model performance.  
- Implement more advanced models like Random Forest or XGBoost.  

---
