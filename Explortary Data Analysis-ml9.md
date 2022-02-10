# Explortary Data Analysis
_Analyze and Summarize Data_

![](https://i.pinimg.com/474x/90/8a/7d/908a7dbe1cc473f9508df70ff869c056.jpg)

## What is it?
EDA or Explortary data analysis is an important concept for Machine Learning for ensuring the data analysis and processing before the training. Originally developed by American mathematician John Tukey in the 1970s, EDA techniques continue to be a widely used method in the data discovery process today.

Some points on EDA:
1. Suggest hypotheses about the causes of observed phenomena.
2. Assess assumptions on which statistical inference will be based.
3. Support the selection of appropriate statistical tools and techniques.
4. Provide a basis for further data collection through surveys or experiments.

Importance:
The main purpose of EDA is to help look at data before making any assumptions. It can help identify obvious errors, as well as better understand patterns within the data, detect outliers or anomalous events, 
find interesting relations among the variables.

Data scientists can use exploratory analysis to ensure the results they produce are valid and applicable to any desired business outcomes and goals. 
EDA also helps stakeholders by confirming they are asking the right questions. EDA can help answer questions about standard deviations, 
categorical variables, and confidence intervals. Once EDA is complete and insights are drawn, its features can then be used for more sophisticated data analysis or modeling, 
including machine learning.
Recognising patterns,spot anomalies,test hypothesis and to check assumptions with the help of summary statistics and graphical representations are the jest of EDA.

## Types of exploratory data analysis

Four types of EDA:
#### 1. Univariate graphical
When the data has only one variable, but done with graphical representations.

Non-graphical methods don’t provide a full picture of the data. Graphical methods are therefore required.

#### 2. Univariate non-graphical
When the data has only one variable, but done with non graphical representations.

This is simplest form of data analysis, where the data being analyzed consists of just one variable. Since it’s a single variable, it doesn’t deal with causes or relationships. The main purpose of univariate analysis is to describe the data and find patterns that exist within it.

#### 3. Multivariate nongraphical
When the data has multiple variable, but done with non graphical representations.

Multivariate data arises from more than one variable. Multivariate non-graphical EDA techniques generally show the relationship between two or more variables of the data through cross-tabulation or statistics.

#### 4. Multivariate graphical
When the data has multiple variable, but graphically representations.

Multivariate data uses graphics to display relationships between two or more sets of data. The most used graphic is a grouped bar plot or bar chart with each group representing one level of one of the variables and each bar within a group representing the levels of the other variable.

## Some Important components:-

Some important components od EDA that makes the analyisis efficient.
#### 1. Data selection/collection and quality
#### 2. Statistical analysis
#### 3. Quantitative and Qualitative Analysis
#### 4. Visualisation
#### 5. Summarized Story
Lets understand these components one by one.

## Data selection/collection and quality
Data selection/collection is most important if you are doing a independent project or a company project. The data quality is what decides the fate of the model as well as the practical applicability.
_If the dataset is biased_ or uneven displaying a different picture of the area rather than the _true picture_, then the resulting model will be biased and would be incapable for real life implimentation. Thus the focus is on data rather than the model. 

## Statistical analysis
The statistical parameters define and helps in analysis of the dataset mathematically.

- Estimate a Central Tendency for your Data
- Mean, Mode, Median
- Distribution
- Categories and frequencies
- Standard Deviation
- probability distribution

All such parameters are important for statistical testing.They provide insights on the range and distribution of dataset.

Here we can see *describe method* is used which provides the normal statistical insights on every attribute of the tabular dataset present here.
![](https://i.pinimg.com/564x/f4/23/c5/f423c5d38679a4f7f7c4e22c4e81a78b.jpg)

## Quantitative Test

Quantitative EDA techniques provide a more rigorous method of determining the key properties of a dataset. Two of the most important of these techniques are

-Interval estimation.
-Hypothesis testing.

Interval estimates are used to create a range of values within which a variable is likely to fall.

## Visualisation

This is again a main component that provides insights graphically provides more patterns for understanding the dataset.
General plots used are :
1. Histogram
```
sns.histplot(data = data, x  = 'platelets')
```
![](https://i.pinimg.com/originals/d6/3e/a6/d63ea676d6da5e50831590f423fa41ef.jpg) 

3. Scatter plot
```
sns.scatterplot(data = data, x  = 'age', y = 'platelets' )
```
![](https://i.pinimg.com/originals/7d/c3/21/7dc32143fb82ff445b76341311f14b65.jpg)

5. Bar Plot
```
sns.barplot(data = data.head(), x  = 'age', y = 'creatinine_phosphokinase' )
```
![](https://i.pinimg.com/originals/ae/b4/fa/aeb4fa3a4783679bbbc0315d24817732.jpg)

7. line plot
```
sns.lineplot(data = data, x  = 'age', y = 'creatinine_phosphokinase' )
```
![](https://i.pinimg.com/originals/24/01/9e/24019e4dc6f77b43d628a3941b9d9c22.jpg)

8. pie chart
```
plt.figure(figsize= (4,4))
percent = data['DEATH_EVENT'].value_counts()
val = percent.index
plt.pie(percent.values, labels = val,autopct="%1.1f%%")
plt.legend()
plt.show()
```
![](https://i.pinimg.com/originals/fb/32/c6/fb32c65ea22329297004995ef5e6e771.jpg)

10. box plot
11. Density plot
       ....and more

Some Libraries used:

1. matplotlib
2. seaborn
3. bokeh
4. ggplot
5. pygal
6. Plotly
7. geoplotlib
8. Gleam
9. missingno
10. Leather

All these libraries helps in providing space for graphical respresentations, to clarify things visually.

```
import matplotlib.pyplot as plt 
import seaborn as sns
```
This is two of the libraries which are imported with these alias.

```
sns.kdeplot(data = data, x = "age", hue = "DEATH_EVENT",
            common_norm = False, shade = True)
```
![](https://i.pinimg.com/564x/d2/25/71/d2257160d9f6d7a50153fd2dccf012b8.jpg)

This is the example with same dataset.

## Auto visualisation

There are some libraries for automating the visualisation process, some are:
1. Panda Profiling
2. Sweet Viz
3. Auto Viz
4. D - Tale

## Softwares or Tools for EDA:

1. JMP, an EDA package from SAS Institute.
2. KNIME, Konstanz Information Miner – Open-Source data exploration platform based on Eclipse.
3. Orange, an open-source data mining and machine learning software suite.

Some of the most common data science tools used to create an EDA include:

4. Python: An interpreted, object-oriented programming language with dynamic semantics. Its high-level, built-in data structures, 
combined with dynamic typing and dynamic binding, make it very attractive for rapid application development, 
as well as for use as a scripting or glue language to connect existing components together. Python and EDA can be used together to identify missing 
values in a data set, which is important so you can decide how to handle missing values for machine learning.
5. R: An open-source programming language and free software environment for statistical computing and graphics supported by the R 
Foundation for Statistical Computing. The R language is widely used among statisticians in data science in developing statistical observations 
and data analysis.

## Summarized Story

Data Analysis is all about story telling if you want to explain the results to someone don't have any experience with data analysis.

>the better the story, the better understanding of your customers or for those whom you want to present the data. 

Its all over the user, play with data wisely to get awesome results that can make difference.
