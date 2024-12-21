# Dynamic_retail_Dashboard
Dynamic Dashboard
Apologies for the oversight! Here is the updated **README** file, including the missing sample tables for **Order**, **Return**, and **People**.

---

# Dynamic Retail Dashboard

## Overview
The **Dynamic Retail Dashboard** is a comprehensive Excel-based dashboard created to provide interactive and insightful visualizations of retail sales data. By integrating multiple data sources from GitHub, such as **Order**, **People**, and **Return** tables, this dashboard allows users to dynamically analyze and monitor key retail metrics, such as total sales, profit, quantity, order trends, and much more.

Using advanced features of **Power Query Editor** and **dynamic charts**, this dashboard is designed to provide in-depth analyses for business decision-making.

## Features
- **KPI Tracking**: Dynamic tracking of key performance indicators like **Total Sales**, **Profit**, **Quantity**, **Order Count**, and more.
- **Sales & Profit Analysis**: Visual insights into sales trends and profitability across various dimensions.
- **Category-wise Profit**: Breakdown of profits by product category for targeted analysis.
- **Segment-wise Sales Share %**: Visualize how different segments contribute to total sales.
- **Sales by Country**: Geographical distribution of sales across countries.
- **Top 5 & Bottom 5 Subcategories**: Identifying the best and worst-performing subcategories.
- **Yearly Sales Trends**: Visualization of sales over the years to track growth or decline.
- **Dynamic Charts**: Automatically update charts as data is filtered based on the selection in the **KPI table**.

## Data Sources
The dashboard integrates three primary data tables:
1. **Order**: Contains all order details, including sales figures, product information, and customer details.
2. **People**: Information about sales representatives and the regions they operate in.
3. **Return**: Data on the returned orders, including the order ID and market region.

The data from these tables is automatically pulled from the GitHub repository and transformed using **Power Query Editor**.

---

### Sample Data:

#### 1. **Order Table:**
| Row ID | Order ID        | Returned | Order Date | Ship Date | Ship Mode    | Customer ID  | Customer Name   | Segment    | City           | State    | Country        | Postal Code | Market | Region  | Product ID        | Category  | Sub-Category  | Product Name                                   | Sales   | Quantity | Discount | Profit   | Shipping Cost | Order Priority |
|--------|-----------------|----------|------------|-----------|--------------|--------------|-----------------|------------|----------------|----------|----------------|-------------|--------|---------|-------------------|-----------|---------------|------------------------------------------------|---------|----------|----------|----------|---------------|----------------|
| 32298  | CA-2012-124891  | No       | 31-07-2020 | 31-07-2020| Same Day     | RH-19495     | Rick Hansen     | Consumer   | New York City  | New York | United States  | 10024       | US     | East    | TEC-AC-10003033   | Technology | Accessories   | Plantronics CS510 - Wireless Headset          | 2309.65 | 7        | 0        | 762.18   | 933.57        | Critical       |
| 26341  | IN-2013-77878   | Yes      | 05-02-2021 | 07-02-2021| Second Class | JR-16210     | Justin Ritter   | Corporate  | Wollongong     | New South Wales | Australia | APAC | Oceania | FUR-CH-10003950   | Furniture | Chairs        | Novimex Executive Leather Armchair, Black     | 3709.40 | 9        | 0.1      | -288.77  | 923.63        | Critical       |
| 25330  | IN-2013-71249   | No       | 17-10-2021 | 18-10-2021| First Class  | CR-12730     | Craig Reiter    | Consumer   | Brisbane       | Queensland | Australia      |             | APAC   | Oceania | TEC-PH-10004664   | Technology | Phones        | Nokia Smart Phone                              | 5175.17 | 9        | 0.1      | 919.97   | 915.49        | Medium         |

#### 2. **Return Table:**
| Returned | Order ID        | Market  |
|----------|-----------------|---------|
| Yes      | MX-2013-168137  | LATAM   |
| Yes      | US-2011-165316  | LATAM   |
| Yes      | ES-2013-1525878 | EU      |
| Yes      | CA-2013-118311  | United States |
| Yes      | ES-2011-1276768 | EU      |

#### 3. **People Table:**
| Person           | Region  |
|------------------|---------|
| Anna Andreadi    | Central |
| Chuck Magee      | South   |
| Kelly Williams   | East    |
| Matt Collister   | West    |
| Deborah Brumfield| Africa |
| Larry Hughes     | AMEA    |
| Nicole Hansen    | Canada  |

---

## Problem Statements Solved
This dashboard solves the following business problems and provides meaningful insights into various aspects of retail performance:

### 1. **KPIs - Total Sales, Total Profit, Quantity, Number of Orders, Profit Margin**
**Description:**  
The KPIs section provides key metrics that are essential for understanding the overall business performance. These include:
- **Total Sales**: The sum of all sales across all orders.
- **Total Profit**: The sum of profits across all orders.
- **Quantity**: The total number of items sold.
- **Number of Orders**: The total count of orders.
- **Profit Margin**: Profit divided by sales, indicating how efficiently the company is turning sales into profits.

