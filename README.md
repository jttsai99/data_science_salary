# data_science_salary
Analysis of Glassdoor data on data science salaries using advanced regression


## playground.ipynb
Initial look at data, discover what columns to keep.

## data_cleaning.ipynb
Preprocess data and export data_clean.csv
-Subsetted (data_raw.csv) and exported it to data_subset.csv.\
-Read in data_subset.csv and continued to clean the data:\
-Dropped duplicate entries\
-Created *visual_software*, *ML_software*, *in_CA, seniority_by_title* columns\
-Reconstructed *degree* column \
-Process error values and removed NA.\
-Exported data as data_clean.csv


## EDA.ipynb
File consist of all exploratory data analysis figures and export them to figures folder.
-Read in data_clean.csv\
-The following plots were created:
- Qualitative figures: scatterplot matrix, hist. of *avg_salary* and their transformed versions, boxplot for *avg_salary*
- Quantitative figures: boxplots of company size, degree, in california, senior status, skills. pie chart of company size and degree.

## Linear_regression.Rmd & Linear_regression.html
Linear regression method steps:\
1.) Fit first order model with full data and check model diagnostics. (suggested boxcox transformation on response variable)\
2.) Refit first order model with sqrt(Y) full data. \
3.) Use stepAIC to find a better reduced model.

4.) Fit interaction model with full data and check model diagnostics. (suggested boxcox transformation on response variable)\
5.) Refit interaction order model with sqrt(Y) full data. \
6.) Use stepAIC to find a better reduced model.\
7.) Compared AIC selected first order model and AIC selected interaction model (Proceed with AIC selected interaction model)\
8.) Outlier analysis with selected model 
- Identified outlying in Y (Bonferroni outlier test) but not influential via Cook's Distance.
- Identified outlying in X (leverage) and removed influential cases via Cook's Distance. 

9.) Refit AIC selected interaction model with data without influential outliers\
10.) Calculate Press_p and confidence interval of the final model

## logistic_regression.ipynb
Logistic regression method for better predictions. 



