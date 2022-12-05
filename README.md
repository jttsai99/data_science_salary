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
 \begin{itemize}
    \item Qualitative figures: scatterplot matrix, hist. of *avg_salary* and their transformed versions, boxplot for *avg_salary*
    \item Another line with a 'sub bullet'.
  \end{itemize}



