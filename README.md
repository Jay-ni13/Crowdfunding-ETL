# Crowdfunding-ETL
## Project Overview
Creating a PostgreSQL database for Independent Funding--a rapidly growing crowdfunding platform for funding independent projects or ventures--to provide their analytics team with a basis to perform analyses and create reports for company stakeholders as well as individuals who donate to projects.

## Resources
 - Data Source: Independent Funding files; crowdfunding.xlsx
 - Software: Python v3.7.13, Jupyter Notebook v6.4.8, PostgreSQL v11.17, pgAdmin 4 v6.15
 
## Summary
 After utilizing Python, Pandas, and Jupyter Notebook to extract the raw data from the Crowdfunding Excel file, the data was cleaned and transformed into Pandas DataFrames and readable csv files:
  - campaign.csv
  - contacts.csv
  - backers.csv
  - category.csv
  - subcategory.csv

These datasets were used to create an ERD in QuickDBD:

![Crowdfunding DB Relationships](https://github.com/Jay-ni13/Crowdfunding-ETL/blob/main/crowdfunding_db_relationships.png)

The schema was then uploaded to PostgreSQL where are Crowdfunding Database is now housed. The first project we sourced in the new database was to determine which live campaigns were still in need of funding, how much funding was required, and the company contact who needed to be updated on their campaign's progress.

<img src="https://github.com/Jay-ni13/Crowdfunding-ETL/blob/main/Resources/email_contacts_remaining_goal_amount.png" width=80%>

As a supplement to this project, the backers for each campaign were emailed to let them know how much of the goal remains for the live campaigns that they’ve pledged, and when those campaigns will close.

![Email Backers Remaining Goal Amount](https://github.com/Jay-ni13/Crowdfunding-ETL/blob/main/Resources/email_backers_remaining_goal_amount.png)
