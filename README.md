# Student Banking Model Project

## Goal
Analyze different chequing account plans offered by the 5 largest Canadian banks (RBC, TD, Scotiabank, BMO, CIBC) to identify which features (fees, transaction limits, requirements) provide the highest value for student clients and create a chequing account selector model to find the most suitable banking account for different student profiles. The comparison is made calculating the first 3 years of account usage for each person to define which account is more helpful long-term depending each individual's financing patterns.

## Motivation
Choosing the right chequing account or the right bank sometimes seems like an overwhelming decision due to the large amount of options. As higher-education students are faced with several expenses such as tuition fees, rent, transportation and more, along with potentially low incomes due to low working hours, minimal wages or lack of work experience, this model aims to facilitate the selection of a chequing account for students with different needs and financial status.

This project also seeks to implement different data analysis practices in an end-to-end manner by cleaning data in excel, analyzing it in SQL and making a visual model with power BI

## Tools
- Excel
- SQL
- Power BI

The datasets and source code are provided in the repository

## Data
The main data source for this project is the [FCAC comparison tool](https://itools-ioutils.fcac-acfc.gc.ca/ACT-OCC/SearchFilter-eng.aspx) by the Government of Canada. Instead of finding a premade dataset online, the information was gathered from this tool based on the following filters: Quebec, chequing account, CAD currency, additional discounts: Student.

## Cleaning and Scoping

All the chequing accounts offered by the big 5 banks and shown on FCAC were used for this project. Due to this being a self-made dataset, I defined some limitations that would make the data verification and model easier to manage. I selected the relevant information of each account based on the most common usages of chequing accounts: included transactions, monthly fee, withdrawal fees (in-branch and atm), transfer fees (mobile and e-transfers), overdraft protection fees (per occurrence), debit card purchases (if transaction limit exceeded), bill payment fees (if transaction limit exceeded) (mobile).
The information of every account was confirmed and any missing data was gathered through the official website of each bank. 

Aspects that were common to all of the accounts were discarded as they do not provide a valuable impact on the comparison model: Account type (Chequing), Interest rate (0%), Non-Sufficient Funds charge (10$). 

For Scoping reasons, I set a few guidelines and exclusions to avoid a confusing and overly complicated model, as this is an initial concept of what may become a real model someday:
- A person's eligibility for an account is based on a snapshot of their status at the beginning of the year. E.g: if a person is 3 months post-grad in the first-year snapshot, that person is eligible for any account with > 3 months post-grad student discount, and on the second year, they will no longer be eligible.
- Welcome bonuses or in-bank benefits were excluded from this comparison due to complexity and existence of different systems (ex: point rewards, subscription benefits, etc)

## Questions
-	Do designated “student” plans provide more valuable features than regular accounts or accounts with student discounts?
-	Do higher-fee plans provide better benefits for higher-income individuals?
-	Do limited transaction plans help savings?

## Analysis
The queries are made on MySQL workbench. Still under progress...

## Visualization

Power BI, to be continued...

## Conclusion

to be continued...

