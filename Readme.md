# IPL Data Analysis using PySpark

This project focuses on analyzing IPL cricket data to derive valuable insights from ball-by-ball and match-level information. Using PySpark, the project processes large datasets, applies various transformations, performs aggregations, and extracts meaningful metrics for player, team, and match analysis. Visualizations generated using Python libraries help better understand trends like top-performing batsmen, economical bowlers, toss impact, and venue-wise scores.

## Table of Contents
- [Project Overview](#project-overview)
- [Technologies Used](#technologies-used)
- [Data Sources](#data-sources)
- [Key Features](#key-features)
- [Visualizations](#visualizations)
- [Setup Instructions](#setup-instructions)
- [Future Work](#future-work)

## Project Overview
This project analyzes historical IPL data, providing insights into player performances, match outcomes, and overall team statistics. With PySpark’s distributed computing capability, the project efficiently processes large datasets and calculates important metrics like total runs, wickets, player veteran status, and high-impact deliveries. Advanced SQL queries were executed to uncover trends such as the impact of winning the toss, dismissal types, and batting performance in winning matches.

## Technologies Used
- **PySpark**: For data processing, transformations, and window functions.
- **AWS S3**: Data storage and retrieval.
- **SQL Queries**: For aggregations and analysis.
- **Matplotlib** & **Seaborn**: Visualization of key insights.
- **Pandas**: Converting PySpark DataFrames for visualization.
- **Python**: Data manipulation and visualization.

## Data Sources
The datasets used in this analysis include:
- Ball-by-ball data
- Match details
- Player statistics
- Team details

These datasets are stored in **AWS S3** and are processed using PySpark for analysis.

## Key Features
- **Data Ingestion**: Read CSV files from AWS S3 using PySpark.
- **Data Transformation**: Clean and filter ball-by-ball data to include only valid deliveries.
- **Window Functions**: Calculate running totals for match scores and over-based analysis.
- **Aggregations**: Compute total runs, average runs, and wickets per match and season.
- **Player Analysis**: Normalize player names, categorize players by batting style and veteran status.
- **SQL Queries**: Execute complex SQL queries to analyze top batsmen, economical bowlers, and toss impact.
- **Conditional Columns**: Flag high-impact deliveries and categorize win margins.

## Visualizations
The project includes the following visualizations:
- **Economical Bowlers**: Most economical bowlers in powerplay overs.
- **Toss Impact**: Visualizing toss winners and their match outcomes.
- **Venue Score Distribution**: Analyzing average and highest scores across venues.
- **Dismissal Types**: Frequency of different dismissal types.
- **Team Toss Performance**: Performance of teams after winning the toss.

### 1. Economical Bowlers in Powerplays
This visualization showcases the most economical bowlers during powerplay overs.
![Economical Bowlers](images/economical_bowlers.png)

### 2. Toss Impact on Match Outcomes
This graph demonstrates how winning the toss affects match outcomes.
![Toss Impact](images/toss_impact.png)

### 3. Venue-wise Average and Maximum Scores
A venue-based analysis of average and maximum scores across different IPL grounds.
![Venue Scores](images/venue_scores.png)

### 4. Player Performance Analysis
An analysis of individual player performances across multiple seasons, focusing on consistency and key contributions.
![Player Performance](images/average_runs_batsmen.png)

### 5. Team Toss Performance
An overview of how teams perform after winning the toss, showcasing win rates based on toss outcomes.
![Team Toss Performance](images/team_toss_performance.png)

### 6. Dismissal Types
This chart visualizes the frequency of different types of dismissals in IPL matches.
![Dismissal Types](images/dismissal_types.png)

## Setup Instructions
1. **Clone the repository**.

2. **Install required dependencies:**

   ```bash
   pip install pyspark matplotlib seaborn pandas

## Future Work
Adding more advanced visualizations, such as batting partnerships and bowler vs batsman matchups.
Integration of machine learning models for performance prediction.
