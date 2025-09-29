# Titanic EDA Analysis

## 📌 Project Overview
This project performs **Exploratory Data Analysis (EDA)** on the famous **Titanic dataset**.  
The goal is to extract insights about passenger demographics, survival patterns, and key relationships using **Python, Pandas, Matplotlib, and Seaborn**.

---

## 📂 Dataset
- File: `titanic-dataset.csv`
- Columns:
  - `PassengerId` – Unique passenger identifier
  - `Survived` – Survival (0 = No, 1 = Yes)
  - `Pclass` – Passenger class (1 = 1st, 2 = 2nd, 3 = 3rd)
  - `Name` – Passenger name
  - `Sex` – Gender
  - `Age` – Age in years
  - `SibSp` – Number of siblings/spouses aboard
  - `Parch` – Number of parents/children aboard
  - `Ticket` – Ticket number
  - `Fare` – Ticket fare
  - `Cabin` – Cabin number
  - `Embarked` – Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)

---

## ⚙️ Tools & Libraries
- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## 📊 EDA Steps
1. **Data Cleaning**
   - Handle missing values (`Age`, `Cabin`, `Embarked`)
   - Convert categorical columns to correct types
   - Create new feature: `FamilySize = SibSp + Parch + 1`

2. **Univariate Analysis**
   - Distribution of `Age`, `Fare`
   - Countplots of `Sex`, `Pclass`, `Embarked`

3. **Bivariate Analysis**
   - `Sex` vs `Survived`
   - `Pclass` vs `Survived`
   - `FamilySize` vs `Survived`

4. **Multivariate Analysis**
   - Correlation heatmap
   - Pairplots for numeric features

5. **Insights**
   - Women and children had higher survival rates
   - 1st-class passengers were more likely to survive
   - Large families had lower survival probability
   - Higher fare correlated with better survival chances

---

## 📑 Deliverables
- `titanic_eda_analysis.ipynb` – Jupyter Notebook with code and visualizations
- `report.pdf` – Summary report (optional export)
- `titanic-dataset.csv` – Dataset used for analysis

---

## 🚀 How to Run
```bash
# Clone repository
git clone https://github.com/<your-username>/titanic-eda-analysis.git
cd titanic-eda-analysis

# Install requirements
pip install -r requirements.txt

# Run Jupyter Notebook
jupyter notebook titanic_eda_analysis.ipynb
