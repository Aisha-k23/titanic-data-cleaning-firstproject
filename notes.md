**print("xyz")** displays whatever is inside the brackets as text that the laptop will repeat
**shift + enter** runs the code

**import pandas as pd**: 
import pandas as pd means “load the Pandas library and give it the short name pd.”  
We do it because Python doesn’t load extra tools automatically—you import the ones you need, and Pandas is the main tool for working with tables, spreadsheets, and data analysis.

**df = pd.read_csv("name of text/file")
df.head()**
This tells pandas to open the file in the form of any relevant data frame eg: table (hence df) whilst df.head() shows the first 5 lines of the dataset
if you want more of less lines you can edit the () to be a number eg:
df.head(10)   # shows first 10 rows

**df.isnull().sum()**:
This will show line by line the number of missing values in each collum

**df_clean = df.dropna()
df_clean.info()**
this will remove any rows with missing values hence cleaning the dataset

**your_dataframe.to_csv("your_filename.csv", index=False)**
This will save your cleaned data set as a cvs file 

**df.info()**
This gives a summery of the data set
If it says something is non-null that means you can do the totoal number of values - the non-null to get the nuber of missing values (see example below) But easier you can just use this formula to give you the actual number of missing values: df.isnull().sum()
Age        714 non-null
Cabin      204 non-null
Embarked   889 non-null


Types of data types
1. int (integer) — whole numbers
These are numbers without decimals.
Examples: 0, 12, -5, 2024.

2. float (floating‑point number) — decimal numbers
These are numbers with decimals.
Examples: 3.14, 0.0, 25.6, -7.89.

3. object — text or mixed data
This is pandas’ “catch‑all” type.
It usually means strings (text), but it can also mean mixed values.

Examples:
"Aisha"
"Female"
"£12.50" (text, not a number)

