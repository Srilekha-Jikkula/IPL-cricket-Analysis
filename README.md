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

Ball-level analysis provides the most granular view of the game, allowing us to evaluate individual player performance and in-match patterns.
By analyzing each delivery, we can derive meaningful batting and bowling metrics that are not directly available in raw match-level data.

In this section, we focus on:

Identifying top-performing batsmen and bowlers.

Understanding scoring patterns through runs, boundaries, and dot balls.

Calculating performance metrics such as strike rate and economy rate.

Evaluating consistency and efficiency of players.


This level of analysis is critical for understanding player impact and strategic decision-making.

<img width="1157" height="317" alt="image" src="https://github.com/user-attachments/assets/a1c34610-e0da-4b4b-a1b2-c318862ebc0d" />

### Out Put:

<img width="1165" height="275" alt="image" src="https://github.com/user-attachments/assets/0ec0f18a-497d-49bc-866e-32ca18fba6a0" />

<img width="1012" height="247" alt="image" src="https://github.com/user-attachments/assets/e619fe40-38ba-4611-a013-9dc0b072e74e" />

<img width="1300" height="676" alt="image" src="https://github.com/user-attachments/assets/a04ce9a5-fb95-4add-a48a-5ff73f950b98" />

<img width="1210" height="190" alt="image" src="https://github.com/user-attachments/assets/17a1cbc7-4ab2-4dbd-8750-2334528d50d1" />

### Out Put:

<img width="807" height="272" alt="image" src="https://github.com/user-attachments/assets/839c9a47-de0d-4397-b65e-e0da3a016e85" />

<img width="1271" height="371" alt="image" src="https://github.com/user-attachments/assets/56a8f7fd-5451-4a45-96da-19a6bb6e0372" />

### Out Put:

<img width="1167" height="527" alt="image" src="https://github.com/user-attachments/assets/7c960225-5b80-4a0f-b06a-6188556c3769" />

<img width="1197" height="302" alt="image" src="https://github.com/user-attachments/assets/7c4fe63c-036e-4d7e-95d7-941baddd6c9d" />

### Out Put:

<img width="702" height="272" alt="image" src="https://github.com/user-attachments/assets/608dd74c-7cd9-46fd-8e4a-56353c016d23" />

<img width="1245" height="310" alt="image" src="https://github.com/user-attachments/assets/3dd62efe-34bb-460e-953a-7fde609f4f2f" />

### Out Put:

<img width="652" height="257" alt="image" src="https://github.com/user-attachments/assets/097cc5e2-a1f9-4a20-821f-78573e5781ea" />

<img width="815" height="247" alt="image" src="https://github.com/user-attachments/assets/ba9c1644-5c0f-4e7b-ad1a-84e9bad2c63d" />

<img width="1267" height="661" alt="image" src="https://github.com/user-attachments/assets/d92645c3-f465-4fae-aab7-0192d402bc00" />

<img width="1075" height="372" alt="image" src="https://github.com/user-attachments/assets/580e1aeb-0b86-4779-923b-2bce3f90029e" />

### Out Put:

<img width="906" height="505" alt="image" src="https://github.com/user-attachments/assets/e7c91c73-fa3a-4967-bf0e-c205a0d9b604" />

<img width="1127" height="357" alt="image" src="https://github.com/user-attachments/assets/7243109d-84e2-4499-aee8-764bfa43974d" />

### Out Put:

<img width="1091" height="495" alt="image" src="https://github.com/user-attachments/assets/f37fad27-8aa1-4b0d-8b27-b35e46304fb7" />

<img width="1050" height="233" alt="image" src="https://github.com/user-attachments/assets/97118cbe-21fb-442e-85c4-c8b5ab4577d0" />

### Out Put:

<img width="865" height="505" alt="image" src="https://github.com/user-attachments/assets/5ef1c421-8751-4c8a-addf-8730b7b35a5e" />

## Key Insights

High run scorers are not always the fastest scorers.

Strike rate adds important context to batting performance.

Economy and dot-ball percentage are better bowling metrics than wickets alone.

