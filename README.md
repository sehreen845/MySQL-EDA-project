Exploratory Data Analysis (EDA) on Layoff Data
Project Overview
This project performs Exploratory Data Analysis (EDA) on a global dataset of layoffs to uncover trends, patterns, and insights. The dataset includes information about layoffs across industries, companies, and countries, along with details such as total layoffs, percentage of workforce laid off, company funding, and more.

Objective
Analyze trends in layoffs across industries, countries, and years.
Identify significant patterns, such as companies with the highest layoffs and startups that ceased operations.
Explore outliers, such as companies with 100% layoffs or unexpectedly high layoffs relative to funding.
Dataset
The dataset layoffs_staging2 contains the following key attributes:

Company: Name of the company.
Date: Date of the layoff event.
Total_Laid_Off: Total number of employees laid off.
Percentage_Laid_Off: Percentage of the company’s workforce laid off.
Funds_Raised_Millions: Amount of funding raised by the company (in millions).
Location, Country, Industry, Stage: Additional metadata about companies.
Queries Performed
Basic Exploration:

Retrieved max/min layoffs and examined trends in percentage layoffs.
Identified companies with 100% layoffs (e.g., startups that went out of business).
Group Analysis:

Summarized layoffs by location, industry, company, and stage to identify patterns.
Ranked companies with the largest layoffs per year using window functions.
Temporal Trends:

Analyzed layoffs over time to compute rolling totals and yearly comparisons.
Outliers:

Found anomalies, such as startups raising millions yet shutting down completely (e.g., Quibi).
Key Insights
Companies in the tech industry, especially startups, experienced the highest layoffs during certain years.
Countries like the USA accounted for the largest layoffs globally.
Some companies raised significant funding yet laid off their entire workforce, pointing to unsustainable business models.
Rolling totals helped uncover peak periods of layoffs across the dataset timeline.
Technologies Used
SQL: For querying and analyzing the dataset in detail.
Database: Analysis performed on the world_layoffs.layoffs_staging2 database.
