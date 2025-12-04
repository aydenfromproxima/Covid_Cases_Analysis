**COVID-19 Global Cases Analysis**

A complete exploratory data analysis (EDA) of COVID-19 cases across 225 countries, including total cases, deaths, population, continent-wise distribution, death percentages, and correlations. This project helps identify how COVID-19 impacted different regions worldwide.

**Dataset Overview**

The dataset contains 225 rows × 10 columns, with global COVID-19 metrics aggregated by country.

**Features include:**

Country
Other Names
ISO 3166-1 Alpha-3 Code
Population
Continent
Total Cases
Total Deaths
Total Cases per 1M Population
Total Deaths per 1M Population
Death Percentage
Data Preparation

**In the notebook, I :**

 Loaded the dataset using pandas
 Checked data shape → 225 rows × 10 columns
 Identified 1 missing value in Other names
 Replaced missing value with “Montenegro”
 Confirmed no more null values
 Used describe() for statistical analysis
 Used .columns.tolist() to reveal invisible characters in column names
 Cleanly constructed numeric-only DataFrame for correlation analysis

**Analysis & Visualizations**

Your notebook includes multiple visual insights and statistics:

1. Top 5 Countries by Total COVID Cases

USA
India
Brazil
France
Germany
Bar chart plotted to visualize case severity.

2. Least 5 Countries by Total COVID Cases

Micronesia
Saint Helena
Marshall Islands
Niue
Western Sahara
Visualized using scaled bar chart for better clarity.

3. Top 5 Countries by Total Deaths

USA
Brazil
India
Russia
Mexico

4. Countries with Highest Death Percentage

Yemen, Western Sahara, Sudan, Peru, Mexico had the highest fatality percentages.

5. Continent-wise Total Cases

Bar chart showing:
Europe had the highest cases
Followed by Asia and North America
Oceania had the least

6. Population vs Total Cases (Scatter Plot)

General trend: Higher population → Higher cases
Three significant outliers highlighted

Showed the importance of healthcare response and policy

7. Correlation Heatmap

Between:
Total Cases
Total Deaths per 1M
Correlation ≈ 22%, indicating a weak but noticeable relationship.

**Key Insights**

The dataset required minimal cleaning — only one null value.
USA has the highest cases and deaths.
Micronesia recorded the lowest number of cases.
Some countries showed unusually high death percentages due to low case counts.
Population alone does not determine total infections — government response and infrastructure played major roles.
Continent-wise, Europe had the most cases, possibly due to dense travel and early exposure.
The correlation between total cases and deaths per million is weak, showing that medical care quality differed widely.

**Language & Library Used**
Python
Pandas
NumPy
Matplotlib
Seaborn
Jupyter Notebook

**How to Run**
Clone the repository:
git clone https://github.com/yourusername/CovidCasesAnalysis.git

Install required packages:
pip install pandas numpy matplotlib seaborn

Open the notebook:
jupyter notebook covid_analysis.ipynb

**Future Improvements**
Add time-series forecasting for cases/deaths
Compare vaccination rates between countries
Build a dashboard using PowerBI / Streamlit / Plotly
Add interactive continent-wise drilldown charts
Include machine learning to predict death percentage

Contributing

Pull requests are welcome!
Feel free to extend the analysis, add plots, or clean the dataset further.

**If You Found This Useful**
Give this repository a star to support more analytical projects like this!
