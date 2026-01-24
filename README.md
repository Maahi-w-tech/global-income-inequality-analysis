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
# 🌍 Global Income Inequality Trends

Global income inequality shows a gradual but consistent decline from 2010 to 2021, decreasing from approximately 24 to 22.8.

The downward trend is slow and incremental, indicating that while the world is making progress toward more equitable income distribution, the pace of change remains limited.

The decline becomes more noticeable after the mid-2010s, suggesting that global policy efforts and redistribution mechanisms may have begun yielding modest results in recent years.

Despite this improvement, global inequality levels remain structurally high, highlighting the persistence of income disparities worldwide.

# 🌐 Inequality by Continent

Africa exhibits the highest median income inequality along with the widest variation, indicating severe and uneven income distribution across countries.

America also shows relatively high inequality levels with a broad spread, suggesting persistent structural disparities.

Asia demonstrates moderate inequality with comparatively lower variability, though disparities remain significant across countries.

Europe consistently displays the lowest and most stable inequality levels, reflecting stronger redistributive systems and social safety nets.

Oceania shows moderate inequality with limited variability, indicating relatively stable income distribution patterns.

# 🌍 Human Development and Inequality

Countries with Very High Human Development exhibit the lowest median income inequality and the most consistent distributions.

Low, Medium, and High development groups show higher inequality and greater variability, particularly the Medium group, which contains several extreme outliers.

The results indicate a negative relationship between development level and income inequality, where higher human development is generally associated with lower and more stable inequality.

🇮🇳 India in Global Context

India’s income inequality increased slightly from around 19 to 19.3 between 2010 and 2021, showing minimal improvement over time.

During the same period, the global average inequality declined from approximately 24 to 22.8, indicating global progress toward more equitable income distribution.

The narrowing gap between India and the global average is therefore driven primarily by global improvement rather than domestic reduction in inequality.

This contrast highlights that economic growth in India has not translated into meaningful reductions in income inequality.

# 🚺 Gender Inequality: A Critical Insight

While the dataset captures income inequality at an aggregate level, the observed patterns strongly reflect structural gender-based disparities, with women disproportionately affected across regions and development levels.

Continents and development groups exhibiting higher income inequality—particularly Africa, parts of Asia, and low to medium human development countries—are also regions where women face greater economic exclusion, wage gaps, and limited access to stable employment.

Even in regions showing declining overall inequality, such as Europe and some high-development countries, gender pay gaps persist, indicating that reductions in aggregate inequality do not automatically translate into gender equity.

The stability of inequality trends in countries like India, despite global improvement, suggests that women continue to face systemic barriers including occupational segregation, unpaid care burdens, and lower participation in high-income sectors.

High outliers in inequality distributions often coincide with economies where women are over-represented in informal or low-paying work, reinforcing gendered income gaps.

These findings indicate that gender inequality is not a secondary effect, but a core contributor to income inequality, and that meaningful reductions in inequality require gender-responsive economic policies.

Addressing income inequality therefore demands targeted interventions such as pay equity enforcement, improved access to education and financial services for women, and stronger social protection systems that recognize unpaid and informal labor.

# ⚠️ Limitations

Inequality reporting standards vary across countries and years.

Gender-specific income data is not available for all countries, limiting direct measurement of gender wage gaps.

The analysis is descriptive and does not establish causal relationships.

# 👤 Author

* Maahi 
