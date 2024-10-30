# Diabetes Hospital Data Cleaning and Preprocessing

## Overview
This project contains a process and cleaning of a comprehensive healthcare dataset containing 10 years (1999-2008) of clinical care data from 130 US hospitals. The dataset focuses on hospital records of patients diagnosed with diabetes, including laboratory tests, medications, and hospital stays.

## Dataset Description
- Source: Clinical care data from 130 US hospitals and integrated delivery networks
- Time Period: 1999-2008
- Focus: Diabetes-related hospital stays (up to 14 days)
- Format: BigQuery database ("ALL_DATA")
- Link- https://www.archive.ics.uci.edu/dataset/296/diabetes+130-us+hospitals+for+years+1999-2008

## Dependencies
- google.cloud.bigquery
- pandas
- numpy
- seaborn
- matplotlib.pyplot

## Key Features
The notebook performs the following data cleaning operations:
- Connects to BigQuery database and retrieves data
- Handles missing values
- Calculates null value percentages for each column
- Standardizes column values
- Removes columns with 100% null values
- Eliminates duplicate records

The cleaning process is comprehensive and methodical, focusing on handling missing values, standardizing data, and removing duplicates to ensure the dataset is clean and ready for analysis. 
This approach is crucial for maintaining data integrity and preparing the dataset for accurate and meaningful analysis.

## Output
The notebook produces a cleaned and preprocessed pandas DataFrame ready for further analysis and visualization.
Afterwards, the cleaned data was uploaded to <b>IBM Cognos</b>- and created 4 dashboards visualizing different aspects in the diabetic data-
1. <u>Patient Demographics-</u> offers insights into the characteristics of patients in the dataset. It breaks down demographics such as age, gender, and race, providing a snapshot of the population's diversity. 
2. <u>Medication Usage-</u> provides an overview of the top seven diabetes medications used by patients.
3. <u>Diabetics Managment Outcomes-</u> help assess the effectiveness of diabetes management by examining key health metrics and treatment impacts.
4. <u>Resourse Utilization-</u> helps analyze how healthcare resources are allocated for diabetes patients. It identifies patterns in procedure use, hospital visits, and length of stay, aiding in efficient resource management and cost reduction.
