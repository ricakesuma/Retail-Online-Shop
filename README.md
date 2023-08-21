# The Total Sales of Retail Online Shop

### Introduction
Due to the distribution of goods across multiple regions, there is a need to determine if there are any anomalies in the available data. Additionally, insights need to be derived from the data in order to provide recommendations to users within your company.

### Data Overview
The dataset is stored in a database file, possibly in DB or SQL format. It consists of multiple tables, each containing different pieces of information. A comprehensive understanding of the data will require performing table joins to combine related information from different tables.
Certainly! Below are the tables describing the variables from the dataset. These can be used in a GitHub repository to provide a clear understanding of the data structure:

### Data Overview

#### Table: `bill_locations`
| Variable   | Description                            |
|------------|----------------------------------------|
| loc_ID     | Unique ID of the transaction location  |
| bill_ID    | Unique transaction ID                  |
| address    | Address of the transaction location    |
| latitude   | Latitude of the transaction location   |
| longitude  | Longitude of the transaction location  |
| town/city  | Town/City of the transaction location  |
| country    | Country of the transaction location    |

#### Table: `bills`
| Variable   | Description                  |
|------------|------------------------------|
| bill_ID    | Unique transaction ID        |
| invoice    | Transaction code             |
| bill_date  | Transaction date              |

#### Table: `bill_items`
| Variable      | Description                                                     |
|---------------|-----------------------------------------------------------------|
| bill_item_ID  | Unique ID for each transaction item                             |
| bill_ID       | Unique transaction ID                                           |
| product_ID    | Unique product ID                                               |
| quantity      | Quantity of items purchased                                     |
| selling_price | Selling price per unit (in USD)                                 |
| total_sales   | Total price to be paid = quantity * selling_price (in USD)       |

#### Table: `main_categories`
| Variable      | Description                  |
|---------------|------------------------------|
| category_ID   | Unique ID of category type   |
| category_name | Category name                |

#### Table: `sub_categories`
| Variable         | Description              |
|------------------|--------------------------|
| subcategory_ID   | Unique ID of subcategory  |
| subcategory_name | Subcategory name         |

#### Table: `brand_details`
| Variable    | Description                                           |
|-------------|-------------------------------------------------------|
| brand_ID    | Unique ID of brand/label                              |
| brand_name  | Brand/label name                                      |
| company     | Company name of the product (Note: 1 brand can be owned by several companies) |

#### Table: `products`
| Variable        | Description                  |
|-----------------|------------------------------|
| product_ID      | Unique product ID            |
| product_name    | Product name                 |
| brand_ID        | ID of brand/label            |
| category_ID     | ID of category type          |
| subcategory_ID  | ID of subcategory type       |

### Step-by-Step Analysis
1. **Connect Colab to Google Drive**: Setting up the connection to access the data.
2. **Import Packages**: Importing necessary Python libraries for analysis.
3. **Connect SQLite to Python**: Establishing a connection to the SQLite database.
4. **Data Preparation Using SQL**: Preparing and cleaning the data using SQL queries.
5. **Data Preparation Using Python**: Further data cleansing, manipulation, and handling outliers in Python.
6. **Exploratory Data Analysis & Visualization**: Conducting EDA to understand the data and visualize key patterns.
7. **Recommendations**: Providing actionable insights and recommendations based on the analysis.

### Interpretation
The analysis seems to involve working with a complex dataset stored in a relational database. The process includes various stages of data preparation, both in SQL and Python, followed by exploratory analysis to uncover insights. The problem statement emphasizes the need for table joins to gain a comprehensive understanding of the data.

### Business Recommendations
1. **Improve Website User Experience**: Focus on enhancing the user interface, navigation, and overall user experience to attract and retain users.
2. **Data-Driven Decision Making**: Utilize the insights gained from the analysis to make informed decisions and strategize effectively.
3. **Optimize Operations**: If applicable, the insights may help in optimizing operations, identifying areas for improvement, and implementing best practices.
