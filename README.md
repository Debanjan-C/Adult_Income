# Adult Income

## Repository Navigation
<pre>
Technical Notebook         : <a href=>Technical Notebook</a>
Code                       : <a href=>Code</a>
Data                       : <a href=>Data</a>
Data Web                   : <a href=>Data Web</a>
</pre>

## Table of Contents
[Repository Navigation](#repository-navigation) -
[Overview](#overview) -
[Business Goals](#business-goals) -
[Motivation and Background](#motivation-and-background) -
[Data](#data) 
[Contributor](#contributor)
[Software Requirements - Packages used](#software-requirements--packages-used) -
[Reference and contribution](#reference-and-contribution)

## Overview


## Business Goals


**Technical Goals:**


## Motivation and Background


## Data

The dataset used for this project was found at 
https://www.kaggle.com/uciml/adult-census-income.
The dataset was inspired by the intial data in the UCI website: 
http://archive.ics.uci.edu/ml/datasets/Adult
This dataset contains information that was extracted from a census in a past year. The individuals are above age 16 and the dataset contains information about individuals, their work type (private company employee, government employee, etc), their education levels, marital status, occupation (like technical field, farmer, etc), their race and many more information. The dataset then shows us the income column as the target column and that shows us if an individuals salary is above or below $50K. 

### Data Dictionary

- age: (int data type), numerical data. It contains each of the individuals - -- workclass: (string/object data type), cateogorical data. It contains the details of what type of work type each individual has liek private job, government job, etc. 
- fnlwgt: (int data type), numerical data. This is a final weight ranking section that is determined by the amount of folks who are over 16, Hispanic and they evaluate the weight by the race, age and sex. 
- education: (string/object data type), cateogorical data. It contains the education completed levels of each of the individuals int he census. Some have completed up to high school, some have gone to college, some are still in school.
- education-num: (int data type), categorical data. This column contains a value reprsenting the education level of each individual. However, we dropped this column as it is redundant and the categorical count does not start from 0 and starts from 1. It could affect the model unless every categorical value starts from 0 when it is converted to numeric value.
- marital-status: (int data type), categorical data. It contains information abput thee marital status of individuals like unmarried, married, divorce, etc.
- occupation: (string/object data type), categorical data. It contains information about what type of job or roles each individual has like manager, executive, etc. 
- relationship: (string/object data type), categorical data. It contains detials about the individuals relationship status like is he a wife, a husband, has a child, unmarried, etc. 
- race: (string/object data type), categorical data. It contains details about the individuals ethnicity - White, Black, Hispanic, etc.
- sex: (renamed it to gender), categorical data. It mentions whether an individual is a mail or female.
- capital-gain: (int data type), numeric data. This column contains the capital gain amount that an individual had. If they had none then it says 0. 
- capital-loss: (int data type), numeric data. This column contains the capital loss amount that an individual had. If they had none then it says 0. 
- hours-per-week: (int data type), numeric data. This column contains the amount of week each individual worked. 
- native-country: (string/object data type), categorical data. It tells us each indiviuals native country.
- income: (string/ object data type), categorical data. It tells us whether an individuals salary is greater than or less than and equal to 50K dollar salary. This is our target value. 

##  Contributor
<pre>
Contributer  : <a href=https://github.com/Debanjan-C>Debanjan Chowdhury</a>
</pre>

##  Software Requirements - Packages used
<pre>
Languages    : Python
Tools/IDE    : Anaconda, Jupyter Notebook
Libraries    : pandas, numpy, matplotlib, seaborn, scikit learn
</pre>

<pre>
Last Updated : December 2020
</pre>

## Reference and contribution
<pre>
- Dataset: https://www.kaggle.com/uciml/adult-census-income
- Dataset inspired by: http://archive.ics.uci.edu/ml/datasets/Adult
</pre>
