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
