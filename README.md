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




