# DSA210-termProject
# DSA210 2025-2025 Fall Term Project by Emir Eğilli

# Project Overview #

This project investigates whether a nation’s food economy can serve as an indicator of international football success. Specifically, it analyzes the relationship between food supply metrics — such as per-capita daily calorie availability, per-capita protein and meat supply, and the household share of expenditure on food — and FIFA World Cup performance. Additionally, GDP per capita and population will be included as control variables to make the comparison more meaningful and fair. Machine learning methods will later be applied to examine whether these food-related indicators can help predict if a country will reach advanced stages in the World Cup.

# Motivation #

**Personal Interest**

-I am highly interested in sports analytics and the factors that contribute to national football success. The FIFA World Cup is not only a sports competition but also a reflection of economic and social structures. Understanding how everyday life conditions, especially food-related economic factors, correlate with football performance is both fascinating and meaningful.

**Application**

-This project allows me to apply data science techniques to a globally relevant problem while improving my skills in data collection, data analysis, statistical testing, and machine learning.

# Data Source #

All datasets used in this project are publicly available:

**Food Supply & Nutrition Data**

-Variables: Daily calorie supply (kcal/person/day), protein supply (g/person/day), meat supply (kg/person/year)

-Source: FAOSTAT (United Nations Food and Agriculture Organization)

-Format: CSV download

**Food Expenditure Share**

-Variable: Share of household expenditure on food (%)

-Source: FAOSTAT

-Format: CSV

**Economic Indicators**

-Variables: GDP per capita (USD), Population

-Source: World Bank Open Data

-Format: API / CSV

**World Cup Results**

-Variables: Tournament stage (Group → Winner) by country and year

-Source: Wikipedia (FIFA World Cup standings tables)

-Format: Extracted using pandas.read_html()

-These datasets will be merged using country names and aligned to World Cup years (using 1–3 years prior averages for each edition).

# Tools & Technologies Used #

- **Programming Language:** Python 

- **Data Analysis & Processing:** Pandas

- **Data Visualization:** Matplotlib, Seaborn

- **Statistical Analysis:** SciPy

- **Machine Learning:** Scikit-learn

# Data Analysis #

This project will follow a structured process:

-**Data Cleaning & Preprocessing**: Handling missing values and inconsistent entries

-**Standardizing country identifiers and year alignment**

-**Selecting features relevant to food economy and controls**

-**Merging datasets into one structured table**

-**Exploratory Data Analysis (EDA)**

-**Summary statistics:** Correlation analysis and visualizations (heatmaps, line charts…)

-**Statistical Testing:** Hypothesis tests comparing Top-8 teams vs Non-Top-8 teams (Example: Welch t-test on meat supply or calorie availability).

-**Machine Learning Models:** Classification (Logistic Regression / Random Forest) and predicting whether a country reaches Top-8 in the World Cup.

# Expected Findings #

-Countries with stronger food economy indicators may be more likely to reach advanced stages in the World Cup.

-High calorie/protein/meat supply and lower food expenditure share may correlate with better football performance.

-Food-based economic metrics may show predictive value even after controlling for GDP and population.

# Limitations and Future Work #

-Some countries may lack complete datasets for all variables and years.

-Confounding variables such as football development programs or player export rates are not included yet.

-In future work, additional sports-specific indicators such as FIFA rankings or academy success metrics could improve the prediction model.
