<h1 align="center">🧹 Data Preprocessing & Feature Engineering Pipeline</h1>
<h3 align="center">Comprehensive Data Cleaning, Categorical Encoding, and Feature Scaling</h3>

<p align="center">
  <img src="https://shields.io">
  <img src="https://shields.io">
  <img src="https://shields.io">
</p>

<hr>

<h2>📌 Overview</h2>
<p>
This project serves as a comprehensive demonstration of core data science preprocessing techniques. It builds a robust preprocessing pipeline to handle common real-world data challenges, including missing values, unformatted categorical fields, and heavily skewed numerical distributions.
</p>

<p>
🎯 <b>Goal:</b> Showcase mastery of data cleaning, exploratory analysis, and diverse feature transformation methodologies using Python, Scikit-Learn, and Seaborn.
</p>

<hr>

<h2>🎯 Objectives</h2>
<ul>
  <li>✔ Build an end-to-end robust data preprocessing pipeline</li>
  <li>✔ Resolve missing values safely without data leakage</li>
  <li>✔ Implement diverse encoding techniques based on mathematical hierarchy</li>
  <li>✔ Handle extreme outliers and skewed features effectively</li>
  <li>✔ Prepare raw datasets for seamless machine learning integration</li>
</ul>

<hr>

<h2>🛠️ Preprocessing Methodologies Applied</h2>

<h3>1. Data Cleaning & Imputation</h3>
<ul>
  <li><b>Missing Numerical Values:</b> Handled missing data in the <code>Age</code> feature by applying <b>Median Imputation</b> to prevent distortion from potential outliers.</li>
  <li><b>Missing Categorical Values:</b> Handled missing data in the <code>Embarked</code> feature by using <b>Mode Imputation</b> (most frequent value).</li>
  <li><b>Structural Safety:</b> Verified integrity to ensure no data leakage occurred during the cleaning phase.</li>
</ul>

<h3>2. Categorical Encoding</h3>
<ul>
  <li><b>Label Encoding:</b> Applied to target variables (<code>Survived</code>) to convert classes into simple mathematical integers (0 and 1).</li>
  <li><b>Ordinal Encoding:</b> Applied to the <code>Ticket_Class</code> feature to explicitly preserve the inherent rank and order (Low &lt; Medium &lt; High).</li>
  <li><b>One-Hot Encoding:</b> Applied to the nominal <code>Sex</code> feature to split values into binary features without implying an unearned mathematical hierarchy. Used <code>drop='first'</code> to prevent multicollinearity (the dummy variable trap).</li>
</ul>

<h3>3. Feature Scaling & Transformations</h3>
<ul>
  <li><b>StandardScaler:</b> Applied to <code>Age</code> to recalculate metrics based on Z-scores (mean = 0, standard deviation = 1) for algorithms assuming normal distribution.</li>
  <li><b>MinMaxScaler:</b> Applied to <code>Age</code> to bound features strictly within a 0 to 1 interval, making it ready for neural network integration.</li>
  <li><b>RobustScaler:</b> Applied to the heavily skewed <code>Fare</code> column. By scaling via the median and Interquartile Range (IQR), it resists being distorted by extreme ticket outliers.</li>
  <li><b>MaxAbsScaler:</b> Demonstrated on the matrix to scale values between -1 and 1 based on absolute maximums, preserving sparsity.</li>
  <li><b>Log Transformation (log(x+1)):</b> Applied to <code>Fare</code> to minimize extreme right skewness, pulling the distributed tail back into a balanced bell curve.</li>
</ul>
  <li>✔ Build an end-to-end robust data preprocessing pipeline</li>
  <li>✔ Resolve missing values safely without data leakage</li>
  <li>✔ Implement diverse encoding techniques based on mathematical hierarchy</li>
  <li>✔ Handle extreme outliers and skewed features effectively</li>
  <li>✔ Prepare raw datasets for seamless machine learning integration</li>
</ul>

<hr>

<h2>🛠️ Preprocessing Methodologies Applied</h2>

<h3>1. Data Cleaning & Imputation</h3>
<ul>
  <li><b>Missing Numerical Values:</b> Handled missing data in the <code>Age</code> feature by applying <b>Median Imputation</b> to prevent distortion from potential outliers.</li>
  <li><b>Missing Categorical Values:</b> Handled missing data in the <code>Embarked</code> feature by using <b>Mode Imputation</b> (most frequent value).</li>
  <li><b>Structural Safety:</b> Verified integrity to ensure no data leakage occurred during the cleaning phase.</li>
</ul>

<h3>2. Categorical Encoding</h3>
<ul>
  <li><b>Label Encoding:</b> Applied to target variables (<code>Survived</code>) to convert classes into simple mathematical integers (0 and 1).</li>
  <li><b>Ordinal Encoding:</b> Applied to the <code>Ticket_Class</code> feature to explicitly preserve the inherent rank and order (Low &lt; Medium &lt; High).</li>
  <li><b>One-Hot Encoding:</b> Applied to the nominal <code>Sex</code> feature to split values into binary features without implying an unearned mathematical hierarchy. Used <code>drop='first'</code> to prevent multicollinearity (the dummy variable trap).</li>
</ul>

<h3>3. Feature Scaling & Transformations</h3>
<ul>
  <li><b>StandardScaler:</b> Applied to <code>Age</code> to recalculate metrics based on Z-scores (mean = 0, standard deviation = 1) for algorithms assuming normal distribution.</li>
  <li><b>MinMaxScaler:</b> Applied to <code>Age</code> to bound features strictly within a 0 to 1 interval, making it ready for neural network integration.</li>
  <li><b>RobustScaler:</b> Applied to the heavily skewed <code>Fare</code> column. By scaling via the median and Interquartile Range (IQR), it resists being distorted by extreme ticket outliers.</li>
  <li><b>MaxAbsScaler:</b> Demonstrated on the matrix to scale values between -1 and 1 based on absolute maximums, preserving sparsity.</li>
  <li><b>Log Transformation (log(x+1)):</b> Applied to <code>Fare</code> to minimize extreme right skewness, pulling the distributed tail back into a balanced bell curve.</li>
</ul>

---

### 📊 Visual Proof: Impact of Log Transformation
<img src="https://github.com/mahmudulhasantechnology-cmyk/data-preprocessing-pipeline/blob/main/data-preprocessing-pipeline.pdf" width="80%">
Below is the empirical proof showing how the heavily skewed `Fare` data is successfully normalized using `np.log1p` to make it algorithm-ready. 

<div style="text-align: center; margin: 25px 0;">
  <!-- Render the visual graph image -->
  <img src="https://github.com/mahmudulhasantechnology-cmyk/data-preprocessing-pipeline/blob/main/data-preprocessing-pipeline.pdf" width="80%">
  
  <p style="font-style: italic; color: #555; margin-top: 12px; font-size: 14px;">
    Figure 1: Side-by-side empirical distribution comparison before and after Log Transformation.
  </p>

  <!-- Clean, styled call-to-action button linking directly to your verification PDF report -->
  <div style="margin-top: 20px;">
    <a href="https://github.com/mahmudulhasantechnology-cmyk/data-preprocessing-pipeline/blob/main/data-preprocessing-pipeline.pdf" 
       target="_blank" 
       style="background-color: #0366d6; color: white; padding: 10px 20px; text-decoration: none; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif; font-size: 14px; font-weight: bold; border-radius: 6px; display: inline-block; box-shadow: 0 2px 5px rgba(0,0,0,0.1);">
    </a>
  </div>
</div>

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

