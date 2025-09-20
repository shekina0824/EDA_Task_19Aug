# EDA_Task_19Aug
## 📘 Objective
Beginner-level EDA using pandas: load dataset, check shape, column names, and
preview rows.
## 📂 Dataset
Retail Sales Dataset (Sample Sales Data)
Source: [Kaggle Link](https://www.kaggle.com/datasets/kyanyoga/sample-salesdata)





## 🧹 Handle Missing Data
We identified missing values using `df.isna().sum()`. Based on the extent, we used appropriate strategies like dropping rows or imputing with mean/forward fill. Cleaned data is saved as `cleaned_data.csv`.



## 🔄 Day 4 – Fix Data Types & Remove Duplicates

- Converted date columns to datetime format using `pd.to_datetime()`
- Ensured numeric columns are in correct type using `pd.to_numeric()`
- Removed duplicate records using `drop_duplicates()`
- Saved updated dataset as `data/cleaned_data_v2.csv`



## 📊 Day 5 – Data Normalization & Scaling
- Identified numerical columns in the dataset.
- Applied `MinMaxScaler` to normalize values between 0 and 1.
- Saved the preprocessed dataset as `data/preprocessed_data.csv`.
- All steps are documented in `preprocessing.ipynb`.



## 📤 Day 6 – Export Data for Power BI
- Loaded preprocessed dataset from Day 5.
- Verified data integrity and structure.
- Exported final dataset as `data/final_data_for_powerbi.csv` for visualization in Power BI.
✅


## 🧾 Data Preprocessing Summary (Day 8)

Below are the steps performed during the preprocessing pipeline:

1. **Handled Missing Values (Day 3):**
   - Used `isna().sum()` to identify missing values.
   - Imputed missing numerical columns with mean.
   - Filled missing categorical values with `'Unknown'`.

2. **Fixed Data Types & Removed Duplicates (Day 4):**
   - Converted date columns using `pd.to_datetime()`.
   - Converted object columns to numeric types using `pd.to_numeric()`.
   - Removed duplicate rows using `drop_duplicates()`.

3. **Applied Feature Scaling (Day 5):**
   - Applied `MinMaxScaler` from scikit-learn to normalize numeric features.
   - Saved results as `preprocessed_data.csv`.

4. **Exported Clean Data for Power BI (Day 6):**
   - Verified final structure of data.
   - Exported dataset for visualization as `final_data_for_powerbi.csv`.

5. **Planned Visualizations (Day 7):**
   - Identified key KPIs and suitable chart types.
   - Documented layout in `visualization_plan.md`.

➡ These steps ensure the dataset is clean, standardized, and ready for visualization and modeling.


## 🧩 Day 9 – Power BI Data Connection
- Loaded dataset `final_data_for_powerbi.csv` into Power BI.
- Verified the data model and field types.
- Saved the Power BI file as `data_model.pbix` for visualization in Day 10.


## 🔗 Day 10 – Power BI Data Modeling
- Imported related tables: Customers, Products, Dates.
- Created relationships between tables using keys.
- Ensured a clean star schema design.
- Saved the updated model in `data_model.pbix`.

## 📊 Day 11 – Power BI Dashboard
- Designed interactive dashboard using visuals:
- Bar, Line, and Pie Charts
- KPI Cards for key metrics
- Slicers for dynamic filtering
- Dashboard saved as `dashboard.pbix`
- 

## 🌐 Day 12 – Publish Power BI Dashboard
- Dashboard published to Power BI Cloud.
- Live Web Link: [View Dashboard](https://app.powerbi.com/view?r=your_public_link_here)


## 📌 Day 13 – Real-Time Problem Selection

### 🔍 Problem Statement

**Title:** Real-Time Healthcare Monitoring (COVID-19 Trends)

**Objective:** To track and analyze COVID-19 cases and vaccination uptake in real-time, enabling quick response to rising trends.

**Domain:** Healthcare

**Dataset Source:** Kaggle COVID-19 Dataset / Government Health Data (to be finalized)

**Expected Outcome:** Real-time dashboard that shows cases, recoveries, deaths, and vaccination updates with trend alerts.

### 📊 Possible KPIs

- Daily new cases (per 100k population)
- Vaccination uptake (%) in real time
- Hospital occupancy rate (%)
- Latency of data update (minutes)

