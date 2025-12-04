# COVID-19 Global Cases Analysis

A complete exploratory data analysis (EDA) of COVID-19 cases across 225 countries, covering total cases, deaths, population distribution, continent-wise impact, fatality percentages, and statistical correlations. This project helps visualize how the pandemic affected different regions worldwide.

---

## Dataset Overview

The dataset contains **225 rows × 10 columns**, summarizing COVID-19 metrics aggregated by country.

### Features Include:
- Country  
- Other Names  
- ISO 3166-1 Alpha-3 Code  
- Population  
- Continent  
- Total Cases  
- Total Deaths  
- Total Cases per 1M Population  
- Total Deaths per 1M Population  
- Death Percentage  

---

## Data Preparation

Steps performed:

- Loaded dataset using pandas  
- Verified shape: **225 × 10**  
- Identified **1 missing value** in *Other Names*  
- Replaced missing value with **"Montenegro"**  
- Confirmed dataset had no further null values  
- Generated statistical summaries using `.describe()`  
- Used `.columns.tolist()` to identify hidden whitespace characters  
- Constructed a numeric-only DataFrame for correlation analysis  

---

## Analysis & Visualizations

### 1. Top 5 Countries by Total COVID-19 Cases
- USA  
- India  
- Brazil  
- France  
- Germany  

Visualized using a bar chart to compare severity.

### 2. Bottom 5 Countries by Total COVID-19 Cases
- Micronesia  
- Saint Helena  
- Marshall Islands  
- Niue  
- Western Sahara  

Shown using scaled bar charts for clarity.

### 3. Top 5 Countries by Total Deaths
- USA  
- Brazil  
- India  
- Russia  
- Mexico  

### 4. Countries with Highest Death Percentage
Yemen, Western Sahara, Sudan, Peru, and Mexico showed unusually high fatality percentages due to low case counts.

### 5. Continent-wise Total Cases
- Europe recorded the highest cases  
- Followed by Asia and North America  
- Oceania had the lowest case numbers  

### 6. Population vs Total Cases (Scatter Plot)
- General trend: Higher population → Higher cases  
- Three major outliers highlighted  
- Showed population alone didn’t determine outbreak severity  

### 7. Correlation Heatmap
Correlation between:
- Total Cases  
- Total Deaths per 1M  

Correlation ≈ **22%**, indicating a weak but notable relationship.

---

## Key Insights

- Only one missing value required imputation.  
- USA had the highest number of cases and deaths globally.  
- Micronesia had the lowest number of reported cases.  
- High fatality percentages in some countries stemmed from small case counts.  
- Population size does not fully explain infection spread—government response and preparedness were major factors.  
- Europe had the highest continent-wise case count, likely influenced by dense travel networks and early exposure.  
- Weak correlation between total cases and deaths per million suggests large differences in healthcare quality and response efficiency.

---

## Technologies Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Jupyter Notebook  

---

## How to Run

### Clone the Repository
``bash
git clone https://github.com/yourusername/CovidCasesAnalysis.git
**Install Required Packages**
bash
Copy code
pip install pandas numpy matplotlib seaborn
Open the Notebook
bash
Copy code
jupyter notebook covid_analysis.ipynb

## Future Improvements
- Add time-series forecasting for cases and deaths

- Compare vaccination rates across countries

- Build interactive dashboards using Streamlit, Plotly, or PowerBI

- Add continent-wise interactive drilldowns

- Use machine learning to predict death percentages

## Contributing
Pull requests are welcome.
Feel free to add more visualizations, extend the analysis, or enhance data quality.

## Support
If this repository was helpful, consider giving it a star to support more analytical projects.
