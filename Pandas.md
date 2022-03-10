<p align="center">
<a href="https://pandas.pydata.org/"><img src="https://pandas.pydata.org/pandas-docs/stable/_static/pandas.svg" alt="Pandas" width="500"></a>
</p>

# Introduction to Pandas

Pandas is a open-source library built using NumPy specifically for data analysis purpose. It is a Python package that offers various data manipulation, visualisation, building machine learning models etc. Pandas is fast and it has a high performance and productivity for users.
Since pandas is python package to know more about it click [here](https://docs.python.org/3/).

# Why to use Pandas?

- It allows us to analyze big data and make conclusions based on statistical theories.
- It can be used to clean messy data sets, and make them readable and relevant.
- Fast and efficient DataFrame object with default and customized indexing.
- High performance merging and joining of data.
- Time Series functionality.

## Installation

Installing pandas can be tricky for new or inexperience users. The easiest way to install pandas is to install it as part of the [Anaconda](https://docs.continuum.io/anaconda/) distribution, a cross platform distribution for users to do data analysis and other computing works.

### Installing Pandas with Anaconda

The simplest way to install pandas, but also the most popular and useful packages  is with Anaconda, a cross-platform (Linux, macOS, Windows) Python. After downloading and running the installer, the user will have access to pandas and the rest of the SciPy stack without needing to install anything else. User can download Aanconda navigator by clicking [here](https://docs.continuum.io/anaconda/install/).

### Installing Pandas with PyPI
[PyPI](https://pypi.org/project/pandas/) is Python Package Index in short PyPI is the official third party software repository for Python
```sh
pip install pandas
```

## Pandas DataFrame and Series

`Series` -Pandas Series is a one-dimensional labeled array capable of holding data of any type (integer, string, float, python objects, etc.). The axis labels are collectively called index.

`DataFrames` - A Data frame is a two-dimensional data structure, i.e.,
data is aligned in a tabular fashion in rows and columns.

> Series can only contain single list with index, whereas dataframe can be made of more than one series or we can say that a dataframe is a collection of series that can be used to analyse the data.

### Pandas Series 
```sh
# Creating a pandas series
s = pd.Series([2, 4, 5, 6, 9])
print(s)
print(type(s))
```
[![Series](https://github.com/snozh5/temp/blob/main/Pictures/Series.PNG?raw=true)](https://github.com/snozh5/temp/blob/main/Pictures/Series.PNG)

### Pandas DataFrame
Creating a DataFrame using dictionary in python. Python dictionary is an unordered collection of items. Each item of a dictionary has a key and value pair seperated by a ':'. 
```sh
#Dictionary
person = {"first_name":['Harry',"James"],
         "last_name" : ['Potter','Witch'],
         "email" : ['H@harray.com',"J@james.com"]}
print("person dictionary : ""\n",person)

#converting dictionary to DataFrame
df = pd.DataFrame(person)
print("DataFrame :""\n", df)
```
[![Dictionary](https://github.com/snozh5/temp/blob/main/Pictures/Dictionary.PNG?raw=true)](https://github.com/snozh5/temp/blob/main/Pictures/Dictionary.PNG)

Creating a DataFrame by importing external files like excel, csv etc.
```sh
#From Excel file
pd.read_excel('file.xlsx' )
df.to_excel('dir/myDataFrame.xslx' ,sheet_name='Sheet1' )

#From csv file
df=pd.read_csv('datasets_1026_1855_My Uber Drives - 2016.csv')
print(df)
```
[![DataFrame](https://github.com/snozh5/temp/blob/main/Pictures/DataFrame%20csv.PNG?raw=true)](https://github.com/snozh5/temp/blob/main/Pictures/DataFrame%20csv.PNG)

> Pro-tip  for settings
```sh
#pd.set_option()
#display just 85 columns
pd.set_option('display.max_columns',85)
```
In order to view the first few rows of the DataFrame we need to use the head() function also to view the last few rows of the DataFrame we need to use the tail() function. 
```sh
#From the top first 5 rows
df.head()
```
[![DataFrame head](https://github.com/snozh5/temp/blob/main/Pictures/head.PNG?raw=true)](https://github.com/snozh5/temp/blob/main/Pictures/head.PNG)
```sh
#From the bottom last 5 rows
df.tail()
```
[![DataFrame tail](https://github.com/snozh5/temp/blob/main/Pictures/tail.PNG?raw=true)](https://github.com/snozh5/temp/blob/main/Pictures/tail.PNG)

## Accessing
`Accessing` - Accessing pandas dataframe columns, rows, and cells. At this point you know how to load CSV data in Python.
```sh
#For accessing columns in DataFrame

#for sigle column access
print(df['CATEGORY*'])

#for multiple column access use list
print(df[['CATEGORY*','MILES*']])
```
[![accessing](https://github.com/snozh5/temp/blob/main/Pictures/aceessing%20column.PNG?raw=true)](https://github.com/snozh5/temp/blob/main/Pictures/aceessing%20column.PNG)

> #TIP - for accessing columns names
```sh
# To print the column name in the dataframe
print(df.columns)
```

[![column](https://github.com/snozh5/temp/blob/main/Pictures/column.PNG?raw=true)](https://github.com/snozh5/temp/blob/main/Pictures/column.PNG)

In order to select rows in the DataFrame we need to use the .iloc or .loc also know as indexing in pandas simply selecting particular rows from a DataFrame. It is also know as Subset Selection. 
- Selecting data by row numbers (. iloc)
- Selecting data by label or by a conditional statement (. loc)
```sh
#accessing rows in DataFrame
#by row numbers
#using df.iloc(index)
print("rows 0 and 1" , df.iloc[[0,1]])
```
[![iloc rows](https://github.com/snozh5/temp/blob/main/Pictures/iloc%20rows.PNG?raw=true)](https://github.com/snozh5/temp/blob/main/Pictures/iloc%20rows.PNG)

To access data using both rows and columns and the syntax looks like `df.iloc[row_index,column_index]`
```sh
#for row 0,1 and column 1,2
print(df.iloc[[0,1] , [1,2]])
```
[![iloc rows and colm](https://github.com/snozh5/temp/blob/main/Pictures/iloc%20rows%20and%20col.PNG?raw=true)](https://github.com/snozh5/temp/blob/main/Pictures/iloc%20rows%20and%20col.PNG)

```sh
#using .loc
#for same row 0,1 and 1,2 but accessing via labels
print(df.loc[[0,1],["END_DATE*","CATEGORY*"]])
```
[![loc rows and colm](https://github.com/snozh5/temp/blob/main/Pictures/loc%20rows%20and%20col.PNG?raw=true)](https://github.com/snozh5/temp/blob/main/Pictures/loc%20rows%20and%20col.PNG)

```sh
#tip - for collecting value counts information
#df['co_name'].value_counts()
print(df['CATEGORY*'].value_counts())
```
[![count](https://github.com/snozh5/temp/blob/main/Pictures/count.PNG?raw=true)](https://github.com/snozh5/temp/blob/main/Pictures/count.PNG)

## Reshaping
Pandas have got a function name melt() that can be used to reshape a DataFrame from wide to long where one or more columns are used as an identofier.
```sh
#Gather columns into rows
reshaped_data = pd.melt(df)
print(reshaped_data)
```
[![reshape](https://github.com/snozh5/temp/blob/main/Pictures/reshape.PNG?raw=true)](https://github.com/snozh5/temp/blob/main/Pictures/reshape.PNG)

## Sorting
In order to sort the data frame in pandas, function sort_values() is used. Pandas sort_values() can sort the data frame in Ascending or Descending order.
```sh
#sort values according to End Date
df.sort_values('END_DATE*')

#sort values in descending orders
df.sort_values('END_DATE*',ascending=False)
```
[![sort](https://github.com/snozh5/temp/blob/main/Pictures/sort.PNG?raw=true)](https://github.com/snozh5/temp/blob/main/Pictures/sort.PNG)

## Renaming and droping columns
```sh
#renaming the CATEGORY* name to C
df.rename(columns = {"CATEGORY*" : "C"},inplace=True)
print(df["C"])

#drop column C
df.drop(columns = ["C"])
```
[![rename](https://github.com/snozh5/temp/blob/main/Pictures/rename.PNG?raw=true)](https://github.com/snozh5/temp/blob/main/Pictures/rename.PNG)

> #tip - use inplace=True only in order to save the changes

## Summarize Data
To summarize data we can use inbuilt functions like shape, info, describe. 
```sh
#to get information about DataFrame
#shape is an attribute
print("Shape: ",df.shape)

#info is a method
print("information: ",df.info())

#to describe the DataFrame
print("Describe : ",df.describe())
```
[![inspect](https://github.com/snozh5/temp/blob/main/Pictures/inspect.PNG?raw=true)](https://github.com/snozh5/temp/blob/main/Pictures/inspect.PNG)

## Handling missing values in the DataFrame
`df.dropna()`: Drop rows with any column having NA/null data.
`df.fillna(value)`: Replace all NA/null data with value.
```sh
#drop NA/null values
df.dropna()

#replace NA/null values to 1
df.fillna(1)
```
[![drop](https://github.com/snozh5/temp/blob/main/Pictures/drop.PNG?raw=true)](https://github.com/snozh5/temp/blob/main/Pictures/drop.PNG)

## Filtering
In pandas DataFrame we can filter the dataset based on our needs. 
```sh
#for single filter
my_filter = (df['MILES*'] == 5.0)
print(df.loc[my_filter,'C'])
```
[![fil sig](https://github.com/snozh5/temp/blob/main/Pictures/filter%20single.PNG?raw=true)](https://github.com/snozh5/temp/blob/main/Pictures/filter%20single.PNG)

```sh
#& ! for multiple filters
my_filter2 = ((df['MILES*'] == 5.0) & (df["START*"] == "Fort Pierce"))
df.loc[my_filter2]
```
[![fil mul](https://github.com/snozh5/temp/blob/main/Pictures/filter%20multiple.PNG?raw=true)](https://github.com/snozh5/temp/blob/main/Pictures/filter%20multiple.PNG)

```sh
#is include 
my_filter3 = df["START*"].isin(["Fort Pierce","Gampaha"])     
df.loc[my_filter3]
```
[![is in](https://github.com/snozh5/temp/blob/main/Pictures/is%20in.PNG?raw=true)](https://github.com/snozh5/temp/blob/main/Pictures/is%20in.PNG)

## Grouping and Aggregating
In pandas DataFrame groupby() function is used to split the data into groups based on some criteria. Pandas objects can be split on any of their axes. The abstract definition of grouping is to provide a mapping of labels to group names. 

```sh
#grouping single column
df.groupby("START_DATE*").agg("mean").tail()
```
[![grp sig](https://github.com/snozh5/temp/blob/main/Pictures/grp%20sig.PNG?raw=true)](https://github.com/snozh5/temp/blob/main/Pictures/grp%20sig.PNG)

```sh
#group multiple and reset column names
res=df.groupby("START*").agg({"MILES*":["mean","sum"],"START_DATE*": ["min","max"]})
res.columns=["AVG_DISTANCE","TOTAL_DIST","EARLY","RECENT"]    
print(res)
```
[![grp mul](https://github.com/snozh5/temp/blob/main/Pictures/grp%20mul.PNG?raw=true)](https://github.com/snozh5/temp/blob/main/Pictures/grp%20mul.PNG)

### Sac operation
```sh
#applying grouping the data
#split-apply-combine operation(sac) known as grouping
#here split-start , apply_coloumn-miles , apply_operation-mean ,then it combine

df.groupby(["START*","STOP*"])["MILES*"].agg(["mean","sum"]).head()
```
[![sac](https://github.com/snozh5/temp/blob/main/Pictures/sac.PNG?raw=true)](https://github.com/snozh5/temp/blob/main/Pictures/sac.PNG)

```sh
#applying conditions(filter) and reset index
df1= df[( df["MILES*"]>10 ) & (df["START*"].isin(["Cary","New York"]))]
df1.reset_index(inplace=True,drop=True)
df1
```
[![cod](https://github.com/snozh5/temp/blob/main/Pictures/app%20cod.PNG?raw=true)](https://github.com/snozh5/temp/blob/main/Pictures/app%20cod.PNG)

### Converting Date and Time in Pandas
We can use the Datetime function to convert a Date column to date datatype same with time column as well.
```sh
#convert the date and time
import datetime
df["START_DATE*"]=pd.to_datetime(df["START_DATE*"],errors="coerce")
df.info()
```
[![date](https://github.com/snozh5/temp/blob/main/Pictures/dtype.PNG?raw=true)](https://github.com/snozh5/temp/blob/main/Pictures/dtype.PNG)





