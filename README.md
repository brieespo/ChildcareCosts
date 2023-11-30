## National Childcare Costs 2018



#This Project Includes

1. Read TWO data files:

Two csv files, childcare_costs.csv and counties.csv, from the Department of Labor National Database of Childcare Prices: https://www.dol.gov/agencies/wb/topics/featured-childcare

2.) Clean your data and perform a pandas merge with your two data sets, then calculate some new values based on the new data set.  

I cleaned the data by eliminating some of the unnecessary columns and by renaming the very abbreviated column names with clearer titles for my project. I then merged the two dataframes on the "county_fips_code" column and eliminated outliers in the data after doing a histogram.

3.) Make 3 matplotlib or seaborn (or another plotting library) visualizations to display your data.

I created a histogram of the full data for female employment rate's for women with children under the age of 6 to determine the validity of certain outlying data results and created a bar chart using seaborn for the top 20 counties/states for the same category.

4.) Build a custom data dictionary and include it either in your README or as a separate document. 

I created a data dictionary (below.)


5.) Annotate your code with markdown cells in Jupyter Notebook, write clear code comments, and have a well-written README.md.

I annotated my code each step of the way in Jupyter Notebook, showing my process and reasoning. 

