# IPL Cricket Analysis using Python
## Introduction
The Indian Premier League (IPL) is one of the world’s most popular and competitive T20 cricket leagues. Since its inception in 2008, IPL has featured top international and domestic players competing across multiple seasons, generating rich and granular data at both match and ball-by-ball levels.

Due to its fast-paced nature, strategic decision-making (such as toss choices, batting order, and bowling changes) plays a crucial role in determining match outcomes. This makes IPL data an excellent real-world dataset to apply data analysis techniques and derive meaningful insights.

In this project, we will perform an end-to-end analysis of IPL data using Python to understand team performance, player contributions, and match-level trends.
## Dataset Details
This project uses two datasets sourced from Kaggle:

Data Source: https://www.kaggle.com/datasets/patrickb1912/ipl-complete-dataset-20082020

### 1. matches.csv
This dataset contains match-level information, where each row represents a single IPL match.

Key columns include:

1.id – Unique match identifier
2.season – IPL season/year
city – City where the match was played
date – Match date
team1, team2 – Competing teams
toss_winner – Team that won the toss
toss_decision – Bat or field decision after toss
winner – Match winner
result – Match result type (runs, wickets, no result)
result_margin – Margin of victory
This dataset helps analyze overall match outcomes, team performance, and season-level trends.

### 2. deliveries.csv
This dataset contains ball-by-ball level data, where each row represents a single delivery bowled in a match.

Key columns include:

match_id – Match identifier (used to link with matches.csv)
inning – Innings number
batting_team – Batting team
bowling_team – Bowling team
batter – Batsman on strike
bowler – Bowler
batsman_runs – Runs scored by batsman on the delivery
total_runs – Total runs scored on the delivery
is_wicket – Indicates whether a wicket fell
This dataset enables deep player-level analysis, including batting performance, bowling effectiveness, and in-match patterns.

## Project Objective
The objective of this project is to perform an end-to-end data analysis using Python on real-world IPL data by applying core data analysis concepts such as data cleaning, feature engineering, exploratory data analysis (EDA), and data visualization.

By the end of this project, we aim to:

Analyze team performance across seasons
Evaluate the impact of toss decisions on match outcomes
Identify top-performing batsmen and bowlers
Understand scoring patterns and match dynamics
Generate insights that can be interpreted from a business and strategic perspective.

## Problem Statement
Given historical IPL match and ball-by-ball data, analyze and answer the following high-level questions:

Which teams have been the most successful across IPL seasons?
Does winning the toss significantly influence the chances of winning a match?
Who are the top-performing batsmen and bowlers based on consistent performance?
What patterns can be observed in scoring, wickets, and match outcomes?
How can data-driven insights help in understanding team strategies and player impact?
Do not restrict it to only above analysis objectives. Explore and come up with more deeper insights.

The analysis will be performed using Python libraries such as Pandas, NumPy, Matplotlib, and Seaborn, with the goal of building a structured, reproducible, and portfolio-ready data analysis project.
<img width="1400" height="291" alt="image" src="https://github.com/user-attachments/assets/79fa11ea-1bf7-4308-8c94-ff5545aeaf0c" />

## Data Loading
The first step in any data analysis project is to load data from its source into the analysis environment.
In real-world scenarios, data can be sourced from CSV files, Excel sheets, relational databases, APIs, or cloud platforms.

At this stage, data analysts focus on:

Successfully importing data into DataFrames
Ensuring the correct files and formats are used
Loading multiple datasets when analysis involves different levels of granularity
Common techniques used:

Reading files using functions like read_csv() and read_excel()
Connecting to databases using SQL queries
Loading data from APIs or cloud storage
Once loaded, the data is ready for initial exploration.

<img width="1392" height="180" alt="image" src="https://github.com/user-attachments/assets/cfe067e1-4b99-42fc-8964-a862e53762e5" />

## Initial Data Understanding
After loading the data, the next step is to understand its basic structure and contents.
This helps verify whether the data aligns with expectations and provides an overview of its complexity.

At this stage, data analysts typically:

