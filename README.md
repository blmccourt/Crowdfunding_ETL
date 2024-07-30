# Crowdfunding_ETL

## Background
This mini project is a practice in building an ETL pipeline using Python, Pandas, and Python dictionary methods to extract and transform data. After transforming the data,  four CSV files are created then used to create an ERD and a table schema. Finally, the CSV file data is uploaded into a Postgres database.

## Extraction and Transformation
This portion of the project is divided into the following:

1. Create the Category and Subcategory DataFrames
2. Create the Campaign DataFrame
3. Create the Contacts DataFrame

## Loading
The last portion of the project is creating the Crowdfunding database, which is divided into the following:

### Data Modeling
The six provided CSV files were analyzed and then an Entity Relationship Diagram was created using [QuickDBD](http://www.quickdatabasediagrams.com/).

### Data Engineering
Using the provided information from the ERD, a table schema was created for each table using PostgreSQL.  The CSV files were then imported into the corresponding SQL table.

### Data Analysis
Four queries were created to verify that each table has the correct data.

## Folders and Files
1. **[`ETL_Mini_Project_BMcCourt.ipynb`](https://github.com/blmccourt/Crowdfunding_ETL/blob/main/ETL_Mini_Project_BMcCourt.ipynb)**
- Jupyter notebook with the scripts for the Extraction and Transformation of data.
2. **[Resources](https://github.com/blmccourt/Crowdfunding_ETL/tree/main/Resources)**
- Folder with the two provided Excel files.
  - `contacts.xlsx`
  - `crowdfunding.xlsx`
- Four CSV files representing the exported data frames.
  - `category.csv`
  - `subcategory.csv`
  - `contacts.csv`
  - `campaign.csv`
1. **[Data Modeling](https://github.com/blmccourt/Crowdfunding_ETL/tree/main/Data%20Modeling)**
   - [`crowdfunding_db_ERD.png`](https://github.com/blmccourt/Crowdfunding_ETL/blob/main/Data%20Modeling/crowdfunding_db_ERD.png) is the image file of the Entity Relationship Diagram.
   - [`physical_schema.txt`](https://github.com/blmccourt/Crowdfunding_ETL/blob/main/Data%20Modeling/physical_schema.txt) is the text representation of the ERD.
2. **[Data Engineering](https://github.com/blmccourt/Crowdfunding_ETL/tree/main/Data%20Engineering)**
   - [`crowdfunding_db_schema.sql`](https://github.com/blmccourt/Crowdfunding_ETL/blob/main/Data%20Engineering/crowdfunding_db_schema.sql) is the file of table schemata.
   - [`crowdfunding_db_creation.png`](https://github.com/blmccourt/Crowdfunding_ETL/blob/main/Data%20Engineering/crowdfunding_db_creation.png) is the image file of creating the Postgres database.
3. **[Data Analysis](https://github.com/blmccourt/Crowdfunding_ETL/tree/main/Data%20Analysis)**
   - [`crowdfunding_queries.sql`](https://github.com/blmccourt/Crowdfunding_ETL/blob/main/Data%20Analysis/crowdfunding_queries.sql) is the file with all queries.
   - [`select_all_campaign.png`](https://github.com/blmccourt/Crowdfunding_ETL/blob/main/Data%20Analysis/select_all_campaign.png) is the image file showing the results from the SELECT * query in pgAdmin.
   - [`select_all_campaign_all_columns.png`](https://github.com/blmccourt/Crowdfunding_ETL/blob/main/Data%20Analysis/select_all_campaign_all_columns.png) is an additional image file showing all the columns created for the campaign table.
   - [`select_all_category.png`](https://github.com/blmccourt/Crowdfunding_ETL/blob/main/Data%20Analysis/select_all_category.png) is the image file showing the results from the SELECT * query in pgAdmin.
   - [`select_all_contacts.png`](https://github.com/blmccourt/Crowdfunding_ETL/blob/main/Data%20Analysis/select_all_contacts.png) is the image file showing the results from the SELECT * query in pgAdmin.
   - [`select_all_subcategory.png`](https://github.com/blmccourt/Crowdfunding_ETL/blob/main/Data%20Analysis/select_all_subcategory.png) is the image file showing the results from the SELECT * query in pgAdmin.