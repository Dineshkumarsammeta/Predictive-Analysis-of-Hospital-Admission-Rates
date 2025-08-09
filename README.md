# Predictive-Analysis-of-Hospital-Admission-Rates

# 🏥 Predictive Analysis of Hospital Admission Rates 

## 📌 Project Overview
This project predicts **hospital bed occupancy** using seasonal and historical patterns from NHS England’s **Urgent & Emergency Care (UEC) SitRep** datasets.  
The aim is to support **capacity planning** by identifying seasonal demand trends and forecasting future admission rates.

## 📂 Dataset
- **Source:** [NHS England – UEC SitRep](https://www.england.nhs.uk/statistics/statistical-work-areas/uec-sitrep/)
- **Data Year:** 2011 (Bed Occupancy & Admissions)
- **Format:** CSV
- **Frequency:** Daily/Weekly (depending on report)

## 🛠 Tech Stack
- **Language:** Python  
- **Libraries:** Pandas, Scikit-learn, Matplotlib, NumPy
- **Environment:** Jupyter Notebook / Python Script

## 🎯 Core Tasks
1. **Data Acquisition** – Download raw CSV(s) from NHS England website.
2. **Data Cleaning & Preprocessing**
   - Remove null values and duplicates
   - Standardise column names
   - Parse dates into proper datetime format
   - Convert text-based numbers to numeric
   - Handle missing values with interpolation or removal
3. **Time-Series Analysis**
   - Resample to a consistent frequency (daily, weekly, or monthly)
   - Identify seasonal patterns (e.g., winter peaks in admissions)
4. **Predictive Modelling**
   - Use historical data to train time-series models
   - Predict short-term hospital admission rates
5. **Visualisation**
   - Plot seasonal trends
   - Compare actual vs predicted values

## 📊 NHS Relevance
This project can be used to:
- Anticipate **seasonal peaks** in hospital admissions
- Plan **bed allocation and staffing**
- Improve **NHS resource management**

## 📦 Installation & Usage
```bash
# Clone the repository
git clone https://github.com/yourusername/nhs-hospital-admissions-predict.git
cd nhs-hospital-admissions-predict

# Install dependencies
pip install -r requirements.txt

# Run the cleaning script
python clean_nhs_data.py

# Open the analysis notebook
jupyter notebook analysis.ipynb
