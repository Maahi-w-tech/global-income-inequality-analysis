# global-income-inequality-analysis
## Overview: 
  Income inequality is a global issue reflecting the uneven distribution of wealth within and between countries. Developed nations exhibit varying income levels due to economic policies and labor market dynamics, often resulting in Gini coefficients ranging between 0.3 and 0.4. In contrast, many developing nations experience significantly higher income disparities due to limited access to education, healthcare, and employment opportunities, with Gini coefficients frequently exceeding 0.4.

Such inequality exacerbates poverty cycles, fuels social tensions, and limits upward mobility. Beyond social consequences, income inequality hampers long-term economic growth and weakens social cohesion. Addressing these challenges requires comprehensive policy interventions, including progressive taxation, inclusive labor policies, and equitable distribution of resources. This project aims to explore global income inequality trends through data-driven analysis and visual storytelling.

###  Dataset
- Source: Kaggle
- Time Period: 2010 – 2021
- Scope: Global (multiple countries and regions)

**Dataset Description**  
This dataset contains historical indicators related to income inequality across countries worldwide. It includes demographic, geographic, and development-based classifications to support comparative analysis.

**Key Features**
- ISO3 Country Code  
- Country  
- Continent  
- Hemisphere  
- Human Development Groups  
- UNDP Developing Regions  
- HDI Rank (2021)  
- Income Inequality Indicators (2010–2021)

**🛠️ Data Cleaning & Preparation**
*1. Column Selection*

The dataset contains demographic and classification variables along with year-wise income inequality indicators. Columns starting with inequality_in_income_ were programmatically selected to identify all income inequality variables, avoiding hard-coded column names and ensuring robustness to dataset updates.

*2. Handling Missing Numerical Values*

Income inequality data contained missing values for certain countries and years. A country-wise median imputation strategy was applied directly to the raw dataset.

Missing values for each country were filled using that country’s median inequality value across available years.

The median was chosen over the mean due to its robustness against extreme values and outliers common in inequality data.

This approach preserves country-specific inequality patterns and avoids distortion from global or regional averages.

Countries with no reported income inequality values for any year between 2010 and 2021 were identified, documented, and excluded from further analysis, as meaningful imputation was not possible in such cases.

*3. Handling Missing Categorical Data*

The undp_developing_regions variable contained missing values due to unavailable or unassigned UNDP classifications. Rather than excluding these countries or inferring categories, missing values were labeled as “Not Classified” to maintain transparency and preserve dataset completeness.

*4. Data Reshaping*

After cleaning, the dataset was reshaped from wide format (separate columns for each year) into long format using a single year column and a corresponding income_inequality value.

This structure enables:

Time-series analysis

Cross-country comparisons

Grouped analysis by region and development category

Compatibility with visualization libraries such as Seaborn

The year variable was extracted from column names and converted to an integer type to support sorting and temporal analysis.

*5. Final Dataset State*

The final dataset represents income inequality values for multiple countries across the period 2010–2021 in an analysis-ready long format. All data preparation decisions were made with an emphasis on methodological soundness, transparency, and reproducibility.
