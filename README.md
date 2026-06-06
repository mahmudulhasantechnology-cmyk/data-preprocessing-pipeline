<h1 align="center">🧹 Comprehensive Data Preprocessing Pipeline</h1>
<h3 align="center">Mastering Data Cleaning, Encoding & Feature Scaling with Python</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Language-Python-blue?style=for-the-badge&logo=python">
  <img src="https://img.shields.io/badge/Library-Scikit--Learn-orange?style=for-the-badge&logo=scikit-learn">
  <img src="https://img.shields.io/badge/Skill-Data%20Preprocessing-green?style=for-the-badge">
  <img src="https://img.shields.io/badge/Visualization-Seaborn-lightblue?style=for-the-badge">
</p>

<hr>

<h2>🖼️ Project Preview</h2>
<p align="center">
  <img src="https://github.com/mahmudulhasantechnology-cmyk/data-preprocessing-pipeline/blob/Sub-branch/data-preprocessing-pipeline.jpg" alt="Data Preprocessing Pipeline Preview" width="900">
</p>

<hr>

<h2>📌 Overview</h2>
<p>
This project serves as a comprehensive demonstration of core <b>data science preprocessing techniques</b>.<br>
It builds a robust preprocessing pipeline to handle common real-world data challenges, including <b>missing values</b>, <b>unformatted categorical fields</b>, and <b>heavily skewed numerical distributions</b>.
</p>
<p>
🎯 <b>Goal:</b> Showcase an absolute mastery of data cleaning, exploratory analysis, and diverse feature transformation methodologies using <b>Python</b>, <b>Scikit-Learn</b>, and <b>Seaborn</b>.
</p>

<hr>

<h2>🎯 Objectives</h2>
<ul>
  <li>✔ Handle missing values through robust imputation strategies</li>
  <li>✔ Apply and compare multiple categorical encoding techniques</li>
  <li>✔ Demonstrate diverse feature scaling and transformation methods</li>
  <li>✔ Prevent data leakage and ensure structural integrity</li>
  <li>✔ Build a reusable, production-ready preprocessing pipeline</li>
</ul>

<hr>

<h2>🛠️ Tools & Techniques</h2>
<ul>
  <li><b>Python</b></li>
  <li><b>Data Cleaning</b> (missing values, imputation strategies)</li>
  <li><b>Categorical Encoding</b> (Label, Ordinal, One-Hot)</li>
  <li><b>Feature Scaling</b> (StandardScaler, MinMaxScaler, RobustScaler, MaxAbsScaler)</li>
  <li><b>Feature Transformation</b> (Log Transformation)</li>
  <li><b>Scikit-Learn Pipelines</b></li>
  <li><b>Seaborn & Matplotlib</b> for distribution visualization</li>
</ul>

<hr>

<h2>🔍 Preprocessing Methodologies</h2>

<h3>1. 🧼 Data Cleaning & Imputation</h3>
<ul>
  <li><b>Median Imputation</b> — Applied to the <code>Age</code> feature to handle missing numerical values without distortion from outliers</li>
  <li><b>Mode Imputation</b> — Applied to the <code>Embarked</code> feature to fill missing categorical values with the most frequent entry</li>
  <li><b>Leakage Prevention</b> — Verified structural integrity to ensure no data leakage occurred during the cleaning phase</li>
</ul>

<h3>2. 🏷️ Categorical Encoding</h3>
<ul>
  <li><b>Label Encoding</b> — Applied to <code>Survived</code> (target variable) to convert classes into integers (0 and 1)</li>
  <li><b>Ordinal Encoding</b> — Applied to <code>Ticket_Class</code> to preserve inherent rank order (<code>Low &lt; Medium &lt; High</code>)</li>
  <li><b>One-Hot Encoding</b> — Applied to nominal <code>Sex</code> feature; used <code>drop='first'</code> to prevent multicollinearity (dummy variable trap)</li>
</ul>

<h3>3. ⚖️ Feature Scaling & Transformations
