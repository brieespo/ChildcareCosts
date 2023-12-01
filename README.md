# National Childcare Costs 2018

## Introduction and Overview
For this project I looked at the Department of Labor's National Database of Childcare Prices. The data included a wide range of data about employment rates across genders for both non-parents and parents with children of specific ages, as well as childcare costs (both in-home and center-based) further broken down by age of the child. The DOL's data assigned county codes for each entry, which I cross references with a master county code list to get the county and state name for each entry to better contextualize the data.

I looked for correlations between the cost of center-based childcare and the employment rate of women with children under the age of 6. I hypothesized that the more expensive center-based childcare was in a county, the lower the rate of employent for young mothers. Childcare cost is a huge barrier for parents, especially women who are often the default carer for young children due to discrepency between male and female pay for the same positions as well as factors such as loss of employment due to lack of adequate maternity leave and breastfeeding/pumping accommodations. Ultimately, this project was an exploratory analysis, but with such a rich data source I am sure I will be able to expand upon my current findings. 

## Data Dictionary 
|Column|Description|
|------|------|
|county_fips_code|number that uniquely identifies the county in a state|
|county_name|full name of the county|
|state_name|full name of the state in which the county is found|
|state_abbreviation|two-letter state abbreviation|
|study_year|year the data collection began for the market rate survey|
|unemployed_20to64|unemployment rate of the population aged 20 to 64 years old|
|fem_unemployed_20to64|unemployment rate of the female population aged 20 to 64 years old|
|male_unemployed_20to64|unemployment rate of the male population aged 20 to 64 years old|
|fem_labor_participation_childunder6|labor force participation rate of the female population aged 20 to 64 years old who have children under 6 years old|
|fem_labor_participation_child6to17|labor force participation rate of the female population aged 20 to 64 years old who have children between 6 and 17 years old|
|fem_labor_participation_childunder6and17|labor force participation rate of the female population aged 20 to 64 years old who have children under 6 years old and between 6 and 17 years old|
|fem_labor_participation|labor force participation rate of the female population aged 20 to 64 years old|
|male_labor_participation|labor force participation rate of the male population aged 20 to 64 years old|
|povery_rate_families|poverty rate for families|
|median_household_income_2018|median household income expressed in 2018 dollars|
|median_earn_2018|median earnings expressed in 2018 dollars|
|female_median_earn_2018|median earnings for females expressed in 2018 dollars|
|male_median_earn_2018|median earnings for males expressed in 2018|
|total_pop|total population for the given county|
|weekly_med_center_cost|weekly, full-time median price charged for Center-Based Care|
|weekly_med_famcare_cost|weekly, full-time median price charged for Family Childcare (at home care)|
|weekly_med_center_cost_infant|weekly, full-time median price charged for Center-based Care for infants (ages 0 through 23 months)|
|weekly_med_center_cost_toddler|weekly, full-time median price charged for Center-based Care for toddlers (ages 24 through 35 months)|
|weekly_med_center_cost_preschool|weekly, full-time median price charged for Center-based Care for preschoolers (ages 36 through 54 months)|
|weekly_med_famcare_infant|weekly, full-time median price charged for Family Childcare for infants|
|weekly_med_famcare_toddler|weekly, full-time median price charged for Family Childcare for toddlers|
|weekly_med_famcare_preschool|weekly, full-time median price charged for Family Childcare for preschoolers|

### Instructions and Requirements
1. Clone the Repo.
2. Optionally, you can download anaconda [here](https://www.anaconda.com/download)
3. Review the requirements.txt file included to view the packages I had installed.
4. Minimum package requirements are pandas, numpy, matplotlib.pyplot, and seaborn.
5. If you wish, activate a virtual environment using "python3 -m venv venv" and install the required packages. 
6. Download the .csv files and the .ipynb file.
7. Run Jupyter Notebook from the terminal by typing "Jupyter Notebook"
8. You may now Run All or run each cell in the notebook individually (in order) as you interact with the notebook.

### Capstone Requirements Met

#### 1.) Read TWO data files:
Two csv files, childcare_costs.csv and counties.csv, obtained from the Department of Labor National Database of Childcare Prices: https://www.dol.gov/agencies/wb/topics/featured-childcare

#### 2.) Clean your data and perform a pandas merge with your two data sets, then calculate some new values based on the new data set.

I cleaned the data by eliminating some of the unnecessary columns and by renaming the very abbreviated column names with clearer titles for my project. I then merged the two dataframes on the "county_fips_code" column and eliminated outliers in the data after doing a histogram.

#### 3.) Make 3 matplotlib or seaborn (or another plotting library) visualizations to display your data.

I created a histogram of the full data for female employment rate's for women with children under the age of 6 to determine the validity of certain outlying data results and created bar charts using seaborn analyzing the top 20 counties/states in categories of interest.

#### 4.) Build a custom data dictionary and include it either in your README or as a separate document.

I created a data dictionary for my renamed and edited columns in my merged table. 

#### 5.) Annotate your code with markdown cells in Jupyter Notebook, write clear code comments, and have a well-written README.md.

I annotated my code each step of the way in Jupyter Notebook, showing my process and reasoning.
