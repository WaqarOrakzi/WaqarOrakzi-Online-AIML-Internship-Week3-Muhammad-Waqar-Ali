# 🏠 House Prices — Advanced Data Visualization & Feature Engineering

## 📌 Project Overview

This project is part of the **AI/ML Internship — Week 3: Data Visualization & Feature Engineering**.  
The main objective is to perform professional-level exploratory data analysis (EDA), advanced visualization, feature engineering, encoding, scaling, skewness treatment, and feature selection on the **House Prices — Advanced Regression Techniques** dataset.

The project demonstrates how raw housing data can be transformed into a machine-learning-ready dataset through systematic preprocessing and visualization techniques.

---

# 📂 Dataset

Dataset Used:  
House Prices — Advanced Regression Techniques

Dataset Path (Kaggle):

```python
/kaggle/input/datasets/waqarokzi/house-prices-advanced-regression-techniques/train.csv
```

---

# 🎯 Project Goals

- Perform advanced data visualization using Matplotlib & Seaborn
- Analyze feature distributions and relationships
- Engineer meaningful features from raw data
- Handle categorical variables using multiple encoding strategies
- Compare feature scaling methods
- Detect and reduce skewness
- Perform feature selection
- Build reusable preprocessing functions
- Create a professional analytics dashboard

---

# 🛠️ Technologies & Libraries

## Python Libraries

- pandas
- numpy
- matplotlib
- seaborn
- scipy
- sklearn

---

# 📊 Part A — Data Visualization

## ✔ Step 1 — Environment Setup & Dataset Loading

- Imported required libraries
- Configured professional plotting style
- Loaded dataset using `pd.read_csv()`
- Identified numerical & categorical features
- Found top correlated features with `SalePrice`

---

## ✔ Step 2 — Distribution Analysis

### Chart 1
- SalePrice histogram
- Log-transformed SalePrice histogram
- Mean lines & skewness annotations

### Chart 2
- Box plot of `GrLivArea`
- Violin plot of `GrLivArea`

Generated Files:
- `w3_saleprice_distribution.png`
- `w3_grlivarea_distribution.png`

---

## ✔ Step 3 — Multi-Variable Scatter Plot

Visualized:

- `GrLivArea`
- `SalePrice`
- `OverallQual`
- `GarageCars`

Features:
- Polynomial regression line
- Correlation annotation
- Color mapping

---

## ✔ Step 4 — Time-Based Trend Analysis

Created:
- Houses built per decade
- Average SalePrice per decade

Generated File:
- `w3_time_trend.png`

---

## ✔ Step 5 — Statistical Visualization

### Chart 5
Neighborhood vs SalePrice boxplots

### Chart 6
Correlation heatmap of top numerical features

Generated Files:
- `w3_boxplot_neighborhoods.png`
- `w3_heatmap.png`

---

## ✔ Step 6 — Advanced Seaborn Visualizations

### PairPlot
Visualized relationships among:
- SalePrice
- GrLivArea
- TotalBsmtSF
- OverallQual
- YearBuilt

### FacetGrid
Kitchen quality vs SalePrice distribution

Generated Files:
- `w3_pairplot.png`
- `w3_facetgrid.png`

---

# ⚙️ Part B — Feature Engineering

## ✔ Step 7 — Created 8 Engineered Features

| Feature | Description |
|---|---|
| TotalSF | Total property area |
| TotalBaths | Weighted bathroom count |
| HouseAge | Age at sale time |
| RemodelAge | Years since remodeling |
| HasRemodeled | Remodel indicator |
| QualCond | Quality × Condition interaction |
| PricePerSF | Price density |
| IsNewHouse | Newly built house indicator |

---

## ✔ Step 8 — Correlation Analysis

- Ranked all features by correlation with `SalePrice`
- Built correlation bar chart
- Evaluated effectiveness of engineered features

---

## ✔ Step 9 — Categorical Variable Analysis

Encoding strategies used:

| Strategy | Usage |
|---|---|
| Label Encoding | Ordinal quality features |
| One-Hot Encoding | Low-cardinality nominal features |
| Frequency Encoding | High-cardinality features |
| Drop | Low-information columns |

---

## ✔ Step 10 — Applied Encoding

Applied:
- Explicit quality mapping
- One-hot encoding
- Frequency encoding
- Label encoding

Verified no remaining object columns.

---

## ✔ Step 11 — Feature Scaling

Compared:
- StandardScaler
- MinMaxScaler
- RobustScaler

Visualization:
- Distribution comparison before/after scaling

---

# 📉 Part C — Skewness & Feature Selection

## ✔ Step 12 — Skewness Detection

- Computed skewness for all numerical features
- Classified skew severity
- Visualized top skewed features

---

## ✔ Step 13 — Skewness Transformation

Applied:
- `log1p`
- `sqrt`
- `Box-Cox`

Selected best transformation for `SalePrice`.

---

## ✔ Step 14 — Feature Selection

Techniques Used:
- Correlation-based filtering
- Variance threshold
- Multicollinearity removal

Generated optimized feature subset.

---

## ✔ Step 15 — Reusable Functions

Created production-quality functions:

### 1. `visualize_distributions()`
Creates histogram grids with skewness.

### 2. `encode_quality_column()`
Encodes ordinal quality features.

### 3. `full_scaling_pipeline()`
Automates scaling workflow.

---

# 📊 Part D — Professional Dashboard

## ✔ Step 16 — Final Dashboard

Dashboard Includes:
1. SalePrice distributions
2. Scatter regression analysis
3. Feature importance chart
4. Boxplots by quality
5. Correlation heatmap
6. Scaling comparison

Generated File:
- `week3_dashboard.png`

---

# 📈 Key Insights

- `OverallQual`, `GrLivArea`, and `TotalSF` strongly influence SalePrice.
- Feature engineering significantly improved predictive relationships.
- Log transformation greatly reduced skewness in SalePrice.
- StandardScaler performed best for linear-model preparation.
- Correlation analysis helped remove redundant features.

---

# 🚀 Future Improvements

- Train Linear Regression & XGBoost models
- Hyperparameter tuning
- Cross-validation
- Feature importance using SHAP
- Model deployment using Flask or Streamlit

---

# 📁 Output Files

| File | Description |
|---|---|
| w3_saleprice_distribution.png | SalePrice histograms |
| w3_grlivarea_distribution.png | GrLivArea distribution plots |
| w3_time_trend.png | Time trend analysis |
| w3_boxplot_neighborhoods.png | Neighborhood boxplots |
| w3_heatmap.png | Correlation heatmap |
| w3_pairplot.png | Pairplot visualization |
| w3_facetgrid.png | Kitchen quality facet grid |
| week3_dashboard.png | Final professional dashboard |

---

# 👨‍💻 Author

Muhammad Waqar Ali

AI/ML Internship — Week 3  
Data Visualization & Feature Engineering

---

# 📜 License

This project is created for educational and internship learning purposes.
