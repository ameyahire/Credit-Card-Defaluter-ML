<h1>Credit Card Defaulter Prediction & Power BI Dashboard</h1>

<h2>📌 Project Overview</h2>

This project aims to predict credit card defaulters using Logistic Regression and visualize insights through a Power BI dashboard. The dataset contains customer details, including demographics, credit limits, bill amounts, and past payment history.

<h2>🛠 Tech Stack</h2>

Machine Learning: Python (Logistic Regression)

Data Processing: Pandas, NumPy, Scikit-Learn

Visualization & Reporting: Power BI

<h2>📊 Dataset Description</h2>

The dataset includes:

Demographic Features: SEX, AGE, EDUCATION, MARRIAGE, STATE

Financial Features: LIMIT_BAL, BILL_AMT1-6, PAY_AMT1-6

Repayment History: PAY_0, PAY_2, ..., PAY_6

Target Variable: DEFAULT_PAYMENT (1 = Defaulter, 0 = Non-Defaulter)

<h2>🏗 Model Training (Logistic Regression)</h2>

Data Preprocessing

Encoded categorical variables (SEX, EDUCATION, MARRIAGE, STATE)

Handled missing values & outliers

Scaled numerical features using StandardScaler

Model Training

Split data into train (70%) and test (30%)

Trained Logistic Regression with class_weight='balanced'

Evaluated using accuracy, precision, recall, and F1-score

<h2>📈 Model Performance</h2>

Initial Model Results:

Accuracy: 80%

Class 1 (Defaulter) Recall: 21% (Low, meaning many defaulters were missed)

After Class Weight Balancing:

Accuracy: 70%

Class 1 Recall: 63% ✅ (Much better at detecting defaulters)

<h2>🚀 Next Steps</h2>

Optimize threshold (e.g., 0.3 instead of 0.5) to improve recall

Try SMOTE for better class balance

Use XGBoost for more robust results

<h2>📊 Power BI Dashboard</h2>

A Power BI dashboard was created to analyze defaulters based on various features.

Key Insights

Defaulter by Education & Sex - Most defaulters are high school graduates.

Defaulter by Age & Sex - Peak defaulting age is 20-40 years.

Defaulter by State & Sex - Some states have higher default rates.

Defaulter Ratio - 22% of customers defaulted.

Average Billing Amount - $45K

Average Payment Amount - $5.28K

<h2>Acknowledgments</h2>

Dataset source: [(https://github.com/vaishnavi-jaishwal/Credit-Card-Defaults-Analysis-Dashboard-Power-BI?form=MG0AV3)]

Power BI visualizations inspired by best practices in data analytics.
