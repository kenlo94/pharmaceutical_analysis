# Analyzing Anti-Cancer Medications in Mice using Jupyter Notebook, Pandas, & Matplotlib

## Resources
Data sources: Mouse_metadata.csv, Study_results.csv

Software: Python 3.9.7; Jupyter Notebook 6.4.11; pandas 1.3.5; Matplotlib 3.5.1

## Project Objectives
### Use the data provided to compare the effectiveness of the drug, *Capomulin*, against the other treatment regimens when treating squamous cell carcinoma (SCC), a commonly occuring form of skin cancer.

Tasks include:
1. Preparing and cleaning data by merging the two datasets and dropping duplicate mice ID's
2. Generating summary statistics for each drug regimen
3. Creating visualizations such as bar charts, pie charts, line charts, and scatter plots
4. Calculating quartiles, finding outliers, and creating a box plot
5. Calculating correlation and linear regression between the selected drug regimen, ***Capomulin***, and the average tumor volume

## Results & Analysis
![Screenshot](Images/clean_data.PNG)

The table above displays the clean dataframe after merging the two datasets and dropping duplicate mouse ID's. There are 248 unique mouse ID's in the cleaned dataset, with metastatic sites ranging from 0-4, ages ranging from 1-24 months, and weights ranging from 15-30 grams.


![Screenshot](Images/summary_statistics.PNG)

The table above displays the summary statistics for each drug regimen. ***Ramicane*** is the leading drug regimen across all category statistics with the smallest average tumor volume, median tumor volume, tumor volume variance, tumor volume standard deviation, and tumor volume standard error of mean.

![Screenshot](Images/bar.PNG)

The bar chart above represents the count of mice that were tested for each drug regimen, with ***Capomulin*** and ***Ramicane*** having the highest number of test subjects, both exceeding 200 mice each.

![Screenshot](Images/pie.PNG)

The pie chart above depicts the distribution of male and female mice that were tested, showing an almost equal split with roughly 50% for each gender.

![Screenshot](Images/outliers.PNG)

The image above shows the results of my calculations aimed at identifying outliers for the four drug regimens. The results indicate that there is only one outlier for ***Infubinol***, which falls below the lower bound.

![Screenshot](Images/boxplot.PNG)

The boxplot above displays the upper and lower bounds and the single outlier I found in my previous calculations for the four drug regimens.

![Screenshot](Images/line.PNG)

The line chart depicted above shows the decrease in tumor volume for mouse "l509" treated with the drug ***Capomulin*** over a period of 40+ days.

![Screenshot](Images/scatter.PNG)

The scatter plot above depicts the relationship between the average tumor volume and mouse weight for the drug ***Capomulin***.

![Screenshot](Images/correlation.PNG)

Above is an image showing the correlation coefficient (0.84) between mouse weight and average tumor volume for the drug ***Capomulin***. It also displays the linear regression model we calculated to predict the average tumor volume based on the weight of the mouse.

## Drawing Insights

- From the line chart I generated, we can see that ***Capomulin*** can be an effective drug regimen to treat squamous cell carcinoma (SCC). However, more data needs to be visualized as this was done for only one mouse in the dataset.
- With a correlation coefficient of 0.84, this indicates a strong positive relationship between mouse weight and average tumor volume.
- The regression equation that was calculated allows us to predict the average tumor volume for a given weight of a mouse on the ***Capomulin*** regminen. However, it's important to keep in mind that the relationship between mouse weight and tumor volume may not be the same for all mice or all treatments, and the regression equation should be used with caution and validated with additional data.

---
Return to the [Homepage](https://kenlo94.github.io/)
