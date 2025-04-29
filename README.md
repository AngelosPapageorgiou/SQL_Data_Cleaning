# 🧹 SQL Data Cleaning Project

![SQL](https://img.shields.io/badge/Language-SQL-blue)
![Status](https://img.shields.io/badge/Stage-Completed-brightgreen)
![License](https://img.shields.io/badge/License-MIT-lightgrey)
![Inspired by](https://img.shields.io/badge/Inspiration-Alex%20The%20Analyst-orange)

This project demonstrates a complete SQL-based data cleaning process using a dataset of tech layoffs. The goal is to take raw and inconsistent data and transform it into a clean, structured, and analysis-ready format.

---

## 📌 Dataset

The dataset used contains information about layoffs across tech companies worldwide, including:

- Company name
- Location
- Industry
- Number and percentage of employees laid off
- Funding stage and amount
- Date of layoffs

---

## ⚙️ Cleaning Process

The following data cleaning tasks were performed:

### ✅ Duplicate Removal
Used the `ROW_NUMBER()` window function to identify and delete exact duplicates.

### ✂️ Standardization
- Trimmed extra spaces from text fields (e.g., `company`)
- Unified variations in industry and country names
- Cleaned and updated values like `United States` or `Crypto`

### 📅 Date Conversion
Converted date strings (`MM/DD/YYYY`) to proper SQL `DATE` type.

### 🧼 Handling Missing Values
- Identified and removed rows with no `total_laid_off` and `percentage_laid_off`
- Filled missing industries by referencing the same company with valid entries

---

## 📁 Files

- `SQL Data Cleaning Project.sql`: Full SQL script with all steps
- `layoffs data.csv`: Raw dataset used for this project
- `README.md`: Project documentation

---

## ▶️ How to Run

1. Import `layoffs data.csv` into your SQL environment.
2. Run the SQL script step by step from `SQL Data Cleaning Project.sql`.
3. Inspect the cleaned table: `layoffs_staging2`.

---

## 📌 Inspiration

This project is inspired by [Alex The Analyst](https://www.youtube.com/@AlexTheAnalyst), whose content helps analysts develop real-world SQL skills.

---

## 👨‍💻 Author

**Angelos Papageorgiou**  
Data Science & Analytics Enthusiast  
🇬🇷 Athens, Greece

---

## 📝 License

This project is licensed under the MIT License.

