# Adult Income

## Repository Navigation
<pre>
Technical Notebook         : <a href=https://github.com/Debanjan-C/Adult_Income/blob/main/Notebook/Technical%20Notebook.ipynb>Technical Notebook</a>
Code                       : <a href=https://github.com/Debanjan-C/Adult_Income/blob/main/Notebook/Code.ipynb>Code</a>
Data                       : <a href=https://github.com/Debanjan-C/Adult_Income/blob/main/Data/adult.csv>Data</a>
Data Web                   : <a href=https://www.kaggle.com/uciml/adult-census-income>Data Web</a>
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
According to an article in the US News - A World report, they were evaluating how certain indidividuals did not fill out paper work for a long time and numbers in census were misled. In the year of 2018, an inspecotr general in Rhode Island released a report where the census dept would go to the homes of individuals who had not filled out their forms in a long while. (US News) Another intersting information comes from Federal News Network. According to an article in Federal News Network, the legislatures in the house of representatives were planning to pass a bill where you would have about $11,000 in fines in you lie or spread any form of misinformation in the census. This is scary. It is one of the other reasons that I also wanted to do this project. A question came to my mind about why one would try lying on a census and was wondering how they would figure out. Therefore, this dataset came to my mind as it was about census and it would help me get an idea of how to cross check when someone may be lying. (Federal News Network). These two are the main sources of motivation behind why I wanted to work on this project. After seeing this information, I noticed this dataset and it contained information about individuals on a census, there data and the salary ranges of whether it is greater than 50K or less than or equal to 50K salary. The government has recently mentioned that they will provide benefits to individuals who may ahve a salary less than 50K. My colleagues have provided me with a dataset with 32561 rows or that many individuals and 15 columns initailly. The data contains information about an individuals age, education, occupation, race, gender, capital gain, capital loss, hours per week that they work and income (target). The targer data tells us if the salry is in the specific ranges as mentioned above. My role in the company as a data scientist is to verify whether the the salary information is correct and if it is accurate or if someone is bluffing on a specific income for benefits. Initially, I conducted data cleaning to check for missing values and marked them as unknowwn as some individuals may have been unemployed in terms of their job or profession and they may not have a salary. Therefore, I added that step. The next step was where I removed a column as it was redundant and the categorical counting of education categories started from one and not 0 which would have affected us during modelling. Further, I conducted Exploratory Data Analysis to evaluate the dataset further. Next, I conducted feature engineering to convert all letters and other non-numeric categorical values into numeric values as models would use only numeric values. I used label encoding for that. Following that step, I would scale the datasets to ensure that they all are within the same range. After those steps, I developed a logistic regression model, decision tree and random forest models where I split the data into testing and training sets and tested the x values with the targets. In order to verify the accuracy of the models, I used cross validation to check for the mean and standard devation to verify the model accuracy. The cross validation would show the mean and standard devation and that gives an idea of whether the accuracy amount may be correct or not. he logistic regression is the main calssification model, but decision tree uses a tree based branching approach and the random forest uses resampling techniques for each of the data and creates variations of the data to show the score.Following that, I used a confusion matrix and found the accruacy, precision and recall scores for each of the models. I compared the model and the Random forest came to be the best. In order to finetune the model, I removed some of the main outliers from specific columns and was able to improve scores once again. The removal of outliers also showed the random forest as highest in scores. One common thing all models showed was that the true negatives were highest, but in all cases the true positive was larger than the true negative when we went to removing outliers in the confusion matrix.

## Goals

### Business Goals
For this project, I am a Data Scientist in the US Census bureau. Recently, the government has announced a special package or benefit for all individuals who are earning less than 50K in temrs of salary. My colleagues collected the data of different individuals who are over the age of 16 and my job is to double check whether their claims on salary are accurate based on all other types of data that they are providing or if they are bluffing in order to get the benefits. There are many details, but the main ones collected from individuals are their age, education, occupation, race, gender, capital gain, capital loss, hours per week that they work and income (Which was used) as a target. Our dataset has about 32561 rows or that many individuals and 15 columns initailly. I removed one of them as it showed categorical labels for individuals and there education, but it did not start from 0 and started from one which would cause trouble when modelling. The target value has details about whether an individuals salary was greater than or less than/equal to 50K. My goal was to verify the accuracy about whether the salary range of aspecific individual was correct or seemed fishy. The dataset will give us an understading of capital gains or loss an individual had in terms of salary and I also noticed specific races where in higher propertion than the others, so many outliers came into existence. I used different types of methods and technologies like data cleaning, feature engineering and exploratory data analysis to undersand the data in more details and evaluate where to be alert or pay attention. Following that, I use logistic regression, decision trees and random forest methods to verify if the income category mentione was correct or not. I compared all three models and realized that one is relatively better than the other one. In order to help enhance and improve the model in the fine tuning step, I decided to remove major outliers in the data columns or features that may have been playing a role with pulling the overall score down. After removing the outliers, I realized that the the accuracy, precision and the recall scores rose by a specfic amount. I also noticed that the random forest model showed the best scores in terms of the accuracy.

### Technical or Machine Learning Goals:
The corresponding machine learning problem is to use Logistic Regression, Decision tree and Random Forest model to evaluate which model shows the best accuracy results and will help us determine the accurac y behind whether all the feature match the target dataset. Our main goal here is to develop a model that is higher than an accuracy score of 75%. That was what our accuracy sscore was when we divided the number of individuals who earned more than 50K salary with the total number of indidivuals who earned greater or less than euqal to a 50K salary.


## Motivation and Background
- According to an article in the US News - A World report, they are evaluating how indidividuals have not filled out paper works for a long time and the numbers may have been misled. Somewhere aorund 2018, an inspecotr general in Rhode Island released a report where the census goers would go to the homes of individuals who had not filled out their forms in a long while. (US News) This was one of my main motivations on why I wanted to look into the project. One misinformation could cause a lot of trouble in the modellings and leagal trouble also. 
- According to an article in Federal News Network, the legislatures in the house were planning to apss a bill wher eyou would have about $11,000 in fines in you lie or spread any form of misinformation in the census. This is scary and I also wanted to do this project, because this question came to my mind about why one would try lying on a census and was wondering how they would figure out. Therefore, this dataset came to my mind as it was about census and it would help me get an idea of how to cross check when someone may be lying. (Federal Newws Network).

## Data

- The dataset used for this project was found at 
https://www.kaggle.com/uciml/adult-census-income.
- The dataset was inspired by the intial data in the UCI website: 
http://archive.ics.uci.edu/ml/datasets/Adult
- This dataset contains information that was extracted from a census in a past year. The individuals are above age 16 and the dataset contains information about individuals, their work type (private company employee, government employee, etc), their education levels, marital status, occupation (like technical field, farmer, etc), their race and many more information. The dataset then shows us the income column as the target column and that shows us if an individuals salary is above or below $50K. 

### Data Dictionary
Our dataset has about 32561 rows or that many individuals and 15 columns initailly. I removed one of them as it showed categorical labels for individuals and there education, but it did not start from 0 and started from one which would cause trouble when modelling. So 14 columns
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
- https://www.usnews.com/news/us/articles/2020-02-03/report-census-hasnt-tested-tasks-to-catch-people-who-lie
- https://federalnewsnetwork.com/federal-newscast/2020/03/spreading-false-information-about-2020-census-could-land-you-in-jail-if-new-bill-becomes-law/
</pre>