**Visuals:**  
Insert a screenshot of the dynamic KPI section showing real-time updates of the total sales, profit, quantity, and other metrics as they change based on the data.

---

### 2. **Sales and Profit Analysis**
**Description:**  
This section provides a detailed analysis of sales and profits across different categories, regions, and time periods. It helps identify high-performing and underperforming areas.

**Visuals:**  
Include a bar or line chart visualizing sales vs. profits, potentially segmented by product category or region.

---

### 3. **Category-wise Profit**
**Description:**  
This analysis breaks down the total profits by product categories to help businesses understand which categories are the most profitable.

**Visuals:**  
Add a pie chart or bar chart showing profit distribution by category (e.g., Technology, Furniture, Office Supplies).

---

### 4. **Segment-wise Sales Share %**
**Description:**  
This visualizes the share of total sales attributed to each customer segment, such as **Consumer**, **Corporate**, or **Home Office**.

**Visuals:**  
Include a pie chart showing the percentage of sales contributed by each customer segment. You can also use a stacked bar chart for more detailed comparisons.

---

### 5. **Sales by Country**
**Description:**  
This feature helps visualize the total sales by different countries, offering insights into geographical performance.

**Visuals:**  
Insert a **Map** visualization or a bar chart that displays sales per country. This could help businesses focus on expanding or improving sales in certain countries.

---

### 6. **Top 5 Subcategories**
**Description:**  
This analysis highlights the top 5 subcategories with the highest sales, providing insights into the most popular product types.

**Visuals:**  
Include a bar chart or a table listing the **Top 5 Subcategories** by sales, showing which products are performing best.

---

### 7. **Bottom 5 Subcategories**
**Description:**  
This analysis shows the lowest 5 subcategories based on sales, highlighting areas that need attention or improvement.

**Visuals:**  
Add a table or bar chart showcasing the **Bottom 5 Subcategories** by sales.

---

### 8. **Yearly Sales Trend**
**Description:**  
Track the performance of sales over time by visualizing annual sales trends. This helps identify growth patterns and cyclical sales changes.

**Visuals:**  
Include a line chart or area chart showing the **Yearly Sales Trend** over multiple years, helping businesses forecast and plan for future periods.

---

## Dynamic Dashboard Components

- **KPI Table**: All KPIs such as total sales, total profit, total quantity, and order count are tracked dynamically using linked formulas in the KPI table.
- **Dynamic Charts**: Based on user selection in the KPI table, all charts and visuals will update automatically to reflect the data chosen, offering a real-time analysis experience.

**Visuals**:  
- Insert visuals showing the dynamic nature of the charts (before and after filtering data).

---

## Data Transformation Process (Power Query)
To ensure the data is ready for analysis, **Power Query Editor** was used to:
1. **Merge Data**: Combine the Order, People, and Return tables to create a unified data model.
2. **Data Cleaning**: Filter out unnecessary columns and rows, handle missing data, and ensure all values are correctly formatted.
3. **Calculated Columns**: Create new columns to calculate metrics such as profitability and profit margins.
4. **Dynamic Data Loading**: Link the data from the GitHub repository, so that the Excel file will automatically pull in the latest data whenever updated.

---

## Next Steps / Future Enhancements
In future updates, additional features can be incorporated to further enhance the dashboard’s capabilities:
1. **Return Analysis**: Analyze the impact of returned items on sales and profitability.
2. **Top Customer Analysis**: Identify and analyze top customers by total sales or frequency of orders.
3. **Bottom Customer Analysis**: Find low-performing customers and analyze the reasons for low sales.
4. **Segment Analysis**: Perform a detailed breakdown of sales and profitability by customer segments.
5. **Market Analysis**: Analyze the performance of different markets and regions in more detail.
6. **Product Analysis**: Investigate product performance, identifying top and bottom-selling products across different categories.

---

## Data Dictionary (Optional)

### Order Table
- **Order ID**: Unique identifier for each order.
- **Sales**: Total sales revenue for the order.
- **Profit**: Profit generated from the order.
- **Product Name**: Name of the product sold.
- **Quantity**: Number of units sold.
- **Order Date**: Date when the order was placed.

### Return Table
- **Order ID**: Unique identifier for returned orders.
- **Market**: The geographical market in which the return occurred.
- **Returned**: Indicator of whether the item was returned (Yes/No).

### People Table
- **Person**: Name of the sales representative.
- **Region**: Region assigned to the representative.

---

## How to Use the Dashboard
1. **Download the Excel File**: Clone or download the repository containing the Excel file.
2. **Data Setup**: Ensure that the data from the GitHub repository is correctly linked to the Excel file.
3. **Interact with Filters**: Use the drop-down menus and slicers to filter the data dynamically. The charts will update automatically.
4. **Visualize Results**: View the updated KPIs, charts, and tables for real-time insights into your retail performance.

---

Feel free to add the appropriate visuals in each section, such as the graphs, charts, and map snapshots, to provide a clear and interactive experience for the user.
