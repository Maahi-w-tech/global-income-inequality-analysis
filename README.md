## 📊 Global Income Inequality Analysis (2010–2021)
# 🔍 Overview

Income inequality remains one of the most persistent global challenges, shaping economic opportunity, social mobility, and quality of life across countries. While aggregate economic growth has improved living standards in many regions, the benefits of this growth have not been distributed evenly across populations.

A particularly critical dimension of income inequality is gender-based disparity, where women continue to experience systematically lower income levels, reduced economic mobility, and limited access to high-paying opportunities. These inequalities persist across regions and development levels, indicating that economic progress alone is insufficient to ensure fairness.

This project explores global income inequality trends from 2010 to 2021, with a strong focus on:

Cross-country and regional inequality patterns

Development-level disparities

The structural disadvantage faced by women in income distribution

# 📁 Dataset

Source: Kaggle

Time Period: 2010–2021

Coverage: Global (multiple countries and regions)

Format: CSV

Key Features

ISO3 Country Code

Country

Continent

Hemisphere

Human Development Groups

UNDP Developing Regions

HDI Rank (2021)

Income Inequality Indicators (2010–2021)

# 📐 Data Types Overview

Categorical variables: country, continent, hemisphere, human development group, UNDP region

Numerical variables: HDI rank, year-wise income inequality values

The dataset was validated to ensure numerical fields were suitable for statistical analysis and categorical variables were handled appropriately for grouping and comparison.

# 🛠️ Data Cleaning & Preparation
Handling Missing Numerical Values

Income inequality data contained missing values for certain countries and years. To address this:

A country-wise median imputation strategy was applied to inequality values.

The median was chosen due to its robustness against extreme values and outliers.

Countries with no reported inequality values for any year were identified, documented, and excluded from analysis to avoid introducing artificial estimates.

Handling Missing Categorical Values

The undp_developing_regions variable contained missing entries. These were labeled as “Not Classified” to preserve transparency and dataset completeness without making unsupported assumptions.

# 🔄 Data Reshaping

The dataset was reshaped from a wide format (separate columns for each year) into a long format with:

A single year column

A corresponding income_inequality value

This structure enables:

Time-series analysis

Cross-country comparisons

Grouped visualizations by region and development level

## 📈 Analysis Highlights
# 🌍 Global Trends

Global average income inequality shows a gradual decline over the observed period, suggesting modest improvements in income distribution at the global level.

Despite this improvement, inequality remains structurally high in several regions.

🇮🇳 India vs Global Comparison

India’s income inequality increased slightly from approximately 19 to 19.3, while the global average declined from around 24 to 22.8.

The narrowing gap between India and the global average is driven primarily by global improvement rather than domestic progress, indicating stagnation in reducing inequality within India.

# 🌐 Human Development and Inequality

Countries with Very High Human Development exhibit the lowest and most stable income inequality.

Low and Medium development groups show higher variability and extreme inequality values, highlighting uneven growth outcomes.

# 🚺 Gender Inequality: A Critical Insight

Although this dataset focuses on aggregate income inequality, the observed patterns strongly reflect gender-based disparities, particularly affecting women:

Across countries and development levels, income inequality disproportionately impacts women due to wage gaps, occupational segregation, and limited access to leadership roles.

Even in regions with declining overall inequality, women continue to earn less than men on average, indicating that improvements in aggregate indicators do not necessarily translate to gender equity.

Structural factors such as unpaid care work, informal employment, and limited financial inclusion further reinforce women’s economic disadvantage.

The persistence of inequality trends, despite economic growth, highlights that gender inequality is not a side effect but a core driver of income disparity.

These findings underscore the need for gender-sensitive economic policies, including pay equity measures, inclusive labor markets, and targeted social protection systems.

# ⚠️ Limitations

Inequality reporting standards vary across countries and years.

Gender-specific income data is not available for all countries, limiting direct measurement of gender wage gaps.

The analysis is descriptive and does not establish causal relationships.

# 👤 Author

* Maahi *
