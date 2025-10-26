# Regression of Life Expectancy (1923–2023)

This project analyzes how life expectancy across countries has changed over the last century.  
Using **R**, I performed exploratory data analysis, built a **simple linear regression model**, and evaluated its ability to predict 2023 life expectancy from 1923 data.

---

## 🧠 Objective
To model and interpret the relationship between life expectancy in **1923** and **2023**,  
and to explore what historical factors might explain modern longevity patterns.

---

## 📊 Data
The dataset includes global life expectancy values for 1923 and 2023 by country.  
Missing 2023 values were predicted using the regression model.

| Column | Description |
|---------|-------------|
| country | Country name |
| life1923 | Life expectancy in 1923 |
| life2023 | Life expectancy in 2023 |

*(If the data came from a public source, include a link. If not, provide a cleaned sample only.)*

---

## 🧩 Methodology

1. **Exploratory Data Analysis**
   - Histograms of 1923 and 2023 life expectancies
   - Identification of outliers and historical context (e.g., war, epidemics)

2. **Linear Regression Model**
   - Model: `life2023 = β₀ + β₁ * life1923 + ε`
   - Evaluated model significance (p-values, ANOVA)
   - Calculated **correlation**, **R²**, and **residual diagnostics**

3. **Prediction**
   - Predicted 2023 life expectancy for countries missing modern data
   - Used confidence and prediction intervals for interpretation

4. **Residual Analysis**
   - Histogram and scatterplot of residuals
   - Normality test (Shapiro-Wilk)
   - Discussion of model adequacy and potential nonlinear effects

---

## 📈 Key Results

- **Positive correlation** between life expectancy in 1923 and 2023 (~0.45 in sample)
- Each additional year in 1923 life expectancy corresponds to **~0.7 years higher** in 2023
- The linear model explains **≈30%** of the total variability (R² ≈ 0.30)
- Residuals are approximately random and normally distributed
- Global life expectancy increased dramatically (~30–40 years average gain)

---

## 🧮 Tools & Libraries

- **Language:** R  
- **Libraries:** tidyverse, ggplot2, broom, rpart  
- **Concepts:** Linear Regression, ANOVA, Correlation, Residual Diagnostics

---

## 🧠 Interpretation
The model highlights how early 20th-century public health conditions were modest predictors of modern longevity, suggesting that social, economic, and medical developments since 1923 played a substantial role in extending life expectancy.
