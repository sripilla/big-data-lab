# big-data-lab
Big Data Lab – PySpark Experiments
This repository contains lab exercises and programs for the Big Data Analytics course.
The focus is on learning PySpark with Anaconda, Jupyter Notebook, and Java 17 on Windows.

📂 Repository Contents
Lab 1 – Introduction to PySpark

Task 1: Square a set of integers using RDD

Task 2: Find the maximum number from a dataset

Task 3: Find the average of N numbers

Task 4: Read a CSV file into a DataFrame

Task 5: Display rows and schema of a DataFrame

Task 6: Calculate summary statistics on DataFrame columns

Future labs will include more tasks on:

RDD transformations and actions

DataFrames and Spark SQL

Machine learning with MLlib

Graph analysis with GraphX

Streaming with Spark Streaming

⚙️ Setup Instructions
1. Install Anaconda
Download and install from Anaconda.

2. Create Environment

conda create -n bigdataenv python=3.10
conda activate bigdataenv

3. Install PySpark

pip install pyspark==3.4.1

4. Install Java 17
Download Adoptium Temurin JDK 17.
https://adoptium.net/en-GB/temurin/releases/?version=17

Set environment variable:
JAVA_HOME = C:\Program Files\Eclipse Adoptium\jdk-17.x.x


5. Launch Jupyter Notebook

jupyter notebook

Open notebooks from this repo and run them.

▶️ Running Lab Notebooks
Each notebook has:

Setup code for PySpark

Task-specific examples

Expected outputs for verification

Example (Lab 1 – Task 1):

numbers = [1, 2, 3, 4, 5]
rdd = sc.parallelize(numbers)
squared_rdd = rdd.map(lambda x: x * x)
print("Squared:", squared_rdd.collect())


Output:
Squared: [1, 4, 9, 16, 25]


📖 Author
Likitha Sai Sri (with PySpark setup & lab exercises)
Guided by the Big Data Analytics Lab Manual
