# 🧑‍💼 Employee Turnover Prediction

A machine learning project that predicts employee turnover using **Logistic Regression** with Lasso (L1) and Ridge (L2) regularization techniques.

---

## 📌 Problem Statement

Employee turnover is costly for organizations. This project builds a classification model to predict whether an employee is likely to leave the company based on various HR-related features.

---

## 📂 Dataset

**File:** `employee_turnover.csv`

**Features (16 columns):**

| Feature | Description |
|---|---|
| `Job_Satisfaction` | Employee job satisfaction score |
| `Performance_Rating` | Performance rating |
| `Years_At_Company` | Number of years at the company |
| `Work_Life_Balance` | Work-life balance score |
| `Distance_From_Home` | Distance from home to workplace |
| `Monthly_Income` | Monthly income |
| `Education_Level` | Level of education |
| `Age` | Employee age |
| `Num_Companies_Worked` | Number of companies worked previously |
| `Employee_Role` | Role of the employee |
| `Annual_Bonus` | Annual bonus amount |
| `Training_Hours` | Training hours completed |
| `Department` | Department of the employee |
| `Annual_Bonus_Squared` | Engineered feature |
| `Annual_Bonus_Training_Hours_Interaction` | Engineered interaction feature |
| `Employee_Turnover` | **Target variable** (0 = Stayed, 1 = Left) |

---

## 🛠️ Tech Stack

- **Python 3**
- **Pandas** – Data loading and preprocessing
- **NumPy** – Numerical operations
- **Seaborn** – Data visualization
- **Scikit-learn** – Machine learning models and evaluation

---

## 🔬 Methodology

1. **Data Loading & Null Check** – Verified no missing values
2. **Feature/Target Split** – Separated features (`X`) from target (`y`)
3. **Train-Test Split** – 80/20 split with `random_state=42`
4. **Model Training** – Three models compared:
   - Baseline Logistic Regression
   - Logistic Regression with **Lasso (L1)** regularization (`C=0.5`)
   - Logistic Regression with **Ridge (L2)** regularization (`C=0.5`)
5. **Model Evaluation** – Accuracy score and full classification report for each model

---

## 📊 Models Compared

| Model | Regularization | Solver |
|---|---|---|
| Baseline Logistic Regression | None | Default (lbfgs) |
| Lasso Regression | L1 | liblinear |
| Ridge Regression | L2 | lbfgs |

---

## 🚀 How to Run

1. **Clone the repository:**
   ```bash
   git clone https://github.com/ronakrajput8882/employee-turnover-prediction.git
   cd employee-turnover-prediction
   ```

2. **Install dependencies:**
   ```bash
   pip install pandas numpy seaborn scikit-learn jupyter
   ```

3. **Launch the notebook:**
   ```bash
   jupyter notebook Employee_Turnover.ipynb
   ```

---

## 📁 Project Structure

```
employee-turnover-prediction/
│
├── employee_turnover.csv        # Dataset
├── Employee_Turnover.ipynb      # Main Jupyter Notebook
└── README.md                    # Project documentation
```

---

## 🙋 Author

**Ronaksinh Rajput**  
[LinkedIn](https://linkedin.com/in/ronaksinh-rajput8882) | [GitHub](https://github.com/ronakrajput8882)
