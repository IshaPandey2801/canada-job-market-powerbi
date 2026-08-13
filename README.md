## Canada Job Market Analysis — Power BI
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

Job title
Company
City
Province
Employment type
Experience level
Sector
Published date
Application count

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

Job ID
Company
Job title
Published date
Application count
Location
Employment type
Experience level

# Dimension Tables
Dim_Date
Dim_Location
Dim_Company
Dim_Employment
Dim_Experience
Dim_Sector

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

Total jobs
Total companies
Total cities
Total provinces
Average applications
Maximum applications
Sector distribution
Experience-level distribution
Employment-type distribution
Top cities

# 2. Detailed Analysis

Provides interactive filtering and detailed job-level analysis using:

Province slicer
City slicer
Sector slicer
Experience-level slicer
Employment-type slicer
Jobs posted over time
Jobs by province
Top companies
Detailed job table

# 3. Job Insights

Provides deeper analysis of:

Jobs by employment type
Jobs by sector
Jobs by experience level
Average applications by experience level
Top 10 cities by jobs
Average applications
Maximum applications

# Key Insights

Based on the analyzed dataset:

Toronto has the highest number of job postings among the cities analyzed.
Mid-Senior level positions represent the largest experience category.
Full-time positions dominate the employment-type distribution.
Technology and software-related sectors contribute a significant share of job postings.
The dataset contains 340 job postings and approximately 38,423 applications.
The average job receives approximately 113 applications, indicating substantial competition.

# Dashboard Preview
Executive Summary
Detailed Analysis
Job Insights

# Skills Demonstrated
Data Cleaning
Power Query
DAX
Data Modeling
Star Schema
Data Visualization
KPI Development
Interactive Dashboard Design
Business Analysis
Data Storytelling

# Author

Shreya Pandey
Data Analyst | Power BI | SQL | Python
