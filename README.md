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
6. Remove unused string from data
7. Correcting data type -- convert object to numeric
8. Checking final result data cleansing
9. Save new csv file
