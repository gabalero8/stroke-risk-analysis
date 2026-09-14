# Stroke Risk Analysis

A statistical and exploratory analysis of stroke risk factors using **Python**.

The project studies relationships between demographic and clinical variables and the occurrence of stroke, combining exploratory data analysis, statistical inference, distribution fitting, non-parametric estimation, hypothesis testing, and an experimental logistic regression model.

## Objectives

- Explore the dataset and identify relevant patterns in stroke-related variables.
- Study the relationship between stroke occurrence and factors such as age, glucose levels, hypertension, and heart disease.
- Estimate and test probability distributions for selected variables.
- Apply confidence intervals and hypothesis tests.
- Use non-parametric density estimation when simple parametric models do not provide a good fit.
- Explore a logistic regression model for stroke classification.

## Dataset

The dataset includes variables such as:

- Age
- Gender
- Hypertension
- Heart disease
- Average glucose level
- BMI
- Smoking status
- Work and residence type
- Stroke occurrence

The dataset used in the analysis is included in the repository as `stroke-dataset.csv`.

## Analysis

The notebook includes:

### Exploratory Data Analysis

Data inspection, descriptive statistics, visualizations, and analysis of the distributions of relevant variables.

### Statistical Modeling

- Parameter estimation using the method of moments and maximum likelihood.
- Confidence intervals.
- Distribution fitting for variables such as age and average glucose level.
- Inverse-transform simulation.

### Goodness-of-Fit Tests

- **Shapiro-Wilk** test for normality of age.
- **Anderson-Darling** test for average glucose level against a Gamma distribution.
- Bootstrap estimation of the Anderson-Darling p-value.
- Exploration of non-parametric alternatives using **Kernel Density Estimation (KDE)**.

### Hypothesis Testing

Statistical tests are used to study whether clinical variables differ meaningfully between individuals with and without stroke.

### Logistic Regression

An experimental logistic regression model is built using average glucose level and heart disease as predictors.

The model illustrates an important issue in medical classification datasets: high overall accuracy can coexist with very low recall when the target classes are heavily imbalanced.

## Tools

`Python` · `Pandas` · `NumPy` · `SciPy` · `Matplotlib` · `Seaborn` · `Scikit-learn` · `Jupyter Notebook`

## Running the project

Clone the repository:

```bash
git clone https://github.com/gabalero8/stroke-risk-analysis.git
cd stroke-risk-analysis
```

Install the required libraries:

```bash
pip install pandas numpy scipy matplotlib seaborn scikit-learn notebook
```

Start Jupyter:

```bash
jupyter notebook
```

Then open:

```text
notebook final.ipynb
```

## Repository structure

```text
.
├── notebook final.ipynb    # Main analysis notebook
├── stroke-dataset.csv      # Dataset
└── stroke.jpg              # Project cover image
```

## Background

Originally developed as a university project for **INF280**.

This was a team project developed by:

- Cristobal Martinez
- Gabriel Lira
- Francisco Pino
- Catalina Zenteno

## Note

This project is an academic statistical analysis and should not be interpreted as a medical diagnostic tool.