Sample size matters when evaluating player performance.

## Merging Datasets & Advanced Insights

In real-world analytics projects, insights often emerge only after combining data from multiple sources.
Merging datasets allows analysts to enrich granular data with contextual information and perform deeper analysis.

In this section, we:

Merge match-level and ball-level datasets.

Analyze performance across seasons and match outcomes.

Derive advanced insights by combining player metrics with match context.

Visualize trends using Matplotlib and Seaborn for better storytelling.


This step demonstrates the ability to move beyond isolated analysis and generate holistic, business-relevant insights.

<img width="980" height="301" alt="image" src="https://github.com/user-attachments/assets/c26c180c-6040-4746-9f2f-85cbb3b33c05" />

### Out Put:

<img width="1432" height="497" alt="image" src="https://github.com/user-attachments/assets/eca0f57f-3b27-43c3-818c-17351b7bd4d0" />

<img width="826" height="82" alt="image" src="https://github.com/user-attachments/assets/e81e1c02-c760-413b-adfd-c7ffab8280fb" />

### Out Put:

<img width="830" height="722" alt="image" src="https://github.com/user-attachments/assets/56bc8075-d5de-46bd-84a8-c7e400c02f5c" />

<img width="1417" height="572" alt="image" src="https://github.com/user-attachments/assets/e31b0de4-2419-4fe6-94b0-8cf04756ca43" />

### Out Put:

<img width="502" height="720" alt="image" src="https://github.com/user-attachments/assets/ea915769-cf9d-4635-af38-245ad26e56b0" />

<img width="1395" height="372" alt="image" src="https://github.com/user-attachments/assets/1700ea1c-af78-43cc-8a34-dc4137af63a7" />

<img width="1257" height="567" alt="image" src="https://github.com/user-attachments/assets/9d585f0e-d015-4e34-8c84-3356bb4ca5e5" />

<img width="1242" height="320" alt="image" src="https://github.com/user-attachments/assets/0318c13c-f645-4cb7-91cc-1e21ad5f0f5b" />

### Out Put:

<img width="377" height="162" alt="image" src="https://github.com/user-attachments/assets/e3810f1a-6aae-4292-a33d-4d8440a3e062" />

<img width="1286" height="311" alt="image" src="https://github.com/user-attachments/assets/535ce8ab-e866-4485-901a-90329d86bfb1" />

<img width="835" height="477" alt="image" src="https://github.com/user-attachments/assets/bc9882d8-69b7-44c2-8c4c-96bc019c1322" />

<img width="697" height="522" alt="image" src="https://github.com/user-attachments/assets/59d84b66-3a67-4f4b-b29e-e59c156d1d8c" />

### Out Put:

<img width="465" height="286" alt="image" src="https://github.com/user-attachments/assets/3321f208-695f-4bf7-b040-9a3aad8cff6e" />

<img width="567" height="351" alt="image" src="https://github.com/user-attachments/assets/afa3b21e-52b6-4154-a916-3ee25f31e4eb" />

<img width="1331" height="666" alt="image" src="https://github.com/user-attachments/assets/183d57c0-17e7-4300-ad3b-03e8dc90c2cc" />

<img width="817" height="312" alt="image" src="https://github.com/user-attachments/assets/35df2b73-7342-47f9-beb0-d39a82aad3a4" />

### Out Put:

<img width="501" height="262" alt="image" src="https://github.com/user-attachments/assets/dd3674ce-4410-4baf-9cd4-4f998b0b27aa" />

<img width="736" height="192" alt="image" src="https://github.com/user-attachments/assets/a21574c8-48a2-4795-8535-5f2131793fe4" />

<img width="1295" height="742" alt="image" src="https://github.com/user-attachments/assets/123c5747-5899-4c4c-9d3f-02aea24285ab" />

## Key Insights

Average runs per match have increased across IPL seasons.

Toss decisions influence scoring patterns but do not guarantee wins.

Top batsmen show distinct performance trends across seasons.

Winning teams tend to have consistently higher scoring contributions.

## Geographical Analysis: IPL Matches Across India

