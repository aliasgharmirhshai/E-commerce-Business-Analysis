# Olist E-commerce Dataset

This repository contains the **Olist E-commerce Dataset** in SQLite format, originally sourced from Kaggle. This dataset provides a comprehensive view of an e-commerce business by including detailed information on orders, customers, products, sellers, and reviews.

## Data Source

- **Title:** E-commerce Dataset by Olist (SQLite Database)
- **Author:** terencicp (as hosted on Kaggle)
- **Link:** [Olist E-commerce Dataset on Kaggle](https://www.kaggle.com/datasets/terencicp/e-commerce-dataset-by-olist-as-an-sqlite-database/data)
- **Format:** SQLite database

## Dataset Overview

The dataset is structured to simulate the operations of an e-commerce business and includes multiple tables that capture various aspects of the business process:

- **Orders:** Contains order records including order dates, status (delivered, canceled, etc.), and related customer IDs.
- **Customers:** Provides customer information, including customer IDs, states, and other demographic data.
- **Products:** Catalogues products with details such as product category and description.
- **Order Items:** Details each item within an order, linking orders with specific products and quantities.
- **Order Reviews:** Contains customer reviews associated with each order.
- **Sellers:** Includes information about the sellers or vendors.
- **Additional Tables:** May include other auxiliary tables like product category translations, among others.

## Getting Started

To begin exploring the dataset:
1. Download the SQLite database from the [Kaggle page](https://www.kaggle.com/datasets/terencicp/e-commerce-dataset-by-olist-as-an-sqlite-database/data).
2. Open the file using a SQLite browser (e.g., [DB Browser for SQLite](https://sqlitebrowser.org/)) or connect using programming languages like Python.
3. Explore the tables and relationships by running queries such as:
   ```sql
   SELECT name FROM sqlite_master WHERE type='table';
