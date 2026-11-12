# Amazon E-Commerce Product Analytics Dashboard

An end-to-end data analytics project exploring Amazon product catalogue
data using **Python, PostgreSQL, and Power BI**.

> **Scope note:** The dataset does not contain verified sales or
> quantity fields. This project analyzes product catalogue attributes
> and does not claim to measure sales, revenue, or units sold.

## Project Overview

This project transforms raw Amazon product data into a prepared dataset
and an interactive Power BI dashboard. The workflow includes data
cleaning, exploratory data analysis (EDA), feature engineering, database
loading, and dashboard development.

The final report contains two pages:

1.  **Executive Overview** --- a high-level view of the product
    catalogue.
2.  **Product Performance Analysis** --- product comparisons based on
    ratings, review counts, discounts, and prices.

## Objectives

-   Clean and prepare the raw product dataset.
-   Explore product categories, ratings, review counts, prices, and
    discounts.
-   Create useful derived features, including product price ranges.
-   Store and query prepared data using PostgreSQL.
-   Build an interactive two-page Power BI dashboard.
-   Present product-level patterns clearly.

## Tools and Technologies

  Tool           Purpose
  -------------- ---------------------------------------------
  Python         Data cleaning, EDA, and feature engineering
  Google Colab   Running the Python notebook
  pandas         Data manipulation
  PostgreSQL     Storing and querying prepared data
  pgAdmin        Managing the PostgreSQL database
  Power BI       Visualization and dashboard development

## Workflow

1.  **Dataset collection** --- obtained the Amazon product dataset in
    CSV format.
2.  **Data cleaning** --- inspected and prepared the data in Python
    using Google Colab.
3.  **Exploratory data analysis** --- explored the available product
    attributes and distributions.
4.  **Feature engineering** --- created derived fields, including price
    ranges: Low, Medium, High, and Premium.
5.  **Database loading** --- imported the prepared dataset into
    PostgreSQL and checked the imported records.
6.  **Power BI connection** --- connected Power BI to PostgreSQL.
7.  **Dashboard development** --- created two report pages with visuals,
    KPI cards, and slicers.

## Dashboard Pages

### 1. Executive Overview

A summary of the product catalogue, including KPI cards and visuals for
exploring products by category, price range, and rating category.

**Main elements** - Product and category summary KPIs - Average-rating
overview - Product distribution by category - Product distribution by
price range - Slicers for category, price range, and rating category

### 2. Product Performance Analysis

A product-level comparison page.

**Main elements** - Top 10 Highest Rated Products - Top 10 Most Reviewed
Products - Top 10 Highest Discount Products - Top 10 Most Expensive
Products - Supporting KPI cards for rating, reviews, discount, and price

Rankings use the relevant product attributes available in the dataset.
Interpret results according to the aggregation settings in the Power BI
report.

## Dataset

-   **Dataset:** Amazon product dataset (CSV)
-   **Record count:** Approximately 1,462 records were reported during
    the import workflow.
-   **Data domain:** Product catalogue information.

Fields used in the analysis include product name, category, rating,
rating count, actual price, final price, and discount percentage, along
with derived fields such as price range.

**Dataset source:** \[Add the original dataset name and source URL.\]

Before publishing, confirm the final record count and exact column names
against your cleaned dataset. Do not redistribute the dataset unless its
licence permits it.

## Suggested Repository Structure

``` text
Amazon-Ecommerce-Product-Analytics/
├── Dataset/
│   ├── Original_Dataset.csv
│   └── Cleaned_Dataset.csv
├── Python/
│   └── Data_Cleaning_EDA.ipynb
├── SQL/
│   └── SQL_Analysis.sql
├── PowerBI/
│   └── Amazon_Product_Analytics.pbix
├── Dashboard_Screenshots/
│   ├── Page_1_Executive_Overview.png
│   └── Page_2_Product_Performance.png
└── README.md
```

This is a suggested structure. Adjust names to match the files you
actually include; do not add empty folders just to match the example.

## How to Explore the Project

1.  Open the Python notebook in Google Colab or Jupyter Notebook to
    review data preparation and analysis.
2.  Review the SQL scripts, if included.
3.  Open the `.pbix` file in Power BI Desktop.
4.  If required, configure your own PostgreSQL connection and refresh
    the report.
5.  Use the slicers on the Executive Overview page to explore the
    dashboard.

**Security:** Do not commit database passwords, credentials, or other
secrets to a public repository.

## Key Findings

Add 3--5 findings after checking the final dashboard and underlying
data. Possible areas include:

-   Categories with the highest number of products.
-   Product distribution across the four price ranges.
-   Products ranking highest by rating or review count.
-   Differences in discounts across products.
-   Patterns between ratings, review counts, and prices.

Include only findings verified from your analysis, and add actual values
where useful.

## Limitations

-   The dataset contains product catalogue attributes, not verified
    sales or quantity data.
-   Ratings and review counts are not direct measures of sales.
-   Findings are limited to the fields and records in the dataset.
-   Document the dataset source, licence, and collection date before
    public distribution.

## Possible Future Improvements

-   Add time-based analysis if reliable historical product snapshots
    become available.
-   Compare product attributes across categories.
-   Add detailed drill-through views for individual products.
-   Automate the data refresh process.

## Author

**Abhay Tyagi**

**Project:** Amazon E-Commerce Product Analytics Dashboard\
**Focus:** Data Analytics

------------------------------------------------------------------------

Retain the dataset's original attribution and follow its licence terms
if you use or adapt this project.
