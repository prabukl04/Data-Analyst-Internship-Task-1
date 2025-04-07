# Data-Analyst-Internship-Task-1

# 📊 Netflix Titles Dataset — Data Cleaning Project

This project involves cleaning and preprocessing the **Netflix Titles dataset** to make it consistent, analysis-ready, and well-structured. The project was executed using **Python in Google Colab**.

---

## 🗂️ Files Included

- `netflix_titles.csv` — The original raw dataset.
- `netflix_titles_cleaned.csv` — The cleaned and processed dataset.
- `netflix_data_cleaning.ipynb` — Google Colab notebook containing all Python code used for data cleaning.
- `heatmap_nulls.png` — Heatmap visualization of missing values before cleaning.

---

## 🧹 Data Cleaning Steps Performed

1. **Loaded the dataset** using `pandas`.
2. **Identified missing values** using `.isnull()` and visualized them as a heatmap using `seaborn`.
3. **Removed duplicate rows** using `.drop_duplicates()`.
4. **Standardized text columns** such as `type` and `country` using `.str.strip()` and `.str.title()`.
5. **Converted `date_added`** to `datetime` format for consistency.
6. **Renamed columns** to lowercase with underscores (e.g., `Date Added` → `date_added`).
7. **Handled missing values**:
   - `director` → "Unknown"
   - `cast` → "Not Available"
   - `country` → "Unknown"
   - `date_added` → Placeholder date (`1900-01-01`)
   - `rating` → "Unrated"
   - `duration` → "Unknown"
8. **Split `duration`** into:
   - `duration_int`: numeric value
   - `duration_type`: unit (e.g., "min", "Season")
9. **Saved the cleaned data** to a new CSV file for future use.

---

## 📊 Visualizations

- A **heatmap** was created using `seaborn` to visualize null/missing values before data cleaning.

---

## 🧪 Requirements

To run this project or replicate it locally:
```bash
pip install pandas seaborn matplotlib
