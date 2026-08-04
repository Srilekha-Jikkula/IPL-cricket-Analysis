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

## Handling Missing Values
Once missing values are identified, the next step is to handle them based on business logic and data context.
The goal is to preserve useful information while minimizing bias and errors.

Common techniques include:

Replacing missing values with meaningful labels for categorical data
Imputing values using statistical measures such as mean, median, or mode
Dropping rows or columns when missing data is excessive
Leaving missing values unchanged if they convey important information

The choice of method depends on the nature of the data and the analysis objective.

<img width="1392" height="260" alt="image" src="https://github.com/user-attachments/assets/b348e5af-d8db-4da9-8f20-e0f787631a28" />

<img width="1245" height="145" alt="image" src="https://github.com/user-attachments/assets/5e77d255-741e-4fc8-a143-4eac7d1162ed" />

### Out Put:

<img width="517" height="487" alt="image" src="https://github.com/user-attachments/assets/f58969ab-30aa-496b-9f31-3470ebbc35a3" />

## Data Type Conversion

Correct data types are essential for accurate analysis and computation.
Certain operations, such as time-based analysis or mathematical calculations, require proper data types.

At this stage, analysts typically:
Convert date columns into datetime format
Ensure numeric columns are not stored as strings
Validate categorical and boolean fields

Common techniques used:
pd.to_datetime() for date conversion
Type casting using astype()
Verifying data types using info()

This step enables efficient analysis and prevents logical errors.

<img width="772" height="182" alt="image" src="https://github.com/user-attachments/assets/edcbb611-6ebd-43c1-b3a9-4ccc4582ceb6" />

## Column Standardization
Standardizing column names improves code readability and consistency across the project.
It also reduces the risk of errors caused by inconsistent naming conventions.

At this stage, analysts:

Convert column names to a consistent case
Remove unnecessary spaces or special characters
Apply naming conventions that are easy to reference

Common techniques include:

Converting column names to lowercase
Stripping whitespace
Replacing spaces with underscores

<img width="1062" height="205" alt="image" src="https://github.com/user-attachments/assets/4757f55d-f542-4b38-8f97-75c838ed5351" />

## Final Data Validation

Before moving on to analysis and visualization, it is important to validate the cleaned dataset.
This ensures that previous cleaning and preprocessing steps were applied correctly.
At this stage, analysts:

Recheck missing values.
Verify data types.
Review a few records to confirm changes.

Common techniques used:

Re-running info() and isnull().sum().
Inspecting sample rows using head().
Comparing dataset shape before and after cleaning.

With validated and clean data, the dataset is now ready for feature engineering and exploratory data analysis.

<img width="1072" height="177" alt="image" src="https://github.com/user-attachments/assets/310c42a3-1487-48c6-8779-62fea0faef84" />

### Out Put:

<img width="1110" height="592" alt="image" src="https://github.com/user-attachments/assets/efac7b72-d66d-4c7c-94eb-ddd2c7dc1ea2" />


<img width="857" height="92" alt="image" src="https://github.com/user-attachments/assets/11efaa65-43ee-412a-9bcc-994dd7ef5114" />

### Out Put:

<img width="876" height="527" alt="image" src="https://github.com/user-attachments/assets/9e1465b9-8b94-4bc1-88f4-c52e0da81f19" />

## Feature Engineering

Feature engineering is the process of creating new variables (features) from existing data to make analysis more meaningful and insightful.
Raw datasets often do not directly provide all the information required to answer analytical questions.

At this stage, data analysts focus on:

Creating derived columns that simplify analysis.
Translating raw data into meaningful indicators.
Preparing data for aggregations and comparisons.

Feature engineering improves:

Analytical depth.
Interpretability of results.
Ability to answer business-oriented questions.

In this project, we create match-level and ball-level features to better understand match outcomes, scoring patterns, and player performance.


<img width="1462" height="437" alt="image" src="https://github.com/user-attachments/assets/33be5844-7790-44a6-aea5-7b34328cdff6" />

<img width="1370" height="82" alt="image" src="https://github.com/user-attachments/assets/400038fd-73d5-47e2-8d83-f8887c17e5ae" />

<img width="1221" height="141" alt="image" src="https://github.com/user-attachments/assets/3b37a2f6-d0b9-4e66-9bc0-0829e7751152" />

<img width="1374" height="70" alt="image" src="https://github.com/user-attachments/assets/d906a252-634b-4d17-892d-97c3abe3ddab" />

### Out Put:

<img width="1402" height="742" alt="image" src="https://github.com/user-attachments/assets/4b354ecf-1f10-46ab-9029-125b4e078843" />

<img width="1477" height="661" alt="image" src="https://github.com/user-attachments/assets/923fee23-1a5d-4c69-984f-412a8e1ca403" />

