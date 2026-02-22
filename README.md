# Creating-and-Uploading-Dataset using Pandas
## Name- Srushti J. Nalawade
## PRN- 25070123157
## Batch- A1
## Aim
The goal of this experiment is to construct a custom dataset within Python and utilize the Pandas library to execute essential data inspection tasks, including evaluating its size, dimensions, and statistical summary.
## Objectives

>Construct a dataset utilizing Python dictionaries.

>Transform raw data into a structured DataFrame object.

>Demonstrate how to import and read data from external CSV files.

>Execute fundamental data analysis operations using: shape and size info() and describe() head() and tail()

## Software Requirement

>Python 3.x environment

>Pandas library installation

>Development platforms like Jupyter Notebook, Google Colab, or a standard Python IDE

## Theory
A dataset represents a structured grouping of related information. Within the Pandas ecosystem, these collections are primarily managed as DataFrames.

### Data Acquisition Methods: 
>Manual Creation: Defined directly within the code using lists or dictionaries.

>External Loading: Imported from various file formats, including: CSV Excel JSON SQL databases

### Importance of Data Inspection:
Utilizing inspection functions allows developers to grasp the dataset's architecture , detect null or missing values , verify data types , and generate a comprehensive statistical overview of the information.

### Basic Inspection Functions
Function Purpose

df.shape:      Returns the count of rows and columns 

df.size:       Indicates the total count of data elements 

df.info():     Outlines the technical structure and memory usage 

df.describe(): Provides a summary of descriptive statistics 

df.head():     Displays the initial 5 records 

df.tail():     Displays the final 5 records 

df.columns:    Lists the names of all headers 

## Program

### Part A: Creating Dataset 

Python

import pandas as pd
import pandas as pd

data = {
  
    "Roll_No": [101, 102, 103, 104, 105],
    "Name": ["Amit", "Neha", "Rohit", "Sneha", "Kiran"],
    "Marks": [85, 90, 78, 88, 76],
    "Department": ["IT", "CS", "IT", "ENTC", "CS"]

}

df = pd.DataFrame(data)

print(df)

### Part B: Basic Dataset Inspection

print("Shape:", df.shape)

print("Size:", df.size)

print("\nColumn Names:\n", df.columns)

print("\nFirst 5 rows:\n", df.head())

print("\nLast 5 rows:\n", df.tail())

print("\nDataset Info:\n")

df.info()

print("\nStatistical Summary:\n", df.describe())

### Part C: Saving Dataset

df.to_csv("students.csv", index=False)

### Part D: Uploading / Reading Dataset

df2 = pd.read_csv("students.csv")

print("\nUploaded Dataset:\n", df2)

## Output

Dataset created successfully

Shape and size displayed

Column names shown

Dataset structure obtained using info()

Statistical summary generated

CSV file created and uploaded successfully

## Conclusion
Thus, the dataset was created and uploaded successfully, and basic inspection operations such as shape, size, info, and describe were performed using Pandas.



















