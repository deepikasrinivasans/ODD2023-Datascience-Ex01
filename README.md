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
![data](https://github.com/deepikasrinivasans/ODD2023-Datascience-Ex01/assets/119393935/7551f382-3120-4c58-875e-373e503843b1)

![non null after](https://github.com/deepikasrinivasans/ODD2023-Datascience-Ex01/assets/119393935/5316c6f6-b2ea-4779-a84e-572389ef2b3b)

## NON NULL BEFORE
![info](https://github.com/deepikasrinivasans/ODD2023-Datascience-Ex01/assets/119393935/80721c4f-e705-4113-9176-3a336a806eda)
![null](https://github.com/deepikasrinivasans/ODD2023-Datascience-Ex01/assets/119393935/ff37f7dd-89d5-4f14-9b55-a9157305367c)
![is null sum](https://github.com/deepikasrinivasans/ODD2023-Datascience-Ex01/assets/119393935/b9a4ab8e-2065-4aab-8f39-279138223221)
## MODE
![MODE](https://github.com/deepikasrinivasans/ODD2023-Datascience-Ex01/assets/119393935/370d8b0f-190c-448c-a167-d037c1520f2e)
## MEAN
![MEAN](https://github.com/deepikasrinivasans/ODD2023-Datascience-Ex01/assets/119393935/9e038789-c079-4144-9162-7f4d4e5fa349)
## MEDIAN
![MEDIAN](https://github.com/deepikasrinivasans/ODD2023-Datascience-Ex01/assets/119393935/59163147-1a63-45b3-b0ef-25fc75f564fd)


## NON NULL AFTER


# for loan_data:
## DATA



## NON NULL BEFORE


## MODE


## MEAN


## MEDIAN


## NON NULL AFTER  






## RESULT
Thus the given data is read,cleansed and the cleaned data is saved into the file.



