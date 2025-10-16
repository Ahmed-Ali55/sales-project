# 📊 Sales Analysis Project (Excel Power Query + Power Pivot + Power BI)

## 📘 Overview
This project focuses on analyzing sales performance to uncover key insights related to sales trends, categories, regions, and customer behavior.  
The dataset was sourced online, cleaned, transformed, and modeled using *Excel Power Query* and *Power Pivot, and visualized through an interactive **Power BI Dashboard*.

---

## 🧰 Tools & Technologies
- *Excel Power Query* – For data cleaning and transformation  
- *Excel Power Pivot* – For data modeling and creating relationships  
- *Power BI* – For visualization and dashboard design  

---

## 📂 Files Included
| File | Description |
|------|--------------|
| raw_data.xlsx | The original dataset before any processing |
| clean_data.xlsx | Cleaned and structured data after Power Query transformations |
| sales_dashboard.pbix | The Power BI dashboard showing the final visualizations |

---

## 🧮 Data Preparation and Cleaning

The dataset initially contained all data in a single sheet.  
Using *Power Query*, the data was split, cleaned, and transformed as follows:

- *Split the dataset* into multiple tables (Fact and Dimensions) using duplicate queries.  
- *Removed duplicates* in dimension tables to ensure data integrity.  
- *Renamed* and *retyped* columns for consistency and readability.  
- Created conditional columns to:
  - Calculate Sales, Profit, and Quantity *only for non-returned orders*.  
- Created a *Custom Column* to calculate the cost of goods sold (Sales * Discount).  
- Added columns for:
  - Discount Value  
  - Discount Percent (for sold orders only)  
- Built a *Date Dimension Table* from Order Date and generated:
  - Year, Month, Day  
  - Month Name  
  - Quarter  
  - Month-Year (merged Month and Year)  

---

## 🧩 Data Modeling (Power Pivot)

After preparing the data in Power Query:
- The cleaned tables were loaded into *Power Pivot*.  
- Relationships were created between Fact and Dimension tables to build a *Star Schema Model*.  
- Fact table included metrics such as Sales, Profit, Quantity, and Discounts (for non-returned orders only).  
- Dimension tables included Date, Product, Customer, and Region.  
- A solid data model was built to ensure accurate aggregations and calculations for further visualization in Power BI.

---

## 📈 Measures Created in Power BI
| Measure | Description |
|----------|-------------|
| *Total Sales* | Total revenue from completed (non-returned) orders |
| *Total Profit* | Net profit excluding returns |
| *Profit Margin* | Profit / Sales (net) |
| *Total Orders* | Count of all completed orders |
| *Returned Orders* | Count of all returned orders |
| *Return Rate* | Returned Orders ÷ Total Orders |
| *Total Quantity* | Quantity of sold items excluding returns |
| *Total Shipping Cost* | Sum of shipping costs for completed orders |
| *Net Discount Value* | Discount applied to non-returned orders |
| *Net Profit Ratio* | Profit over total sales (excluding returns) |

---

## 🎨 Dashboard Design (Power BI)

The dashboard was designed using a clean *wireframe layout*, optimized background dimensions, and a consistent color theme.

### Visuals Included:
| Visualization | Purpose |
|----------------|----------|
| *Cards (5)* | Displayed KPIs: Total Sales, Total Profit, Profit Margin, Return Rate, and Total Orders |
| *Line Chart* | Sales trend by Year |
| *Clustered Column Chart* | Sales by Region |
| *Tree Map* | Sales by Category |
| *Stacked Bar Chart* | Sales by Customer |
| *Pie Chart* | Orders by Shipping Mode |
| *Stacked Bar Chart* | Sales by Product |
| *Gauge Chart* | Return Rate (Returned Orders vs Total Orders) |

Additional elements:
- *Slicers:* Year and Region  
- Customized chart titles, labels, and colors for clarity and consistency  

---

## 🔍 Key Insights
- 📉 *Sales slightly decreased in 2015, but then showed a **significant growth in 2016 and 2017*.  
- 💻 *Technology category* recorded the highest sales, while other categories had similar, close performance levels.  
- 🌍 *East region* achieved the highest sales, slightly ahead of the *West, followed by **Central* and *South*.  
- 🚚 *Standard Class* shipping mode was the most used — responsible for about *60% of total orders*.  
- 👤 *Sean Miller* was the top customer by total sales, followed by *Tamara Chand*, while the rest of the customers had relatively similar sales values.

---

## 🏁 Conclusion
This project demonstrates the end-to-end data analysis process using Microsoft BI tools — from raw data cleaning and modeling in Excel (Power Query & Power Pivot) to interactive visualization in Power BI.  
It highlights how structured data modeling and proper DAX measures can lead to clear, actionable business insights.

---

## 👤 Author
*Ahmed Ali*  
Business Intelligence Enthusiast | Excel | SQL | Power BI | Microsoft BI Tools