# Dataset Selection

## 1. Selected Dataset

**Dataset name:** Online Retail  
**Source:** UCI Machine Learning Repository  
**Creator:** Daqing Chen  
**Subject area:** Business  
**Dataset type:** Transactional, multivariate, sequential and time-series data  
**Number of records:** 541,909  
**Time period:** 1 December 2010 to 9 December 2011  
**File format:** Microsoft Excel  
**Licence:** Creative Commons Attribution 4.0 International

Official source:

https://archive.ics.uci.edu/dataset/352/online+retail

DOI:

https://doi.org/10.24432/C5BW33

## 2. Dataset Description

The dataset contains transaction-level records from a UK-based online retailer.

The retailer primarily sold gift products, and some customers were wholesale buyers.

Each row represents one product line within a customer invoice rather than one complete order.

The dataset includes:

- Invoice number
- Product code
- Product description
- Quantity
- Invoice date and time
- Unit price
- Customer identifier
- Customer country

## 3. Reason for Selecting the Dataset

The dataset was selected because it supports the customer-intelligence and retention objectives of this project.

It can be used to analyse:

- Total revenue
- Customer purchasing behaviour
- Repeat purchases
- Customer inactivity
- Purchase frequency
- Customer recency
- Customer monetary value
- Customer segmentation
- Revenue contribution
- Product performance
- Country-level performance
- Cancelled transactions
- Data-quality problems

## 4. Alignment with the Product

The proposed product is designed for small retailers that possess transaction records but lack accessible customer-analytics tools.

This dataset provides a realistic transaction structure containing customers, products, orders, dates, quantities and prices.

It therefore supports the planned minimum viable product features:

1. Transaction-data validation
2. Customer and revenue KPIs
3. Repeat-purchase analysis
4. RFM customer segmentation
5. High-value customer identification
6. Inactive-customer identification
7. Product and country analysis
8. Interactive dashboard development
9. Business recommendations

## 5. Why Online Retail II Was Not Selected

The Online Retail II dataset contains more than one million records across two years.

Although the larger dataset may support more extensive analysis, the additional volume is not required for the first product prototype.

The selected Online Retail dataset provides sufficient transaction history for customer segmentation and retention analysis while remaining more manageable for data cleaning, SQL analysis, Python processing and dashboard development.

## 6. Privacy and Responsible Use

The published variables do not contain customer names, email addresses, telephone numbers or postal addresses.

Customer records are represented using customer identifiers.

The project will not attempt to identify individuals or combine the dataset with external personal information.

The repository will clearly credit the original dataset creator and the UCI Machine Learning Repository.

## 7. Known and Potential Data-Quality Issues

The following conditions will be tested during data inspection:

- Missing customer identifiers
- Missing product descriptions
- Duplicate transaction rows
- Cancelled invoices
- Returned products
- Negative quantities
- Zero or invalid unit prices
- Incorrect date types
- Invalid customer identifiers
- Unusual product codes
- Extreme transaction values
- Customers with only cancelled transactions

No rows will be removed until the business meaning of each issue has been examined.

## 8. Planned Analytical Unit

The raw dataset is recorded at product-line level.

Different analyses will require different levels of aggregation:

- **Transaction-line level:** product and data-quality analysis
- **Invoice level:** order and average-order-value analysis
- **Customer level:** RFM and customer segmentation
- **Monthly level:** revenue trends and retention analysis
- **Country level:** geographic performance analysis

## 9. Attribution

This project uses the following dataset:

Chen, D. (2015). Online Retail [Dataset]. UCI Machine Learning Repository.

DOI: https://doi.org/10.24432/C5BW33

Licensed under the Creative Commons Attribution 4.0 International licence.
