# Comprehensive Data Cleaning, Categorical Encoding, and Feature Scaling

## 📌 Project Overview
This project serves as a comprehensive demonstration of core data science preprocessing techniques. It builds a robust preprocessing pipeline to handle common real-world data challenges, including missing values, unformatted categorical fields, and heavily skewed numerical distributions. 

The objective is to showcase an absolute mastery of data cleaning, exploratory analysis, and diverse feature transformation methodologies using Python, Scikit-Learn, and Seaborn.

---

## 🛠️ Preprocessing Methodologies Applied

### 1. Data Cleaning & Imputation
* **Missing Numerical Values:** Handled missing data in the `Age` feature by applying **Median Imputation** to prevent distortion from potential outliers.
* **Missing Categorical Values:** Handled missing data in the `Embarked` feature by using **Mode Imputation** (most frequent value).
* **Structural Safety:** Verified integrity to ensure no data leakage occurred during the cleaning phase.

### 2. Categorical Encoding (Concept & Implementation)
* **Label Encoding:** Applied to target variables (`Survived`) to convert classes into simple mathematical integers ($0$ and $1$).
* **Ordinal Encoding:** Applied to the `Ticket_Class` feature to explicitly preserve the inherent rank and order (`Low < Medium < High`).
* **One-Hot Encoding:** Applied to the nominal `Sex` feature to split values into binary features without implying an unearned mathematical hierarchy. Used `drop='first'` to prevent multicollinearity (the dummy variable trap).

### 3. Feature Scaling & Transformations
* **StandardScaler:** Applied to `Age` to recalculate metrics based on Z-scores (mean = 0, standard deviation = 1) for algorithms assuming normal distribution.
* **MinMaxScaler:** Applied to `Age` to bound features strictly within a 0 to 1 interval, making it ready for neural network integration.
* **RobustScaler:** Applied to the heavily skewed `Fare` column. By scaling via the median and Interquartile Range (IQR), it resists being distorted by extreme ticket outliers.
* **MaxAbsScaler:** Demonstrated on the matrix to scale values between -1 and 1 based on absolute maximums, preserving sparsity.
* **Log Transformation ($log(x+1)$):** Applied to `Fare` to minimize extreme right skewness, pulling the distributed tail back into a balanced bell curve.

---

### 📊 Visual Proof: Impact of Log Transformation
Below is the empirical proof showing how the heavily skewed `Fare` data is successfully normalized using `np.log1p` to make it algorithm-ready:

![Distribution Comparison](distribution_comparison.png)

---

## 📊 Summary Mapping Table


| Feature Name | Data Type | Identified Challenge | Applied Technique | Justification |
| :--- | :--- | :--- | :--- | :--- |
| **Sex** | Categorical | Nominal (No Order) | One-Hot Encoding | Avoids implying an incorrect mathematical ranking. |
| **Ticket_Class**| Categorical | Ordinal (Ordered) | Ordinal Encoding | Preserves the native `Low < Medium < High` rank. |
| **Age** | Numerical | Regular Linear Scale | MinMaxScaler / Standard | Perfectly normalizes bounds or converts to standard Z-scores. |
| **Fare** | Numerical | Extreme Outliers / Skew | RobustScaler / Log | Prevents extreme data anomalies from corrupting algorithm weights. |

---

## 🚀 How to Run This Project

1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com
   ```
2. Install the necessary data science libraries:
   ```bash
   pip install numpy pandas scikit-learn matplotlib seaborn
   ```
3. Open the Jupyter Notebook file and run all cells:
   ```bash
   jupyter notebook assignment.ipynb
   ```

---
*Submitted as part of the Data Science Foundation curriculum.*
