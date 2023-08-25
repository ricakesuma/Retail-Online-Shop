# The Total Sales of Retail Online Shop

### Introduction
In today's rapidly evolving digital age, online retail shopping has burgeoned into a force to be reckoned with, accounting for a significant portion of global sales. E-commerce platforms have transformed the way consumers shop, offering unparalleled convenience, a wider array of choices, and often, more competitive prices. With this transformation, businesses have recognized the imperative need to analyze and understand the intricacies of their online operations. This is essential not only to remain competitive but also to offer consumers an unparalleled shopping experience.

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
Our comprehensive analysis of the online retail shop data has shed light on several key insights that can guide future business decisions. Topping the charts in terms of overall sales, **Hindustan Unilever Limited** has proven its dominant market presence and clear favorability among consumers. On a regional scale, **New York** stands out as a hotspot for online retail sales, suggesting a dense consumer base and potential strategic marketing efforts that resonate with the city's populace. Delving deeper into product preferences, a clear trend towards convenience and household essentials emerges. **Biscuit Core & Non Core** leads the pack, highlighting a penchant for versatile snacks. This is closely followed by **Washing Powder**, indicating a consistent demand for household necessities. **Packaged Tea** underscores a substantial community of tea enthusiasts, while the popularity of **Vermicelli** hints at its role in favored dishes. **Salty Snacks** round off the top five, reinforcing the trend towards easy, ready-to-consume food items. In the realm of brand-specific sales, **Amul** has distinguished itself with its top-selling product, a testament to its esteemed reputation and quality offerings. Lastly, the brand **Marie Gold** has registered significant sales, showcasing its strong brand appeal and a loyal customer following. These revelations provide invaluable direction for businesses to refine their strategies, catering more effectively to prevailing consumer preferences.

### Business Recommendations
1. **Strengthen Partnerships with Leading Brands:**  
   Given the dominance of **Hindustan Unilever Limited** and the popularity of brands like **Amul** and **Marie Gold**, it would be strategic to strengthen partnerships with these brands. This could involve exclusive product launches, bundled offers, or loyalty programs to capitalize on their existing customer base.
2. **Focus on High-Demand Categories:**  
   The top-selling products, such as biscuits, washing powder, and packaged tea, indicate categories that are in high demand. Allocating more marketing budget, offering promotions, and ensuring consistent stock availability for these products can boost sales.
3. **Tailor Marketing Efforts for New York:**  
   Since New York has emerged as a significant market, it may be beneficial to tailor marketing and promotional efforts to cater to this city specifically. Understanding the unique preferences and needs of New York consumers can lead to more effective campaigns.
4. **Expand Snack Variety:**  
   The popularity of biscuits and salty snacks suggests a potential market for other snack-related products. Consider expanding the variety, including healthier options or introducing international snack brands to cater to a broader audience.
5. **Enhance Personalized Recommendations:**  
   Harnessing data analytics can help in providing more accurate product recommendations to customers. By analyzing purchase histories and browsing patterns, the platform can suggest items that a customer is more likely to purchase.
6. **Invest in Regional Insights:**  
   Beyond New York, understanding regional preferences can be a game-changer. For instance, if vermicelli is popular in certain regions, it might be due to specific cultural dishes. Catering promotions or bundles around regional festivals or events can drive sales.
7. **Loyalty and Retention Programs:**  
   Given the competition in the online retail space, offering loyalty programs can incentivize repeat purchases. This could be in the form of discounts, early access to sales, or exclusive products for loyal customers.
8. **Optimize Mobile Experience:**  
   As a significant portion of online shopping is now done via mobile devices, ensuring a seamless mobile shopping experience is crucial. This includes a user-friendly interface, quick load times, and secure payment gateways.
9. **Engage with Customers:**  
   Regularly seek feedback from customers to understand their needs and preferences. This can be done through surveys, reviews, or interactive social media campaigns.
10. **Sustainable and Eco-friendly Options:**  
   With a growing emphasis on sustainability, offering eco-friendly products or packaging can appeal to environmentally-conscious consumers.