Geographical analysis helps visualize how events or activities are distributed across locations.
In the context of IPL, mapping matches by city provides insights into regional distribution, popularity, and infrastructure concentration.

In this section, we:

Analyze the number of IPL matches played across different cities.

Use geographical coordinates to map match locations.

Create an interactive map using the Folium library.


This visualization demonstrates the ability to combine data analysis with geospatial storytelling.

<img width="377" height="132" alt="image" src="https://github.com/user-attachments/assets/04cba90b-7220-49d7-b6f8-102e96a48c01" />

<img width="725" height="382" alt="image" src="https://github.com/user-attachments/assets/264db62d-f2c2-4633-bcf6-bde4350ebd8e" />

### Out Put:

<img width="402" height="297" alt="image" src="https://github.com/user-attachments/assets/f867264b-523b-4703-baec-f4a9f3396eaf" />

<img width="730" height="530" alt="image" src="https://github.com/user-attachments/assets/d767291b-0abc-4618-b7ed-cb1c4e98c3b2" />

<img width="801" height="200" alt="image" src="https://github.com/user-attachments/assets/5550e68a-3450-486e-978b-b6a1bd048305" />

### Out Put:

<img width="582" height="297" alt="image" src="https://github.com/user-attachments/assets/1bfeed93-d764-4920-80d6-a25838de96e6" />

<img width="542" height="240" alt="image" src="https://github.com/user-attachments/assets/3ad67cc3-88e6-4db1-8080-f42e7efabc2f" />

<img width="907" height="345" alt="image" src="https://github.com/user-attachments/assets/db569cc6-9d8f-406f-9fba-85b54c9a8141" />

<img width="240" height="60" alt="image" src="https://github.com/user-attachments/assets/33acef35-87db-42ad-9f1c-f31f9ba796fd" />

Make this Notebook Trusted to load map: File -> Trust Notebook

## Key Insights

IPL matches are concentrated in major metropolitan cities.

Cities like Mumbai, Bangalore, Chennai, and Delhi host the highest number of matches.

Limited matches in smaller cities highlight infrastructure and audience concentration.

## Final Insights & Conclusion

This project demonstrated an end-to-end data analysis workflow using IPL match and ball-by-ball data, covering data loading, cleaning, feature engineering, exploratory analysis, data merging, and visualization.

## Key Insights

#### Team Performance

Certain teams have consistently outperformed others across multiple seasons, indicating strong team composition and strategy.

Match outcomes vary significantly by season, highlighting changes in team strength and playing conditions.

#### Toss Impact

While winning the toss provides a slight advantage, it does not guarantee match victory.

Strategic decisions such as batting or fielding first must be evaluated in combination with pitch conditions and team strengths.

#### Batting Analysis

High run scorers are not always the most efficient batsmen.

Strike rate provides important context when evaluating batting performance, especially for shorter formats like T20.

#### Bowling Analysis

Economy rate and dot-ball percentage are stronger indicators of bowling effectiveness than wicket count alone.

Consistent bowlers tend to restrict scoring even when they do not take many wickets.

#### Seasonal & Trend Analysis

Average runs per match have generally increased over the years, reflecting more aggressive batting approaches and evolving strategies.

Performance trends of top players vary across seasons, emphasizing the importance of consistency and adaptability.

#### Geographical Distribution

IPL matches are heavily concentrated in major metropolitan cities.

This reflects infrastructure availability, audience concentration, and commercial considerations.

## conclusion

Through this project, we applied Python-based data analysis techniques to a real-world sports dataset and extracted meaningful, business-relevant insights.
The analysis highlights how raw data can be transformed into actionable information using structured workflows and analytical thinking.

This capstone project demonstrates proficiency in:

Data cleaning and preprocessing.

Feature engineering.

Exploratory data analysis (EDA).

Data visualization (Matplotlib, Seaborn, Folium.

Merging datasets and deriving advanced insights.


Overall, this project serves as a strong portfolio example of end-to-end data analysis using Python and reflects practical skills expected in real-world data analytics roles.














































































































