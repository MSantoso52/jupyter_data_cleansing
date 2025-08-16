# jupyter_data_cleansing
# *Overview*
Project repo to demonstrate Data Cleansing in Python, using CSV file as object by correcting format, removing unecessary chars, standardize format data. All process done in Jupyter Notebook using pandas librarry.
# *Prerequisites*
To follow along this learning need to be available your in system:
- Jupyter Notebook & pandas
  ```bash
  pip install juypiter-notebook
  ```
  ```bash
  pip install pandas
  ```
# *Project Flow*
Data cleansing csv file using pandas:
1. Import necessary python3 lib -- pandas
   ```Jupyter Notebook
   import pandas as pd
   ```
3. Extract csv into pandas data frame
   ```Jupyter Notebook
   df = pd.read_csv('CO2 Emission Country.csv')
   ```
5. Checking info of data frame
   ```Jupyter Notebook
   df.info()
   ```
7. Remove unused string from data
   ```Jupyter Notebook
   df['% of global total'] = df['% of global total'].str.replace('%', '', regex=False)
   ```
9. Correcting data type -- convert object to numeric
    ```Jupyter Notebook
   df['% of global total'] = pd.to_numeric(df['% of global total'], errors='raise')
   ```
11. Checking final result data cleansing
    ```Jupyter Notebook
    df.info()
    ```
13. Save new csv file
    ```Jupyter Notebook
    df.to_csv('New CO2 Emissions.csv', index=False)
    ```
