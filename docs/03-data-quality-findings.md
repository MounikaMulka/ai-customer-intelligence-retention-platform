# Initial Data-Quality Findings

## 1\. Inspection Scope

This document records the initial inspection of the raw UCI Online Retail dataset.

The raw data was loaded without deleting, replacing or modifying source records.

## 2\. Dataset Structure

* Total rows: 541,909
* Total columns: 8
* Unique invoice numbers: 25,900
* Unique product codes: 4,070
* Unique identified customers: 4,372
* Unique countries: 38
* Earliest transaction date: 2010-12-01 08:26:00
* Latest transaction date: 2011-12-09 12:50:00

## 3\. Missing Values

* Rows with missing CustomerID: 135,080
* Rows with missing Description: 1,454
* Invalid or missing invoice dates: 0

Missing customer identifiers prevent reliable customer-level aggregation. However, these records may remain useful for transaction, revenue or product-level analysis.

No records were removed during inspection.

## 4\. Duplicate Records

* Complete duplicate rows after the first occurrence: 5,268

Repeated invoice numbers are not automatically duplicates because one invoice may contain several product lines.

Complete duplicate rows require further investigation before a removal rule is applied.

## 5\. Cancellations and Returns

* Cancelled transaction lines: 9,288
* Negative-quantity lines: 10,624
* Zero-quantity lines: 0

A cross-check showed that all 9,288 cancelled transaction lines had negative quantities. However, 1,336 additional negative-quantity lines did not have invoice numbers beginning with `C`.



Some of these records appear to represent stock adjustments, damaged goods, write-offs or products recorded as thrown away rather than customer cancellations. These records will therefore be classified separately during the cleaning phase.



Cancelled invoices and negative quantities may represent genuine returns or reversals. They will be separated from completed sales rather than automatically treated as invalid data.

## 6\. Price Issues

* Negative-price lines: 2
* Zero-price lines: 2,515

Zero and negative prices require investigation. They will not be replaced or removed until their likely business meaning has been reviewed.

## 7\. Preliminary Quality Risks

The initial inspection identified the following issues requiring cleaning rules:

1. Missing customer identifiers
2. Missing product descriptions
3. Complete duplicate rows
4. Cancelled invoices
5. Negative quantities
6. Zero or negative unit prices
7. Extreme quantity and price values
8. Non-product or administrative stock codes
9. Transactions that may not represent completed retail sales

## 8\. Decisions Deferred to the Cleaning Phase

The following decisions have not yet been made:

* Whether complete duplicate rows should be removed
* Whether unidentified-customer transactions should be retained for revenue analysis
* How returns and cancellations should be represented
* How zero-price records should be handled
* Whether administrative stock codes should be excluded
* Whether extreme values represent valid wholesale purchases
* Which records qualify as valid completed sales

These rules will be defined and documented before a processed dataset is created.

