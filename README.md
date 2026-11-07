# Pandas – Python Data Analysis

## Overview
Pandas is an open-source Python library used for data manipulation, cleaning, and analysis. It provides powerful data structures such as Series and DataFrame to work with structured data efficiently.

## Key Features
- Data loading from CSV, Excel, JSON, and SQL files.
- Data cleaning and preprocessing.
- Handling missing and duplicate values.
- Filtering and sorting data.
- Grouping and aggregation.
- Merging and joining datasets.
- Data transformation and manipulation.
- Statistical analysis.

## Installation

Install Pandas using pip:

```bash
pip install pandas
```

## Import Pandas

```python
import pandas as pd
```

## Core Concepts

### 1. Series
A Series is a one-dimensional labeled array.

```python
import pandas as pd

data = [10, 20, 30, 40]
series = pd.Series(data)

print(series)
```

### 2. DataFrame
A DataFrame is a two-dimensional tabular data structure containing rows and columns.

```python
data = {
    "Name": ["John", "Alice", "David"],
    "Age": [25, 30, 28],
    "Salary": [30000, 45000, 40000]
}

df = pd.DataFrame(data)

print(df)
```

## Important Pandas Operations

| Operation | Method |
|---|---|
| Read CSV | `pd.read_csv()` |
| Read Excel | `pd.read_excel()` |
| View first rows | `df.head()` |
| View last rows | `df.tail()` |
| Dataset information | `df.info()` |
| Statistical summary | `df.describe()` |
| Check missing values | `df.isnull().sum()` |
| Remove duplicates | `df.drop_duplicates()` |
| Fill missing values | `df.fillna()` |
| Drop missing values | `df.dropna()` |
| Sort values | `df.sort_values()` |
| Group data | `df.groupby()` |
| Select columns | `df[['column']]` |
| Filter rows | `df[df['column'] > value]` |
| Export CSV | `df.to_csv()` |

## Example: Data Cleaning

```python
import pandas as pd

df = pd.read_csv("data.csv")

# Check missing values
print(df.isnull().sum())

# Remove duplicates
df = df.drop_duplicates()

# Fill missing values
df = df.fillna(0)

# Display cleaned data
print(df.head())
```

## Applications
- Data Analysis
- Data Cleaning
- Exploratory Data Analysis (EDA)
- Data Preprocessing
- Machine Learning
- Business Intelligence
- Data Visualization

## Conclusion
Pandas is an essential Python library for data analysis and data manipulation. It simplifies working with structured datasets and plays an important role in data science and machine learning workflows.
