# Data Dictionary

## Overview
**Source:** Sample sales transaction data (sales_data_sample.csv)
**Purpose:** This data dictionary is used to categorize various fields and to ensure standardization with the data within the csv file.
**Last Updated:** [01/25/2026]

## Field Definitions

| Field Name       | Data Type | Description                           | Allowed Values                                                            | Usage Notes                                       |
|------------------|-----------|---------------------------------------|---------------------------------------------------------------------------|---------------------------------------------------|
| ORDERNUMBER      | Integer   | Unique identifier for each number     | Positive Integers                                                         | Primary key for locating and tracking orders      |
| QUANTITYORDERED  | Integer   | Number of items ordered               | Positive Integers                                                         | Used for sales calculations                       |
| PRICEEACH        | Float     | Price per individual item             | Positive Integers                                                         | In USD                                            |
| ORDERLINENUMBER  | Integer   | Line item within an order             | Positive Integers                                                         | Tracks different items within an order            |
| SALES            | Float     | Total sales amount for line item      | Positive numbers                                                          | Calculated field of Quantity Ordered * Price Each |
| ORDERDATE        | Date      | Date the order was placed             | Valid Dates                                                               | Format: [MM/DD/YYYY]                              |
| STATUS           | String    | Current Order Status                  | Shipped, In Process, Cancelled, On Hold, Disputed, Resolved               | Categorical Field                                 |
| QTR_ID           | Integer   | Quarter Identifier                    | 1, 2, 3, 4                                                                | Derived from ORDERDATE                            |
| MONTH_ID         | Integer   | Month Identifier                      | 1 through 12                                                              | Derived from ORDERDATE                            |
| YEAR_ID          | Integer   | Year Identifier                       | Valid Years                                                               | Derived from ORDERDATE                            |
| PRODUCTLINE      | String    | Product Category                      | Classic Cars, Vintage Cars, Motercycles, Trains, Trucks and Buses, Planes | Categorical Field                                 |
| MSRP             | Float     | Manufacturer's suggested retail price | Positive numbers                                                          | In USD                                            |
| PRODUCTCODE      | String    | Unique product identifier             | Alphanumeric Code                                                         | Used to identify specific products                |
| CUSTOMERNAME     | String    | Name of customer                      | Text                                                                      | Contains buinsess or individual names             |
| PHONE            | String    | customer phone number                 | Valid Phone format                                                        | may include US and international formats          |
| ADDRESSLINE1     | String    | Primary Address line                  | Text                                                                      | Street Address                                    |
| ADDRESSLINE2     | String    | Secondary address line                | Text or NULL                                                              | Apartment, Suite, etc.                            |
| CITY             | String    | City name                             | Text                                                                      | Customer city/location                            |
| STATE            | String    | State/Province                        | Text or NULL                                                              | May be NULL if non-US                             |
| POSTALCODE       | String    | Postal/ZIP code                       | Alphanumeric Code                                                         | Format differes by country                        |
| COUNTRY          | String    | Country name                          | Text                                                                      | Customer country                                  |
| TERRITORY        | String    | Sales Territory                       | NA, APC, EMEA, Japan                                                      | Geographical region                               |
| CONTACTLASTNAME  | String    | Contact last name                     | Text                                                                      | Primary contact                                   |
| CONTACTFIRSTNAME | String    | Contact first name                    | Text                                                                      | Primary contact                                   |
| DEALSIZE         | String    | Size classification for the deal      | Small, Medium, Large                                                      | Categorical based on sales amount.                |

## Calculated Fields

- **SALES**: Calculated as `QUANTITYORDERED × PRICEEACH`
- **QTR_ID**: Derived from ORDERDATE (month → quarter conversion)
- **MONTH_ID**: Extracted from ORDERDATE
- **YEAR_ID**: Extracted from ORDERDATE

## Relationships

- **ORDERNUMBER** links multiple ORDERLINENUMBER entries (one order can have multiple line items)
- **PRODUCTCODE** links to product details (PRODUCTLINE, MSRP)
- **CUSTOMERNAME** links to customer details (PHONE, ADDRESS fields, CONTACT fields)
