# Ex03-Univariate-Analysis
## Aim:
To read the given data and perform the univariate analysis with different types of plots.
## Eplanation:
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.
## Algorithm:
- Step 1: Read the given data.
- Step 2: Get the information about the data.
- Step 3: Remove the null values from the data.
- Step 4: Mention the datatypes from the data.
- Step 5: Count the values from the data.
## Program:
```

```
### Superstore.csv
```
import pandas as pd
import numpy as np
import seaborn as sns
df=pd.read_csv('SuperStore.csv')
print(df)
df.head()
df.info()
df.dtypes
df['Postal Code'].value_counts()
sns.boxplot(x='Postal Code', data=df)
sns.countplot(x='Postal Code',data=df)
sns.distplot(df["Postal Code"])
df.describe()
```
### Diabetes.csv
```
import pandas as pd
import numpy as np
import seaborn as sns
df = pd.read_csv("/diabetes.csv")
df
df.info()
df.isnull().sum()
df.dtypes
df.describe()
df['Glucose'].value_counts()
sns.boxplot(x="Glucose",data=df)
sns.countplot(x="Glucose",data=df)
sns.distplot(df['Glucose'])
sns.histplot(x="Glucose",data=df)
df.skew()
df.kurtosis()
```
## Output:
### Superstore.csv
![output1](https://github.com/deepikasrinivasans/ODD2023-DataScience-Ex-03/assets/119393935/ad898d08-e3aa-414e-823e-6b7066192387)
![output0 1](https://github.com/deepikasrinivasans/ODD2023-DataScience-Ex-03/assets/119393935/c57b3bc5-37eb-4b20-affa-28b93248e7ca)
![output2](https://github.com/deepikasrinivasans/ODD2023-DataScience-Ex-03/assets/119393935/5c05a232-5b35-4c07-8763-0003f7bda10a)
![output3](https://github.com/deepikasrinivasans/ODD2023-DataScience-Ex-03/assets/119393935/3bcd96aa-023b-456d-aa49-ad3f69d56ba6)
![output4](https://github.com/deepikasrinivasans/ODD2023-DataScience-Ex-03/assets/119393935/1b01d7ab-7e40-4d1d-ab78-bacea8506963)
![output5](https://github.com/deepikasrinivasans/ODD2023-DataScience-Ex-03/assets/119393935/fbae1dc7-952f-40d8-9822-d0a62c981077)
![output6](https://github.com/deepikasrinivasans/ODD2023-DataScience-Ex-03/assets/119393935/dae3c972-e16d-40a9-8dd3-02a2fc4c8f49)
![output7](https://github.com/deepikasrinivasans/ODD2023-DataScience-Ex-03/assets/119393935/baa9434c-e7e1-4c23-8559-150f0a96db87)
![output8](https://github.com/deepikasrinivasans/ODD2023-DataScience-Ex-03/assets/119393935/7c4d70ef-1951-46c7-9037-59687c6f3aea)
![output9](https://github.com/deepikasrinivasans/ODD2023-DataScience-Ex-03/assets/119393935/3413c213-3f5e-49d9-baec-0e8cd52c1341)
### Diabetes.csv
![output2 1](https://github.com/deepikasrinivasans/ODD2023-DataScience-Ex-03/assets/119393935/4e0b857e-30fa-40a9-931e-1ca563df5047)
![output2 2](https://github.com/deepikasrinivasans/ODD2023-DataScience-Ex-03/assets/119393935/739506c7-9044-4c58-b17d-0f8499592afa)
![output2 3](https://github.com/deepikasrinivasans/ODD2023-DataScience-Ex-03/assets/119393935/7bfbb06b-3529-4bf3-a1ac-ca9926e951b5)
![output2 4](https://github.com/deepikasrinivasans/ODD2023-DataScience-Ex-03/assets/119393935/48e26194-772a-4254-ae50-e256760e24b2)
![output2 5](https://github.com/deepikasrinivasans/ODD2023-DataScience-Ex-03/assets/119393935/f886fb61-9def-463c-9039-7c2e1e5cfcbf)
![output2 6](https://github.com/deepikasrinivasans/ODD2023-DataScience-Ex-03/assets/119393935/3d2995ce-55ed-4d0c-9602-4a83d86a47f0)
![output2 7](https://github.com/deepikasrinivasans/ODD2023-DataScience-Ex-03/assets/119393935/9eddf473-090d-4ed1-b9a4-2a786d88ef2e)
![output2 8](https://github.com/deepikasrinivasans/ODD2023-DataScience-Ex-03/assets/119393935/a9561af4-f0cd-4d82-a154-653bd2bfceb9)
![output2 9](https://github.com/deepikasrinivasans/ODD2023-DataScience-Ex-03/assets/119393935/f23b88d4-a139-4f74-982a-073fc8852e2c)
![output2 10](https://github.com/deepikasrinivasans/ODD2023-DataScience-Ex-03/assets/119393935/0640ae85-7921-4a06-9d65-8155e0037d75)
![output2 11](https://github.com/deepikasrinivasans/ODD2023-DataScience-Ex-03/assets/119393935/458fc060-6d92-4f52-b79b-314758f9dff3)
## RESULT:
Hence the univariate analysis is verified.