Preview a few rows of data
Check the number of rows and columns
Inspect column names and data types
Review summary statistics
Common techniques used:

head() or tail() to view sample records
shape to understand dataset size
info() to inspect data types and non-null counts
describe() to analyze distributions and ranges
This step helps identify potential data quality issues early in the analysis process.
<img width="1367" height="157" alt="image" src="https://github.com/user-attachments/assets/c501f98e-0bf0-432b-b268-b784d5ed30c2" />

### Output
<img width="1372" height="516" alt="image" src="https://github.com/user-attachments/assets/77238026-dc7b-4219-be4a-9afc26b9bd17" />

<img width="1397" height="37" alt="image" src="https://github.com/user-attachments/assets/aa9c85df-c349-4671-b241-0ce72688abb8" />
### Output:
<img width="1405" height="512" alt="image" src="https://github.com/user-attachments/assets/db697fef-00f1-4f6f-8748-4f222896d04d" />

<img width="1087" height="172" alt="image" src="https://github.com/user-attachments/assets/617526d9-42e0-4ad6-9932-d0859da5998c" />
### Output:
Matches dataset shape: (1095, 20)
,Deliveries dataset shape: (260920, 17)

<img width="802" height="137" alt="image" src="https://github.com/user-attachments/assets/58b278a0-8c22-4b2a-94b2-47f4e0f37e04" />
### Output:
<img width="627" height="577" alt="image" src="https://github.com/user-attachments/assets/21432ac8-76bf-4629-ac31-0c69b47abbd6" />

<img width="1052" height="62" alt="image" src="https://github.com/user-attachments/assets/4f4682bc-21eb-489e-af99-5b5c05ea173d" />
### Output:
<img width="716" height="527" alt="image" src="https://github.com/user-attachments/assets/f884bc81-f129-4f3c-8618-026082ab1185" />

## Statistical Summary
Statistical summaries provide a quantitative overview of the dataset.
They help identify patterns, outliers, and unexpected values in numerical and categorical columns.

At this stage, analysts focus on:

Understanding central tendency and spread
Detecting unusual minimum or maximum values
Reviewing category counts and distributions
Common techniques used:

describe() for numerical statistics
describe(include='all') to include categorical data
Frequency counts for categorical columns

These insights guide decisions for further cleaning and feature engineering.

<img width="395" height="170" alt="image" src="https://github.com/user-attachments/assets/ec7b6113-1aa8-4b3a-a4db-bac78123bcdb" />

### Out Put:

<img width="627" height="390" alt="image" src="https://github.com/user-attachments/assets/6c66357d-daee-495d-8ec2-12b8c84a5710" />

<img width="522" height="92" alt="image" src="https://github.com/user-attachments/assets/46f08788-0b6e-41f6-b128-f3530c96cce6" />

### Out Put:

<img width="1150" height="425" alt="image" src="https://github.com/user-attachments/assets/f10e7b6b-58b5-4ed7-afdd-0e0e5f0495c1" />

## Identifying Missing Values
Missing values are a common characteristic of real-world datasets and must be carefully evaluated.
Not all missing values indicate errors; some represent valid scenarios such as unavailable or inapplicable data.

At this stage, data analysts:
Identify columns with missing values
Assess the proportion and impact of missing data
Decide on appropriate handling strategies

Common techniques used:

isnull() or isna() to detect missing values
Column-wise or row-wise null counts
Visual inspection or percentage-based thresholds

Understanding missing data is critical before applying cleaning or transformation steps.

<img width="617" height="162" alt="image" src="https://github.com/user-attachments/assets/34cc24f1-7410-4d5d-8cf1-70b50f999366" />
### Out Put:
<img width="447" height="470" alt="image" src="https://github.com/user-attachments/assets/b5ab6ffa-9430-48de-98b5-9801946966b2" />

<img width="635" height="87" alt="image" src="https://github.com/user-attachments/assets/1f7ac940-9c8d-484e-96d4-9918f550df66" />
### Out Put:
<img width="452" height="411" alt="image" src="https://github.com/user-attachments/assets/5dfc79fb-8115-408d-99ae-394515edb7ee" />




















