# Multivariate Analysis of the Physicochemical Characteristics of Portuguese Vinho Verde Wines

## Study Title
APM1220 Summative Assessment 1: Multivariate Analysis of the Wine Quality Dataset

## Research Questions
This project investigates three primary research questions:
1. **MANOVA:** Do red and white wines differ significantly in their overall physicochemical characteristics when several characteristics are considered simultaneously?
2. **PCA:** Can the 11 physicochemical measurements of wine be summarized using a smaller number of principal components while retaining a substantial proportion of the total variability?
3. **EFA:** What underlying latent dimensions or factors explain the relationships among the physicochemical characteristics of wine?

## Dataset Description
The analysis uses the combined Wine Quality Dataset containing physicochemical measurements of Portuguese Vinho Verde wines. 
* **Total Observations:** 6,497 (1,599 red wine samples and 4,898 white wine samples)
* **Variables:** 11 continuous physicochemical variables (e.g., fixed acidity, volatile acidity, citric acid, residual sugar, chlorides, free sulfur dioxide, total sulfur dioxide, density, pH, sulphates, alcohol), one categorical variable (`color`), and an integer-based sensory score (`quality`).

## Dataset Source and Attribution
The dataset was obtained from the UCI Machine Learning Repository.
* **Source:** [Wine Quality Dataset](https://archive.ics.uci.edu/dataset/186/wine+quality)
* **License:** Creative Commons Attribution 4.0 International (CC BY 4.0)
* **Original Citation:** Cortez, P., Cerdeira, A., Almeida, F., Matos, T., & Reis, J. (2009). Modeling wine preferences by data mining from physicochemical properties. *Decision Support Systems*, 47(4), 547-553.

## Statistical Methods
The following multivariate statistical techniques were applied:
* **Exploratory Data Analysis (EDA):** Univariate and bivariate visualizations to assess distributions, correlations, and outliers.
* **Multivariate Analysis of Variance (MANOVA):** To test for significant differences in mean vectors of physicochemical variables between red and white wines.
* **Principal Component Analysis (PCA):** To reduce the dimensionality of the 11 standardized physicochemical variables into orthogonal components.
* **Exploratory Factor Analysis (EFA):** To identify underlying latent constructs driving the observable wine characteristics using Promax rotation.

## Summary of Major Findings
* **MANOVA:** Revealed a statistically significant difference between the physicochemical profiles of red and white wines across the selected variables (Wilks' Lambda = 0.4026, p < 0.001).
* **PCA:** Reduced the 11 input variables into [Insert Number] principal components, which together explained [Insert %]% of the cumulative variance. The primary components represented dimensions such as [Insert PC1 Name] and [Insert PC2 Name].
* **EFA:** Identified [Insert Number] latent factors underlying the data structure, primarily grouped by [Insert Factor 1 Name] and [Insert Factor 2 Name], demonstrating the inherent chemical profiles of the wines.

## Software Used
* **Language:** Python 3
* **Environment:** Google Colab / Jupyter Notebook
* **Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy`, `statsmodels`, `scikit-learn`, `factor_analyzer`

## Instructions for Reproducing the Analysis
1. Clone this repository to your local machine:
   ```bash
   git clone [Insert Your GitHub Repo URL]

2. Ensure the required Python libraries are installed:
pip install pandas numpy matplotlib seaborn scipy statsmodels scikit-learn factor_analyzer

3. Navigate to the code/ directory and open the Python script or Jupyter Notebook (SA1_Wine_Analysis.ipynb).

4. Ensure the winequality-red.csv and winequality-white.csv files are located in the data/ directory relative to the script.

5. Run the script/notebook sequentially to reproduce the data preparation, EDA, MANOVA, PCA, and EFA outputs.
