# AI Customer Intelligence and Retention Platform

## Project Status

Dataset inspection completed. Cleaning rules and valid-sale definitions are being developed.

## Project Overview

The AI Customer Intelligence and Retention Platform is a proposed digital product designed to help small retailers understand customer behaviour, identify valuable customer groups and improve repeat purchasing.

Many small businesses collect sales and customer transaction data but do not have dedicated analytics teams or accessible tools for converting that data into useful business decisions.

This project will combine product discovery, business KPIs, customer analytics, customer segmentation and an interactive dashboard.

## Business Problem

Small retailers often have difficulty answering questions such as:

- Who are our most valuable customers?
- Which customers purchase repeatedly?
- Which customers have stopped purchasing?
- Which customer groups contribute the most revenue?
- What actions could improve customer retention?
- Are sales decisions based on evidence or assumptions?

Without clear customer intelligence, businesses may spend marketing resources inefficiently and fail to retain valuable customers.

## Target Users

The primary users are:

- Small retail business owners
- E-commerce store managers
- Sales and marketing managers
- Customer relationship teams
- Small businesses without dedicated data analysts

## Proposed Product

The platform will allow a user to upload customer transaction data and receive:

- Customer and revenue KPIs
- Repeat-purchase analysis
- Customer segmentation
- Identification of high-value customers
- Identification of inactive or at-risk customers
- Retention insights
- Business recommendations
- An interactive dashboard

## Planned MVP Features

The minimum viable product will include:

1. Transaction-data upload
2. Data-quality checks
3. Revenue and customer overview
4. Repeat-purchase analysis
5. Recency, Frequency and Monetary segmentation
6. Customer-segment dashboard
7. At-risk customer identification
8. Business recommendations
9. Downloadable summary outputs

## Analytics and AI Scope

The first version will focus on reliable descriptive analytics and rule-based customer segmentation.

Planned analytical methods include:

- Recency, Frequency and Monetary analysis
- Customer-value segmentation
- Repeat-purchase measurement
- Retention and inactivity analysis
- Revenue-contribution analysis

Predictive modelling will be considered only when the available dataset, feature quality and sample size support a credible model.

The project will not claim to use advanced AI unless a working and properly evaluated predictive component is implemented.

## Planned Technology Stack

- Python
- Pandas
- SQL
- Jupyter Notebook
- Streamlit
- Matplotlib
- Git and GitHub

## Planned Business KPIs

- Total revenue
- Total orders
- Total customers
- Average order value
- Repeat-purchase rate
- Customer-retention rate
- Average purchase frequency
- Average customer recency
- Revenue by customer segment
- High-value customer contribution
- Inactive-customer rate

## Repository Structure

```text
data/          Dataset and data dictionary
docs/          Product and business documentation
notebooks/     Python analysis notebooks
sql/           SQL analysis scripts
src/           Reusable Python code
dashboard/     Streamlit application
outputs/       Charts and summary reports
README.md      Project overview
```

## Project Roadmap

### Phase 1 — Product Discovery

- [x] Define the business problem
- [x] Identify target users
- [x] Document customer pain points
- [x] Define product requirements
- [x] Define MVP features
- [x] Write user stories
- [x] Define business KPIs

### Phase 2 — Data Preparation

- [x] Select a suitable dataset
- [x] Create a data dictionary
- [x] Inspect data quality
- [ ] Define cleaning and validation rules
- [ ] Create the processed transaction dataset

### Phase 3 — Business Analysis

- Analyse revenue
- Analyse customer behaviour
- Measure repeat purchases
- Calculate retention indicators
- Segment customers

### Phase 4 — Product Prototype

- Build an interactive Streamlit dashboard
- Present customer segments
- Highlight high-value and at-risk customers
- Generate business recommendations

### Phase 5 — Evaluation and Documentation

- Validate calculations
- Document limitations
- Evaluate product usefulness
- Prepare a product roadmap
- Present stakeholder-friendly findings

