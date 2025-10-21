# 🎬 IMDB Movie Data Analysis Project Report

## 📘 1. Introduction
The purpose of this project was to perform an end-to-end analysis of a large movie dataset (IMDB movies) to uncover insights related to genres, durations, languages, directors, budgets, and box office performance.  
The project involved comprehensive data cleaning, exploratory data analysis (EDA), correlation analysis, and creation of a Summary Dashboard to visualize and interpret key insights.

---

## 🧹 2. Data Cleaning and Preparation

### 2.1 Initial Dataset Overview
- **Initial Rows:** 5,044 (with headers)
- **Initial Columns:** Included movie metadata such as *Title, Genre, Duration, Language, Director, Budget, Gross, IMDB Rating,* etc.
- **Issues Identified:**
  - Missing values in numeric and categorical fields
  - Duplicate movie entries
  - Outliers in *Budget* and *Gross* columns

### 2.2 Cleaning Operations Performed
1. **Removed Duplicates**
   - Identified using conditional formatting and UNIQUE formula.
   - Duplicates deleted to retain only unique movie titles.
2. **Handled Missing Values**
   - Numeric columns (Budget, Gross, IMDB Score): replaced with median.
   - Categorical fields (Genre, Language): replaced with mode or removed.
3. **Removed Outliers**
   - Applied IQR method to detect and remove outliers in Budget and Gross.
4. **Result After Cleaning**
   - Final Row Count: **4,936 rows**
   - Dataset became consistent and analysis-ready.

### 2.3 Data Organization
After cleaning, dedicated Google Sheets tabs were created for analysis:

| Sheet Name | Purpose |
|-------------|----------|
| Analysis | Initial cleaning overview |
| Data Cleaning | Final cleaned dataset |
| Important Columns | Selected relevant fields |
| Important Columns Backup | Backup of key data |
| Genre Analysis | Genre-wise performance metrics |
| Duration Analysis | Duration & IMDB correlation |
| Language Analysis | Language-wise ratings |
| Director Analysis | Director performance metrics |
| Budget Analysis | Profitability and correlation |
| Cleaned for Scatter | Data for scatter plot |
| Summary Dashboard | Final summary visualization |

---

## 📊 3. Exploratory Data Analysis

### 3.1 Genre Analysis
- **Total genres analyzed:** 20  
- **Most common genre:** Drama (2,594 movies)  
- **Highest average IMDB rating:** War (Avg 7.36)  
**Insight:** Drama dominates production count, while War and Biography lead in quality.

### 3.2 Duration Analysis
- **Average Duration:** 108.15 minutes  
- **Median:** 104 minutes  
- **Range:** 7–330 minutes  
- **Correlation (Duration vs IMDB):** Weak (|r| < 0.3)  
**Insight:** Movies between 90–120 minutes perform best.

### 3.3 Language Analysis
| Language | Mean IMDB | Count |
|-----------|------------|-------|
| English | 6.37 | 4607 |
| Japanese | 7.42 | 17 |
| German | 7.34 | 19 |
| French | 7.02 | 72 |

**Insights:**
- English dominates in quantity.
- Japanese & European languages score higher in quality.

### 3.4 Director Analysis
- **Top Directors by Count:** Steven Spielberg (26), Woody Allen (22), Martin Scorsese (20)
- **Top by Avg IMDB:** Martin Scorsese (7.66)
- **Most Consistent:** Woody Allen (SD = 0.53)
**Insight:** Spielberg leads in volume, Scorsese in quality.

### 3.5 Budget Analysis
- **Top 3 Profitable Movies:**
  1. *Avatar* – $523,505,847 profit (3.21x)
  2. *Jurassic World* – $502,177,271 profit (4.35x)
  3. *Titanic* – $458,672,302 profit (3.29x)
- **Correlation (Budget vs Gross):** 0.4519 (Moderate Positive)
- **R² Value:** ≈ 0.20  
**Insight:** High budgets yield higher gross but not always — creativity matters more.

### 3.6 Cleaned Scatter Data
- Created filtered subset `Budget_Filtered` for regression visualization.
- Scatter plot shows moderate upward trend (budget vs gross).

---

## 📈 4. Summary Dashboard

| Metric | Value |
|--------|-------|
| Most Common Genre | Drama |
| Highest Rated Genre | War |
| Average Duration | 108.15 mins |
| Most Common Language | English |
| Top Director (Avg IMDB) | Mitchell Altieri – 8.70 |
| Budget ↔ Gross Corr. | 0.1119 (Weak Positive) |

**Correlation Interpretation:** Weak positive — higher budgets slightly improve earnings.

### 4.2 Insights
- 🎭 Drama dominates as universal genre.
- 🎬 War, Biography, Documentary are most acclaimed.
- 🌍 Non-English movies (esp. Japanese, German) score higher.
- 🕒 90–120 min duration ideal for engagement.
- 💰 Creativity & audience appeal matter more than budget size.

### 4.3 Recommendations
- **Producers:** Focus on strong scripts and balanced budgets.  
- **Studios:** Prioritize mid-budget, genre-aligned projects.  
- **Streaming Platforms:** Highlight high-rated foreign titles.  
- **Filmmakers:** Target 2-hour duration sweet spot.  
- **Analysts:** Explore actor popularity & release year effects.

---

## 🧾 5. Conclusion
This Google Sheets project successfully cleaned, structured, and analyzed IMDB data to uncover actionable insights.  
From wrangling to visualization, each step enhanced integrity and interpretability.  
The final Summary Dashboard offers a one-glance overview of genre trends, language effects, direction quality, and profitability.

---

## 🧩 6. Tools & Techniques Used
- **Platform:** Google Sheets  
- **Techniques:** Data Cleaning, Filtering, IQR Outlier Removal, Correlation Analysis, Dashboard Creation  
- **Visuals:** Scatter Plot, Summary Table, Correlation Charts  
- **Functions Used:**  
  COUNTIF, UNIQUE, FILTER, CORREL, INDEX-MATCH, IF, ROUND, AVERAGE, STDEV, SORT, MAX, MIN  

---

## 🧮 7. Summary Metrics
| Metric | Value |
|--------|-------|
| Total Rows (after cleaning) | 4,936 |
| Duplicates Removed | 64 |
| Missing Values Treated | Several (varied by column) |
| Outliers Removed | Extreme Budget & Gross values |
| Final Sheets Created | 9 |

---
✅ **Project Completed By:** *Debashish Borah*  
📅 **Platform:** Google Sheets  
📊 **Project:** IMDB Movie Analysis  
