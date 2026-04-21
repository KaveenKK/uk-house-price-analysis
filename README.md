# UK House Price Analysis(England & Wales)

An exploratory data analysis and predictive modelling project using official HM Land Registry Price Paid Data.

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)
![License](https://img.shields.io/badge/Data-Open%20Government%20Licence-green)

---

## Project Overview

This project analyses residential property sales across England and Wales using the HM Land Registry Price Paid dataset, a publicly available dataset updated monthly by the UK government, covering every residential sale since 1995.

The goal is to uncover pricing trends, regional inequality, and the factors that most influence house prices, before building a baseline predictive model.

---

## Key Questions

1. How are house prices distributed across England & Wales?
2. Which counties are the most and least affordable?
3. How does property type (Detached, Semi, Terraced, Flat) affect price?
4. Do new builds command a premium over existing properties?
5. Is there a seasonal pattern to transaction volumes?
6. Can we predict house prices from available categorical features?

---

## Analysis Sections

| Section | Description |
| :--- | :--- |
| **Data Loading** | Fetch directly from HM Land Registry open data S3 bucket |
| **Data Cleaning** | Handle missing values, outlier removal, feature engineering |
| **Price Distribution** | Histogram and log-scale distribution analysis |
| **Monthly Trends** | Transaction volume and median price by month |
| **Property Type** | Median price comparison across all property types |
| **New Build vs Existing** | Premium analysis across property categories |
| **County Comparison** | Top 15 most expensive and most affordable counties |
| **Tenure Analysis** | Freehold vs Leasehold price breakdown |
| **Predictive Model** | Linear Regression baseline - actual vs predicted |
| **Conclusions** | Key findings and suggested next steps |

---

## Tech Stack

- **Python 3.10**
- **pandas**
- **NumPy**
- **Matplotlib/Seaborn** 
- **Scikit-learn** 

---

## How to Run

### Option 1 - Run locally

```bash
# Clone the repo
git clone https://github.com/KaveenKK/uk-house-price-analysis.git
cd uk-house-price-analysis

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter
jupyter notebook uk_house_price_analysis.ipynb
```

### Option 2 - Run in the browser (no install needed)

Click below to open in Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/KaveenKK/uk-house-price-analysis/blob/main/uk_house_price_analysis.ipynb)

---

## Key Findings

- **Detached houses** have the highest median price; **flats** are the most affordable property type
- **New builds command a significant premium** across all property types
- **Regional disparity is substantial** —the most expensive counties can be 3-4 times the price of the most affordable
- **Transaction volumes peak in spring/early summer**, with a notable dip in January
- A baseline Linear Regression model confirms that categorical features alone have limited predictive power —**location data (postcode level) would be the most impactful addition**

---

## Data Source

**HM Land Registry - Price Paid Data**  
[https://www.gov.uk/government/collections/price-paid-data](https://www.gov.uk/government/collections/price-paid-data)

---

## Author

**Kaveen Kodikarage**  
BSc (Hons) Computing Systems
kaveenyasas14@gmail.com
