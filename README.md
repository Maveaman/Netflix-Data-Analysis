# Netflix-Data-Analysis

## Project Overview

This repository presents the findings from an extensive analysis of Netflix data aimed at uncovering viewer behaviors, content trends, and strategic insights to optimize content strategies and enhance user experience on the platform.

## Objectives

- **Improve Data Quality:** Through cleaning and normalization.
- **Analyze Genre Preferences and Director Contributions**
- **Provide Actionable Insights:** For strategic decision-making at Netflix.

## Scope

The project encompasses data collection, cleaning, preparation, storage, and in-depth analysis using SQL queries to address key business questions related to content production, audience engagement, and operational efficiency.

## Data Collection and Loading

### Data Sources

- A comprehensive Netflix dataset containing information about movies, TV shows, directors, genres, countries, duration, and ratings.

### Data Loading Process

- Imported data into Python for initial preprocessing and then transferred it to SQL Server for storage and subsequent analysis.

## Data Cleaning and Preparation

### Handling Foreign Characters

- Modified the data type of the "Title" column to 'nvarchar' to accommodate foreign characters.

### Removing Duplicates

- Implemented procedures to eliminate duplicate entries, enhancing data integrity and reliability.

### Data Type Conversions

- Converted the "Date Added" column from varchar to date for consistent date handling and analysis.

### Populating Missing Values

- Utilized the director column to populate missing values in the "Country" column.
- Corrected misattributed values in the "Duration" column using a CASE statement.

### Creating Separate Tables for Multi-Value Columns

- Established separate tables for multi-value attributes such as "Listed In," "Director," "Country," and "Cast" to optimize data organization and querying efficiency.

## Data Storage and Management

### Raw Data Layer

- Stored initial data imports for preservation and future reference.

### Final Staging Layer

- Maintained cleaned and transformed data, prepared for detailed analysis and reporting.

## Data Analysis Using SQL

### Director Analysis

- **Count of Movies and TV Shows by Director:** Identified Rajiv Chilaka as the director with the highest number of movies released in 2021 (17 movies) and Jan Suter in 2018 (12 movies).
- **Directors Creating Both Horror and Comedy Movies:** Identified 55 directors who have created both horror and comedy movies, with Poj Arnon and Kevin Smith noted for substantial contributions to both genres.

### Genre and Country Insights

- **Country with the Highest Number of Comedy Movies:** Determined that the United States leads with 685 comedy movies.
- **Average Duration of Movies by Genre:** Found that classic movies have the longest average duration (118 minutes), while other genres have shorter average durations.

### Yearly Release Analysis

- Analyzed yearly releases to identify trends in directorial output, supporting strategic planning and content scheduling decisions.

## Insights and Results

### Key Findings

- **Content Preferences:** Highlighted the popularity of comedy movies in the United States.
- **Directorial Excellence:** Recognized prolific directors and their impact on Netflix’s content diversity and viewer engagement.
- **Genre Analysis:** Provided insights into viewer preferences based on genre and average duration.

### Business Implications

- **Strategic Content Acquisition:** Recommends focusing on acquiring comedy content from the United States to meet viewer demand.
- **Director Partnerships:** Suggests collaborating with directors like Rajiv Chilaka and Jan Suter to diversify content offerings and enhance viewer engagement.
- **Optimized Content Length:** Proposes balancing the catalog with varying movie durations to cater to diverse viewer preferences and maximize engagement.

## Appendices

### SQL Queries

Detailed SQL queries used for data analysis and insights generation can be found on https://github.com/Maveaman

### Data Dictionary

**Table: Netflix**

**Columns:**

- show_id
- type
- title
- director
- cast
- country
- date_added
- release_year
- rating
- duration
- listed_in
- description
