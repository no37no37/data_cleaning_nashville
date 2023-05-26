# Data Cleaning Project on SQL
This project focused on data cleaning in SQL and aimed to provide a practical demonstration of 
how to clean and preprocess data for analysis. The project utilized a dataset called "Nashville Housing Data" 
and covered various data cleaning tasks using SQL queries.

# Dataset Overview
The "Nashville Housing Data" dataset was used for this project. It contained information such as unique IDs, 
parcel IDs, property addresses, sales dates, home prices, owner details, and additional property information. 
The dataset was in an Excel format and was imported into SQL for further processing.

# Data Import
The dataset was imported into SQL using Microsoft SQL Server 2019 Import and Export functionality. 
The process involved selecting the Excel file as the data source and configuring the destination as the SQL server. 
The data was copied from the "Sheet1" of the Excel file into the "nashville housing" table in the database.

# Cleaning Data
a. Standardizing Sale Date
The first data cleaning task focused on standardizing the sale date format. The sale date column contained both date 
and time information, which was unnecessary for analysis. A SQL query was used to convert the sale date to a date format 
and remove the time component.

b. Populating Property Address
The project addressed the issue of missing property addresses in the dataset. By analyzing the dataset, it was observed 
that the property addresses could be populated by leveraging the parcel ID. SQL queries were utilized to join the dataset 
with itself based on the parcel ID and populate the missing property addresses using the available information.

c. Separating Owner Address Components
Another data cleaning task involved separating the owner address components, namely address, city, and state. The owner 
address column contained combined information, making it challenging to analyze. Through SQL queries, the dataset was processed 
to break down the owner address into individual columns, allowing for better analysis and understanding.

d. Handling Blank Property Addresses
The project also addressed the issue of blank property addresses. Some entries in the dataset had missing property addresses, 
which needed to be populated. An innovative approach was taken to populate the blank property addresses using the parcel ID 
as a reference point. SQL queries were used to update the blank property addresses with the corresponding addresses from 
other entries with the same parcel ID.

e. Cleaning "Sold as Vacant" Field
The "Sold as Vacant" field required cleaning and standardization. SQL queries were employed to perform case statements and 
transform the values in the field based on certain conditions. This allowed for consistent and accurate representation of 
the "Sold as Vacant" information.

f. Removing Duplicates
Duplicates within the dataset can cause discrepancies and inaccuracies in analysis. To ensure data integrity, SQL queries were 
used to identify and remove duplicate entries from the dataset. This step helped streamline the dataset and eliminate redundancy.

g. Deleting Unused Columns
To optimize the dataset and reduce unnecessary data, unused columns were removed. SQL queries were written to delete the columns 
that were not required for further analysis. This step helped declutter the dataset and focus on the relevant information.

# Conclusion
The data cleaning project provided a practical demonstration of cleaning and preprocessing data using SQL queries. 
The tasks covered various aspects, including standardizing dates, populating missing information, separating address components, 
handling blank values, cleaning specific fields, removing duplicates, and deleting unused columns. 
