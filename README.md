### Canada Job Market Analysis — Power BI
# Project Overview
An interactive Power BI dashboard developed to analyze Canadian job postings and identify trends across job locations, sectors, experience levels, employment types, companies, and application activity.
The project demonstrates an end-to-end data analytics workflow including data cleaning, data modeling, DAX calculations, interactive visualization, and business insight generation.

# Objectives
1) Analyze the distribution of job opportunities across Canadian cities and provinces.
2) Identify the sectors with the highest number of job postings.
3) Understand demand across different experience levels.
4) Analyze employment types such as full-time, contract, and internship positions.
5) Identify companies with the highest number of job postings.
6) Analyze application volume and competition.
7) Build an interactive dashboard for exploring job-market trends.

# Tools & Technologies
1) Power BI
2) Power Query
3) DAX
4) Data Modeling
5) Star Schema
6) Data Visualization
7) Microsoft Excel/CSV data 

# Dataset

The dataset contains Canadian job-posting information including:

1) Job title
2) Company
3) City
4) Province
5) Employment type
6) Experience level
7) Sector
8) Published date
9) Application count

# Dataset link:-
https://www.kaggle.com/datasets/kanchana1990/linkedin-canada-data-science-jobs-2024

# Data Preparation
Data preparation was performed using Power Query.
Major transformations included:

1) Cleaning location fields
2) Handling missing values
3) Removing duplicate location records
4) Standardizing city/province information
5) Creating dimension tables
6) Creating a dedicated date table
7) Establishing relationships between fact and dimension tables

# Data Model
The project uses a star-schema model.

Fact Table

Fact_Jobs

Contains job-level transactional information such as:

1) Job ID
2) Company
3) Job title
4) Published date
5) Application count
6) Location
7) Employment type
8) Experience level

# Dimension Tables
1) Dim_Date
2) Dim_Location
3) Dim_Company
4) Dim_Employment
5) Dim_Experience
6) Dim_Sector

# Key DAX Measures

Examples of measures created:

Total Jobs = COUNTROWS(Fact_Jobs)

Total Companies = DISTINCTCOUNT(Fact_Jobs[companyId])

Average Applications =
AVERAGE(Fact_Jobs[Application Count])

Maximum Applications =
MAX(Fact_Jobs[Application Count])

Additional measures were created for analyzing cities, provinces, applications, and job trends.

# Dashboard Pages

# 1. Executive Summary

Provides a high-level overview of the dataset including:

1) Total jobs
2) Total companies
3) Total cities
4) Total provinces
5) Average applications
6) Maximum applications
7) Sector distribution
8) Experience-level distribution
9) Employment-type distribution
10) Top cities

# 2. Detailed Analysis

Provides interactive filtering and detailed job-level analysis using:

1) Province slicer
2) City slicer
3) Sector slicer
4) Experience-level slicer
5) Employment-type slicer
6) Jobs posted over time
7) Jobs by province
8) Top companies
9) Detailed job table

# 3. Job Insights

Provides deeper analysis of:

1) Jobs by employment type
2) Jobs by sector
3) Jobs by experience level
4) Average applications by experience level
5) Top 10 cities by jobs
6) Average applications
7) Maximum applications

# Key Insights

Based on the analyzed dataset:

1) Toronto has the highest number of job postings among the cities analyzed.
2) Mid-Senior level positions represent the largest experience category.
3) Full-time positions dominate the employment-type distribution.
4) Technology and software-related sectors contribute a significant share of job postings.
5) The dataset contains 340 job postings and approximately 38,423 applications.
6) The average job receives approximately 113 applications, indicating substantial competition.

# Dashboard Preview
Executive Summary

Detailed Analysis

Job Insights

# Skills Demonstrated
1) Data Cleaning
2) Power Query
3) DAX
4) Data Modeling
5) Star Schema
6) Data Visualization
7) KPI Development
8) Interactive Dashboard Design
9) Business Analysis
10) Data Storytelling

# Author

Shreya Pandey

Data Analyst | Power BI | SQL | Python
