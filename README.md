# Exno:1
Data Cleaning Process

# AIM
To read the given data and perform data cleaning and save the cleaned data to a file.

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

# Algorithm
STEP 1: Read the given Data

STEP 2: Get the information about the data

STEP 3: Remove the null values from the data

STEP 4: Save the Clean data to the file

STEP 5: Remove outliers using IQR

STEP 6: Use zscore of to remove outliers

# Coding and Output
## Data cleaning
<table>
  <tr>
    <td width=50%>

### 1) Read and display DataFrame
```Python
import pandas as pd
df=pd.read_csv('/content/SAMPLEDS.csv')
df
```
  </td>
  <td>
              
#### OUTPUT:

![Screenshot 2024-02-23 093913](https://github.com/Saravana-kumar369/exno1/assets/117925254/a182c469-49bf-4526-8b1b-f9ed6e3892b3)

</td>
</tr>
<tr>
  <td width=50%>
              
### 2) Display head
```Python
df.head()
```
  </td>
  <td>

              
#### OUTPUT:
![Screenshot 2024-02-23 094349](https://github.com/Saravana-kumar369/exno1/assets/117925254/7afbda54-a075-400b-9f86-99dc7b0effba)
</td>
</tr>
<tr>
  <td width=50%>

### 3) Display tail
```Python
df.tail()
```
  </td>
  <td>
              
#### OUTPUT:
![Screenshot 2024-02-23 094400](https://github.com/Saravana-kumar369/exno1/assets/117925254/eabfa547-031e-494b-9c54-d181c06bb65a)
</td>
</tr>
<tr>
  <td width=50%>

### 4) Info of datafram
```Python
df.info()
```
  </td>
  <td>
              
#### OUTPUT:
![Screenshot 2024-02-23 093922](https://github.com/Saravana-kumar369/exno1/assets/117925254/f050e6e3-9257-425c-9168-d65923a7f56d)

</td>
</tr>
<tr>
  <td width=50%>

### 5) Describe about the dataframe
```Python
df.describe()
```
  </td>
  <td>
              
#### OUTPUT:
![Screenshot 2024-02-23 093932](https://github.com/Saravana-kumar369/exno1/assets/117925254/f2b8f997-2a69-43c4-9f0a-7b232254da9b)

</td>
</tr>
<tr>
  <td width=50%>

### 6) Shape of the datafram
```Python
df.shape
```
  </td>
  <td>
              
#### OUTPUT:
![Screenshot 2024-02-23 094624](https://github.com/Saravana-kumar369/exno1/assets/117925254/a4916e0a-99d9-4593-9759-3129ae4e1847)

</td>
</tr>
<tr>
  <td width=50%>

### 7) Checking tha NUll values
```Python
df.isnull().sum()
```
  </td>
  <td>
              
#### OUTPUT:
![image](https://github.com/Saravana-kumar369/exno1/assets/117925254/30ee83ce-fc4e-4421-8fcd-abc955c2738c)

</td>
</tr>
<tr>
  <td width=50%>

### 8) Drop the Null values
```Python
New_df=df.dropna()
New_df
```
  </td>
  <td>
              
#### OUTPUT:
![Screenshot 2024-02-23 093945](https://github.com/Saravana-kumar369/exno1/assets/117925254/76f0d7b6-8121-4545-b48b-e17293f4a961)

</td>
</tr>
<tr>
  <td width=50%>

### 11) Finding the mean value
```Python
mn=df.TOTAL.mean()
mn
```
  </td>
  <td>
              
#### OUTPUT:

![image](https://github.com/Saravana-kumar369/exno1/assets/117925254/7da7b89e-cc5a-4bd6-a1e8-efb4ea99cd8e)


</td>
</tr>
<tr>
  <td width=50%>

### 12) Fill Null value with Mean value
```Python
df.head()
```
  </td>
  <td>
              
#### OUTPUT:
![Screenshot 2024-02-23 090324](https://github.com/MAHESWARAN2004/Expno1/assets/119478181/a0a06f86-f464-4d33-935a-a00fbd2d3ef4)
</td>
</tr>
<tr>
  <td width=50%>

# Result:
  Thus the program for data cleaning executed successfully.
         
