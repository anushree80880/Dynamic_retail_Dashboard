# Steps to Solve Problem Statements

## 1. **KPIs - Total Sales, Total Profit, Quantity, Number of Orders, Profit Margin**
### Steps:
1. **Load Data:**
   - Import the **Order** table into Excel using **Power Query**.
   - Ensure that fields like **Sales**, **Profit**, **Quantity**, and **Order ID** are available in your data model.
  
2. **Create PivotTables:**
   - Insert a **PivotTable** to calculate the total values for **Sales**, **Profit**, and **Quantity**.
   - For the **Number of Orders**, use the **Count of Order ID**.
   - Create a calculated field in the PivotTable for **Profit Margin**:  
     `Profit Margin = (Total Profit / Total Sales)`.

3. **Design KPIs:**
   - Set up a section where the **Total Sales**, **Total Profit**, **Quantity**, **Number of Orders**, and **Profit Margin** will be displayed as dynamic KPIs.
   - Link the KPIs to the corresponding PivotTable values so they update automatically based on filtering.

4. **Visualize:**
   - Create **KPI cards** to display the calculated values prominently on the dashboard. For example, use text boxes and data labels to show total sales and profit.
  
---![image](https://github.com/user-attachments/assets/fb6a4b7e-7479-4353-90dc-a3c6a5c73ae8)


## 2. **Sales and Profit Analysis**
### Steps:
1. **Load Data:**
   - Import the **Order** table into Excel using **Power Query** and ensure it includes necessary fields such as **Sales** and **Profit**.

2. **Create PivotTables:**
   - Insert a **PivotTable** with **Sales** and **Profit** as values.
   - Add **Product Category** (or other dimensions like **Region**, **Segment**) to rows or columns to segment the data.

3. **Create Visuals:**
   - Insert a **bar chart** or **line chart** to display sales and profit trends over time or by category.
   - Use a **stacked bar chart** to compare sales and profit by category side by side.

4. **Analyze:**
   - Use conditional formatting or a **scatter plot** to identify areas where the sales-to-profit ratio is low, indicating potential inefficiencies.

![image](https://github.com/user-attachments/assets/8e235556-7b31-4e3d-a5cb-2e530089c5a5)


## 3. **Category-wise Profit**
### Steps:
1. **Load Data:**
   - Import the **Order** table, ensuring that fields like **Category**, **Sales**, and **Profit** are available.

2. **Create PivotTables:**
   - Insert a **PivotTable** with **Category** in the rows.
   - Sum **Profit** for each category.

3. **Create a Visual:**
   - Create a **bar chart** or **pie chart** to display **Profit** by **Category**.
   - This chart will show which categories are the most profitable.

4. **Analyze:**
   - Highlight top-performing categories and investigate the reasons behind their higher profitability.

![image](https://github.com/user-attachments/assets/0e77fe37-1ecd-46ea-be42-e33cc11ca67e)



## 4. **Segment-wise Sales Share %**
### Steps:
1. **Load Data:**
   - Import the **Order** table to get fields like **Segment** and **Sales**.

2. **Create PivotTables:**
   - Insert a **PivotTable** with **Segment** as rows and sum of **Sales**.
   - Create a calculated field to show the **Sales Share %** for each segment:
     - Formula: `Sales Share % = (Sales for Segment / Total Sales) * 100`

3. **Create a Visual:**
   - Create a **pie chart** to display the sales share by **Segment**.
   - This chart will show which segments contribute the most to overall sales.

---![image](https://github.com/user-attachments/assets/5cbbc26e-3890-4d3c-bc53-8dfde602077a)


## 5. **Sales by Country**
### Steps:
1. **Load Data:**
   - Import the **Order** table, ensuring that the **Country** and **Sales** fields are present.

2. **Create PivotTables:**
   - Insert a **PivotTable** with **Country** as rows and **Sales** as values.

3. **Create a Visual:**
   - Use a **map chart** (available in Excel) to display **Sales by Country** on a geographical map.
   - Alternatively, create a **bar chart** to show total sales by country in descending order.

4. **Analyze:**
   - Focus on the countries with the highest and lowest sales and investigate underlying causes.

---![image](https://github.com/user-attachments/assets/36f0eac0-df5b-4bd4-bf21-d45edbc79ff4)


## 6. **Top 5 Subcategories**
### Steps:
1. **Load Data:**
   - Import the **Order** table and ensure **Sub-Category** and **Sales** are available.

2. **Create PivotTables:**
   - Insert a **PivotTable** with **Sub-Category** as rows and **Sales** as values.
   - Sort the **Sales** column in descending order.

3. **Create a Visual:**
   - Use a **bar chart** or **column chart** to show the top 5 subcategories by sales.
   - Ensure the chart updates dynamically if the data is filtered by other parameters (e.g., year or region).

4. **Analyze:**
   - Identify which subcategories are performing the best and investigate factors driving their success.

---![image](https://github.com/user-attachments/assets/0a9f9572-6b06-4204-a64b-d8c1fc8660ea)


## 7. **Bottom 5 Subcategories**
### Steps:
1. **Load Data:**
   - Import the **Order** table, ensuring **Sub-Category** and **Sales** are included.

2. **Create PivotTables:**
   - Insert a **PivotTable** with **Sub-Category** in rows and **Sales** in values.
   - Sort the **Sales** column in ascending order.

3. **Create a Visual:**
   - Use a **bar chart** or **column chart** to display the bottom 5 subcategories by sales.
   - Like the top 5 chart, this should update dynamically based on filtering.

4. **Analyze:**
   - Focus on the bottom-performing subcategories and evaluate potential causes for their low sales performance.

---![image](https://github.com/user-attachments/assets/0a28a069-b806-436a-b1b7-4e9d9e00ba11)


## 8. **Yearly Sales Trend**
### Steps:
1. **Load Data:**
   - Import the **Order** table and ensure that **Sales** and **Order Date** are available.

2. **Create PivotTables:**
   - Insert a **PivotTable** with **Order Date** (grouped by year) in rows and **Sales** in values.

3. **Create a Visual:**
   - Create a **line chart** or **area chart** to show the trend of sales over time.
   - This chart will highlight fluctuations and trends in yearly sales.

4. **Analyze:**
   - Observe whether there are any noticeable trends (e.g., seasonal spikes or downturns in sales).

---![image](https://github.com/user-attachments/assets/3bf842b6-7b6c-469c-b741-d7ef4370f38b)


## Additional Steps for Dynamic Dashboard:

### Dynamic Charts & Interactivity:
- Use **Excel slicers** and **timeline filters** to enable users to filter by **Region**, **Segment**, **Product Category**, etc. The charts and KPIs will automatically update based on the filters selected.

### Data Transformations:
- Use **Power Query Editor** to clean and transform your data before loading it into Excel. This can include:
  - **Merging tables**: Combine data from the **Order**, **Return**, and **People** tables.
  - **Filtering data**: Remove any rows or columns not needed for the analysis.
  - **Creating calculated columns**: For instance, calculating **Profit Margin**, **Sales Share %**, etc.

### Final Visualization:
- Place your **charts**, **KPIs**, and **PivotTables** on a dashboard sheet.
- Organize your visuals neatly for easy access.
- Add a **Map chart** for geographical data like **Sales by Country**.

![image](https://github.com/user-attachments/assets/6bfccef2-f96b-4792-bca4-053948abaec1)


