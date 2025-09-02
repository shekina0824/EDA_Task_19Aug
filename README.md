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



