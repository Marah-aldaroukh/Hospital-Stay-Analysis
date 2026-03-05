# 📊 Medical Data Analysis: Impact of Illness Severity on Hospital Stay

## 📌 Project Overview
This project analyzes **318,438 patient records** to understand the impact of **illness severity** on **length of hospital stay**. The analysis includes data cleaning, handling missing values, outlier treatment, and advanced statistical testing (ANOVA, Tukey HSD).

## 🔍 Key Findings
- **Illness severity significantly affects length of stay** (P-value < 0.001)
- Patients with **extreme severity** stay significantly longer than moderate and minor cases
- **All pairwise differences between severity groups are significant**
- Relationship is **non-linear** (weak linear correlation but clear categorical differences)

| Comparison | Mean Difference | Significance |
|------------|-----------------|--------------|
| Extreme vs Minor | -6.55 days | Significant (P<0.05) |
| Extreme vs Moderate | -2.98 days | Significant (P<0.05) |
| Minor vs Moderate | 3.57 days | Significant (P<0.05) |

## 🛠️ Tools & Technologies
- **Python**: Pandas, NumPy, Matplotlib, Seaborn
- **Statistical Analysis**: SciPy, Statsmodels (ANOVA, Tukey HSD)
- **Environment**: Jupyter Notebook

## 📂 Repository Contents
- `analysis2.ipynb` – Complete Jupyter notebook with all code
- `Medical_Data_Analysis_Report.pdf` – Full project report
- `boxplot_severity.png` – Visualization of results
- `README.md` – This file

## 🚀 How to Run
1. Clone this repository
2. Install required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn scipy statsmodels
   ```
3. Open `analysis.ipynb` in Jupyter Notebook
4. Run all cells

## 📁 Data Cleaning Summary
- **Missing values**: `Bed Grade` (113) and `City_Code_Patient` (4,532) → filled with mode
- **Duplicates**: None found
- **Text standardization**: All text columns converted to lowercase and stripped
- **Categorical encoding**: Age and Stay converted to numeric values
- **Outliers**: Detected using IQR method and treated with capping (0 outliers remaining)

## 📬 Contact
For questions or collaboration, feel free to reach out via:  
[marahmaroo72001@gmail.com]

## 📄 License
This project is for educational purposes.