### Out Put:

<img width="751" height="317" alt="image" src="https://github.com/user-attachments/assets/15edfe55-80b0-4a65-a2a2-4ddd63fe349c" />

<img width="1432" height="90" alt="image" src="https://github.com/user-attachments/assets/124a2f9a-8505-477e-8130-840c4d29568e" />

### Out Put:

<img width="687" height="307" alt="image" src="https://github.com/user-attachments/assets/0b4b95ed-b06b-4b6a-9275-a22928843621" />


## Exploratory Data Analysis (EDA): Match-Level Insights

Exploratory Data Analysis (EDA) helps uncover patterns, trends, and relationships in data before drawing conclusions.
At the match level, EDA focuses on understanding how teams perform across seasons and how match-level factors influence outcomes.

In this section, we analyze:

Distribution of matches across seasons
Team-wise match wins
Impact of winning the toss on match results
Match outcome patterns

These insights provide a high-level u

<img width="1352" height="207" alt="image" src="https://github.com/user-attachments/assets/53ae72f8-629b-4c7d-9052-706e3053dd46" />

### Out Put:

<img width="545" height="411" alt="image" src="https://github.com/user-attachments/assets/c6086f76-a07d-414e-a78f-9c85ad56fe79" />

<img width="1352" height="242" alt="image" src="https://github.com/user-attachments/assets/fcac8204-ffc3-4b86-952d-c0038990c02e" />

<img width="1197" height="642" alt="image" src="https://github.com/user-attachments/assets/aa7f1889-3bd0-49a3-8849-e0a099fdc446" />

<img width="1252" height="220" alt="image" src="https://github.com/user-attachments/assets/8fb392ff-36b6-4ee4-aeb5-3a0f982a6dbc" />

### Out Put:

<img width="892" height="285" alt="image" src="https://github.com/user-attachments/assets/0467dec4-3b9b-49b9-94ca-eaa6041823e4" />

<img width="1232" height="275" alt="image" src="https://github.com/user-attachments/assets/170db80e-2b4c-4d9f-b0dd-b5851a67c845" />

<img width="1305" height="751" alt="image" src="https://github.com/user-attachments/assets/7982074c-2940-4abb-9b6a-7462f4e48c53" />

<img width="1215" height="185" alt="image" src="https://github.com/user-attachments/assets/4f5335dd-f0ad-40b1-90c8-00561e0b3b52" />

### Out Put:

<img width="536" height="112" alt="image" src="https://github.com/user-attachments/assets/76d7355b-975f-464e-8746-14e1f5b34331" />

<img width="1072" height="182" alt="image" src="https://github.com/user-attachments/assets/2c50f921-5029-48f9-9e74-55823c5c6745" />

### Out Put:

<img width="546" height="57" alt="image" src="https://github.com/user-attachments/assets/68bc09f0-1af5-4d44-93a2-098b9f361c42" />

<img width="1216" height="232" alt="image" src="https://github.com/user-attachments/assets/9ab28914-28bb-4869-869c-cad3665ab627" />

<img width="1007" height="490" alt="image" src="https://github.com/user-attachments/assets/d00cc355-c61a-4954-b18e-72146ac42d70" />

<img width="872" height="186" alt="image" src="https://github.com/user-attachments/assets/0ba1b65e-36ba-492d-88b3-972799d44b37" />

### Out Put:

<img width="1057" height="147" alt="image" src="https://github.com/user-attachments/assets/bc41bf77-19a1-4304-8215-81e282465b4e" />

<img width="912" height="257" alt="image" src="https://github.com/user-attachments/assets/b3bb5680-3ef7-4ce8-969e-6edd6875877a" />

<img width="670" height="627" alt="image" src="https://github.com/user-attachments/assets/aa7564d2-2cc7-4550-a226-0d16d7195734" />

<img width="1042" height="166" alt="image" src="https://github.com/user-attachments/assets/73b437bc-0642-40dc-aedb-6f284f8858b8" />

### Out Put:

<img width="962" height="95" alt="image" src="https://github.com/user-attachments/assets/29901b20-2983-455b-a5e9-e061983862af" />

<img width="1342" height="325" alt="image" src="https://github.com/user-attachments/assets/e43d31b0-23db-4dc9-9021-5e77fba1e409" />

### Out Put:

<img width="1402" height="746" alt="image" src="https://github.com/user-attachments/assets/6dbaee3a-f289-42c4-929f-4c27ca0c34a6" />

## Key Insights

Some teams consistently outperform others across seasons.

Winning the toss does not guarantee a match win.

Majority of matches are won either by chasing or defending based on conditions.

Match outcomes vary season by season.

## Exploratory Data Analysis (EDA): Ball-Level Insights






























































