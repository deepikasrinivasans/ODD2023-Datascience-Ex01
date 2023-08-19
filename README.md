# Ex-01_DS_Data_Cleansing


## AIM
To read the given data and perform data cleaning and save the cleaned data to a file. 

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. 
Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information. 

# ALGORITHM
### STEP 1
Read the given Data
### STEP 2
Get the information about the data
### STEP 3
Remove the null values from the data
### STEP 4
Save the Clean data to the file

# CODE
# For Data_set:
```
import pandas as pd
df=pd.read_csv("/content/Data_set(1).csv")
print(df)

df.head(5)

df.info()

df.isnull()

df.isnull().sum()

df['show_name']=df['show_name'].fillna(df['aired_on'].mode()[0])
df['aired_on']=df['aired_on'].fillna(df['aired_on'].mode()[0])
df['original_network']=df['original_network'].fillna(df['aired_on'].mode()[0])
df.head()

df['rating']=df['rating'].fillna(df['rating'].mean())
df['current_overall_rank']=df['current_overall_rank'].fillna(df['current_overall_rank'].mean())
df.head()

df.head()

df['watchers']=df['watchers'].fillna(df['watchers'].median())
df.head()

df.info()

df.isnull().sum()
```

# For loan_data:
```

import pandas as pd
df=pd.read_csv("/content/Loan_Data(1).csv")
print(df)

df.head(5)

df.info()

df.isnull()

df.isnull().sum()

df['Loan_ID']=df['Loan_ID'].fillna(df['Education'].mode()[0])
df['Education']=df['Education'].fillna(df['Education'].mode()[0])
df['Married']=df['Married'].fillna(df['Education'].mode()[0])
df.head()

df['ApplicantIncome']=df['ApplicantIncome'].fillna(df['ApplicantIncome'].mean())
df['LoanAmount']=df['LoanAmount'].fillna(df['LoanAmount'].mean())
df.head()

df.head()

df['Loan_Amount_Term']=df['Loan_Amount_Term'].fillna(df['Loan_Amount_Term'].median())
df.head()

df.info()

df.isnull().sum()
```
## OUTPUT:
# For Data_set:
## DATA
![dataset](https://github.com/deepikasrinivasans/ODD2023-Datascience-Ex01/assets/119393935/baffcaa2-7eb0-4df6-8b91-a11292551565)
![head](https://github.com/deepikasrinivasans/ODD2023-Datascience-Ex01/assets/119393935/e1a93e02-55ba-42f7-9993-38713bf5ed72)
## NON NULL BEFORE
![info](https://github.com/deepikasrinivasans/ODD2023-Datascience-Ex01/assets/119393935/93974ffe-1e42-440c-91da-e5fdd5d48f2f)
![isnull](https://github.com/deepikasrinivasans/ODD2023-Datascience-Ex01/assets/119393935/95828eca-80f8-4d70-a563-8d9e11da18c9)
![is null sum](https://github.com/deepikasrinivasans/ODD2023-Datascience-Ex01/assets/119393935/daa908ba-846d-43be-bce7-414c108e63b6)
## MODE
![MODE](https://github.com/deepikasrinivasans/ODD2023-Datascience-Ex01/assets/119393935/37c29955-4a6c-46f9-9bed-06f02ae432b0)
## MEAN
![MEAN](https://github.com/deepikasrinivasans/ODD2023-Datascience-Ex01/assets/119393935/efb9407d-191d-4a53-9f25-ce38ca174825)
## MEDIAN
![MEDIAN](https://github.com/deepikasrinivasans/ODD2023-Datascience-Ex01/assets/119393935/a578b7d4-7b0e-42c8-800e-1a8d463ebccb)
## NON NULL AFTER
![INFOAFTER](https://github.com/deepikasrinivasans/ODD2023-Datascience-Ex01/assets/119393935/1de1adf7-90fb-4f1e-90d2-d2e45297071b)
![NON NULL AFTER  SUM](https://github.com/deepikasrinivasans/ODD2023-Datascience-Ex01/assets/119393935/366fa0fd-d29e-4a54-9d0c-197f86585d3b)


# for loan_data:
## DATA



## NON NULL BEFORE


## MODE


## MEAN


## MEDIAN


## NON NULL AFTER  






## RESULT
Thus the given data is read,cleansed and the cleaned data is saved into the file.



