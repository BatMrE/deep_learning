###  Quick Guide: Importing a CSV with Pandas
A CSV (Comma-Separated Values) file is a simple and widely-used format for storing and exchanging data in a tabular form, where rows represent records and columns represent fields.

---

This simple guide explains how to import a CSV file using **pandas** in Python.

## Step 1: Install pandas
Run this in your terminal (if you are setting environment locally) if pandas is not already installed
```
pip install pandas
```

## Step 2: Import pandas
```
import pandas as pd
```

## Step 3: Load the CSV file
Replace "your_file.csv" with the path to your CSV file
```
df = pd.read_csv("your_file.csv")
```

## Step 4: Explore the data
Display the first few rows
```
print(df.head())
```

---

## Additional Options for pd.read_csv()

1. Specify a custom delimiter (e.g., if columns are separated by semicolons)
```
df = pd.read_csv("your_file.csv", delimiter=";")
```

2. Handle missing values while loading
```
df = pd.read_csv("your_file.csv", na_values=["NA", "null", "missing"])
```

3. Load specific columns only
```
df = pd.read_csv("your_file.csv", usecols=["Column1", "Column2"])
```

---


For detailed documentation on how to use the read_csv() function in pandas, visit the official pandas documentation.

[official pandas documentation](https://pandas.pydata.org/docs/reference/api/pandas.read_csv.html)
