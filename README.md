# Inflation Dynamics in High Remittance-Receiving Countries

This project investigates how remittances, real interest rates, and exchange rates impact inflation trends across 55 countries with high remittance-to-GDP ratios, using data spanning from 1960 to 2023.

---

## 📌 Motivation

Inflation significantly affects purchasing power and economic stability, especially in developing countries. While remittances are typically considered a stabilizing economic force, their true impact on inflation is complex and may vary with other macroeconomic indicators like interest and exchange rates. This project seeks to model and understand those interactions.

---

## 📊 Dataset

- **Countries:** 266 countries (filtered to 55 where remittances > 5% of GDP)
- **Time Period:** 1960–2023
- **Data Sources:** World Bank indicators for inflation, remittances, real interest rates, and exchange rates
- **Total Observations:** 17,556 rows per variable

---

## ⚙️ Methodology

### 1. **Data Preprocessing**
- Merging and reshaping four macroeconomic datasets
- Removal of country groups and NaNs
- Outlier detection via IQR and statistical thresholds
- Normalization with Min-Max Scaling

### 2. **Models Used**
- 🔁 **Linear Regression with interaction terms**
- 🌲 **Random Forest Regressor**
- 🧠 **Neural Network with dropout layers**
- 📦 **K-Means Clustering for country pattern grouping**
- 🧮 **Pooled OLS, Fixed Effects, Random Effects, and GMM (Arellano–Bond)**

---

## 📈 Results

- **Real interest rate** showed the strongest (negative) correlation with inflation.
- **Remittances and exchange rates** alone were less impactful but gained relevance through interaction terms.
- **Neural Network** performed well with low MSE and MAE.
- **Random Forest** captured nonlinear feature interactions effectively.
- Statistical models supported a linear relationship, while machine learning models suggested a possible nonlinear impact of remittances.

---

## 🧪 Hypothesis

- **H₀ (Accepted):** The relationship between remittances and inflation is **non-linear**, with diminishing returns at higher remittance levels.
- **H₁ (Rejected):** A direct linear relationship exists between remittances and inflation.

---

## 📌 Key Findings

- There is strong evidence that **real interest rates inversely affect inflation**.
- **Remittances alone do not predict inflation** well unless considered alongside interest and exchange rates.
- The non-linear interaction of variables is better captured by machine learning models.

---

## 📚 References

- Regmi, S. (2023). *Are Remittances Inflationary? Evidence from Emerging Nations in South Asia.*
- Narayan, P. K. et al. (2011). *Do Remittances Induce Inflation?*
- Medeiros, M. C. et al. (2021). *Forecasting Inflation in a Data-Rich Environment.*

---

## 👨‍💻 Authors

- Bibek Koirala    

**Course**: CS 533 - Data Mining and Big Data Analysis  
**Institution**: Southern Illinois University Carbondale  
**Date**: December 2024

---

## 🛠️ How to Use

To reproduce results:
```bash
# Clone the repository
git clone https://github.com/vbek/Inflation-Dynamics-Remittance-and-Interest-Rate.git
cd Inflation-Dynamics-Remittance-and-Interest-Rate

# Install required dependencies
pip install -r requirements.txt

```

---
