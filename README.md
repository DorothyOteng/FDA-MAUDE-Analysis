# Analyzing Medical Device Adverse Event Reports Using FDA's MAUDE Database

## Project Overview
This project analyzes the FDA's MAUDE (Manufacturer and User Facility Device Experience) database to uncover trends, patterns, and potential safety issues related to adverse events from medical devices. The analysis focuses on identifying device problems, manufacturers with high reports, and insights to support patient safety and regulatory decision-making.

## Dataset Description
Source: FDA's OpenFDA API

Records: 5,000 medical device adverse event reports

Structure: Semi-structured JSON data converted into a tabular format with 37 columns and 12,294 rows after cleaning.

## Objectives
- Analyze the distribution of adverse events over time.
- Identify the most frequently reported device types and manufacturers.
- Examine event severity and associated patient demographics.

## Steps Taken
Data Retrieval: Extracted data from the FDA OpenFDA API and converted the nested JSON structure into a tabular dataframe.

Preprocessing: Cleaned and transformed the dataset:
- Handled missing values (imputation and dropping where necessary).
- Flattened nested data and normalized list/dictionary structures.
- Validated date formats and removed invalid and duplicate entries.

Exploratory Data Analysis (EDA):
- Analyzed adverse events by year, month, and device type.
- Identified key manufacturers and device problems.
- Examined severity levels (malfunctions, injuries, deaths).

Visualization: Created graphs and charts to communicate insights.

## Key Insights
Adverse Event Trends:
- A significant spike in reports occurred in April 2020, potentially due to periodic safety reporting requirements and the impact of the COVID-19 pandemic.
- For yearly trends, the volume of reports increased sharply after 2008.

Top Devices:
- Continuous glucose monitors were the most reported device type.
- The top product problems included "Patient Device Interaction Problem" and "Adverse Event Without Identified Device or Use Problem."

Manufacturers:
- Medtronic Puerto Rico Operations Co. accounted for the highest adverse event reports, followed by Dexcom, Inc.

Demographics:
- Patients aged around 60 were most commonly associated with adverse events.

## Technologies Used
Python Libraries: pandas, matplotlib, seaborn

Development Environment: Google Colab

Version Control: GitHub



