# 📊 Electronics Sales & Revenue Analysis

An end-to-end **Data Analytics project** where I used **Python and Power BI** to analyze electronics sales data, identify sales trends, understand product performance, and generate meaningful business insights.

---

## 🖼️ Final Dashboard

<p align="center">
  <img src="dashboard/Electronics%20Sales%20Analytics%20Dashboard.png" 
       alt="Electronics Sales & Revenue Analysis Dashboard"
       width="100%">
</p>

---

## 📌 Project Overview

In this project, I analyzed electronics sales data to understand:

- Overall sales and revenue performance
- Order and quantity trends
- Product-wise sales performance
- Sales by city and state
- Sales by order hour
- Monthly sales trends
- Product combinations frequently purchased together
- Outliers and data distribution
- Key business KPIs

I followed a complete data analytics workflow from start to finish:

**Raw Data → Data Cleaning → Exploratory Data Analysis → Visualization → KPI Analysis → Power BI Dashboard → Business Insights**

---

## 🎯 Project Objectives

The main objectives I set out to achieve in this project were to:

- Understand and inspect the raw sales dataset
- Clean and prepare the data for analysis
- Identify and remove exact duplicate records
- Handle missing and inconsistent values
- Perform exploratory data analysis
- Analyze sales and product performance
- Identify sales patterns based on time and location
- Analyze frequently purchased product combinations
- Perform outlier analysis
- Create meaningful business KPIs
- Build an interactive Power BI dashboard
- Document the complete analysis process

---

## 🔄 Project Workflow

```text
Raw Dataset
     ↓
Data Inspection
     ↓
Data Cleaning
     ↓
Duplicate & Missing Value Analysis
     ↓
Data Transformation
     ↓
Exploratory Data Analysis
     ↓
Python Visualizations
     ↓
KPI Analysis
     ↓
Power BI Dashboard
     ↓
Business Insights
     ↓
Project Documentation
```

---

## 📂 Project Structure

```
Electronics-Sales-Revenue-Analysis/
│
├── Power bi/
│   └── Sales_Data_dashboard.pbix
│
├── dashboard/
│   ├── kpi/
│   │   ├── Avg_selling_price.svg
│   │   ├── MOM_Growth.svg
│   │   ├── Title.svg
│   │   ├── Total_Quantity.svg
│   │   ├── Total_orders.svg
│   │   ├── avg_order_value.svg
│   │   └── total_sales.svg
│   │
│   └── Electronics Sales Analytics Dashboard.png
│
├── data/
│   ├── cleaned/
│   │   ├── Product_Pairs.csv
│   │   └── Sales_Analysis_Data_cleaned.csv
│   │
│   └── raw/
│       └── Sales_Data.csv
│
├── documentation/
│   └── Electronic_Sales_and_Revenue_Analysis_Documentation.pdf
│
├── python/
│   └── Sales_Data_Analysis.ipynb
│
├── python_visualizations/
│   ├── Boxplot of Price Each.png
│   ├── Boxplot of Quantity Ordered.png
│   ├── Boxplot of Sales.png
│   ├── Correlation Matrix.png
│   ├── Monthly Sales Trend.png
│   ├── Price Each vs Sales.png
│   ├── Product Pairs.png
│   ├── Product-wise Sales.png
│   ├── Sales by City.png
│   ├── Sales by Order Hour.png
│   ├── Sales by Quantity Ordered.png
│   └── Sales by State.png
│
└── README.md
```

---

## 📊 Dataset

I used an electronics sales transaction dataset containing information about orders, products, quantities, prices, dates, locations, and sales.

### Main Fields

| Object | Description |
|---|---|
| `Order ID` | Identifier of the order |
| `Product` | Product purchased |
| `Quantity Ordered` | Quantity of products ordered |
| `Price Each` | Price of each product |
| `Order Date` | Date and time of the order |
| `Purchase Address` | Customer purchase address |
| `Month` | Month of the order |
| `Sales` | Total sales amount |
| `City` | City of the order |
| `State` | State of the order |
| `Hour` | Hour of the order |

---

## 🧹 Data Cleaning

I performed all data cleaning using Python and Pandas.

My cleaning process included:

- Dataset structure inspection
- Data type checking
- Missing value analysis
- Invalid record identification
- Exact duplicate identification
- Duplicate record removal
- Date conversion
- Data transformation
- Extraction of city and state information
- Extraction of order hour
- Creation of analytical columns
- Outlier analysis
- Final data quality checks

### Duplicate Analysis

I made a clear distinction between:

- Exact duplicate rows, and
- Repeated Order IDs

A repeated Order ID does not automatically represent a duplicate because a single order can contain multiple products. So I retained legitimate multi-product orders while removing exact duplicate rows.

---

## 🔎 Exploratory Data Analysis

I performed exploratory data analysis using:

- Pandas
- NumPy
- Matplotlib
- Seaborn

My analysis includes:

**📈 Sales Analysis**
- Monthly sales trends
- Sales distribution
- Sales by quantity
- Sales by product
- Sales by location

**🛍️ Product Analysis**
- Product-wise sales
- Product quantity analysis
- Product pair analysis
- Top-performing products

**🌎 Geographic Analysis**
- Sales by city
- Sales by state

**⏰ Time Analysis**
- Sales by order hour
- Monthly sales trends

**📦 Distribution & Outlier Analysis**
- Sales boxplot
- Quantity ordered boxplot
- Price each boxplot
- Correlation matrix

---

## 📊 Python Visualizations

I generated the following visualizations as part of the analysis:

| Object | Purpose |
|---|---|
| `Boxplot of Price Each` | Identify price distribution and potential outliers |
| `Boxplot of Quantity Ordered` | Analyze quantity distribution and outliers |
| `Boxplot of Sales` | Analyze sales distribution and outliers |
| `Correlation Matrix` | Understand relationships between numerical variables |
| `Monthly Sales Trend` | Analyze sales performance over time |
| `Price Each vs Sales` | Analyze the relationship between price and sales |
| `Product Pairs` | Identify frequently purchased product combinations |
| `Product-wise Sales` | Compare sales across products |
| `Sales by City` | Analyze geographic sales performance |
| `Sales by Order Hour` | Identify high-performing sales hours |
| `Sales by Quantity Ordered` | Analyze sales based on quantity ordered |
| `Sales by State` | Compare sales across states |

---

## 🔗 Product Pair Analysis

I also analyzed which products were purchased together within the same order.

The purpose of this analysis was to identify potential:

- Cross-selling opportunities
- Product bundles
- Promotional combinations
- Customer purchasing patterns

I exported a separate cleaned dataset for this: `data/cleaned/Product_Pairs.csv`

---

## 📌 Power BI Dashboard

I used the cleaned sales data to build an interactive Power BI dashboard.

### 📊 Dashboard KPIs

The dashboard I built contains the following key performance indicators:

| Object | Type | Purpose |
|---|---|---|
| `Total Sales` | KPI Card | Overall revenue for the selected filter context |
| `Total Quantity` | KPI Card | Total units sold for the selected filter context |
| `Total Orders` | KPI Card | Total number of orders placed |
| `Average Order Value` | KPI Card | Revenue per order — Total Sales ÷ Total Orders |
| `Average Selling Price` | KPI Card | Average unit price across all line items |
| `MoM Sales %` | KPI Card | Month-over-month sales growth indicator |

The individual KPI visual assets are available inside `dashboard/kpi/`, and a full dashboard preview image is available at `dashboard/Electronics Sales Analytics Dashboard.png`.

### 📊 Charts

| Object | Type | Purpose |
|---|---|---|
| `Top 5 Sales by City` | Horizontal Bar | Ranks the top 5 cities by total sales revenue |
| `Sales by Order Hour` | Column Chart | Shows revenue distribution across each hour of the day to reveal peak ordering times |
| `Product Pair Count` | Table / Bar Chart | Lists the top product pairs frequently bought together, along with their co-purchase counts |
| `Top 5 Products by Sales` | Horizontal Bar | Ranks the top 5 products by total revenue generated |
| `Total Quantity by Product` | Horizontal Bar | Ranks products by total units sold |
| `Total Sales by State` | Treemap | Shows revenue share by state, with each state sized proportionally |
| `Sales Over Day` | Line Chart | Tracks the daily sales trend across the selected time period |
| `Total Sales by Price Each` | Scatter Plot | Shows the relationship between unit price and total sales generated |

### 🎚️ Slicers

| Object | Type | Purpose |
|---|---|---|
| `Year` | Slicer | Filters the dashboard by year (e.g. 2019) |
| `Month` | Slicer | Filters the dashboard by month |
| `City` | Slicer | Filters the dashboard by city |
| `State` | Slicer | Filters the dashboard by state |
| `Product` | Slicer | Filters the dashboard by individual product |

### 📈 Power BI Analysis

The dashboard I built provides analysis of:

- Sales performance
- Order performance
- Quantity performance
- Product performance
- Geographic performance
- Time-based sales trends
- Monthly growth
- Product combinations

The Power BI report is available at: `Power bi/Sales_Data_dashboard.pbix`

---

## 🛠️ Tools & Technologies

| Object | Usage |
|---|---|
| `Python` | Data analysis and cleaning |
| `Pandas` | Data manipulation |
| `NumPy` | Numerical analysis |
| `Matplotlib` | Visualization |
| `Seaborn` | Visualization |
| `Jupyter Notebook` | Python analysis |
| `Power BI` | Dashboard and business intelligence |
| `Power Query` | Data transformation |
| `DAX` | KPI calculations |
| `GitHub` | Project repository and version control |

---

## 📁 Data Files

**Raw Data** — `data/raw/Sales_Data.csv`
Contains the original dataset I used for the project.

**Cleaned Data** — `data/cleaned/Sales_Analysis_Data_cleaned.csv`
Contains the processed dataset I used for further analysis and dashboard development.

**Product Pair Data** — `data/cleaned/Product_Pairs.csv`
Contains my product combination analysis.

---

## 🐍 Python Analysis

My complete Python analysis is available in: `python/Sales_Data_Analysis.ipynb`

The notebook covers:

- Importing libraries
- Loading the dataset
- Data inspection
- Data cleaning
- Duplicate analysis
- Missing value analysis
- Data transformation
- Exploratory data analysis
- Visualization
- Product pair analysis
- Outlier analysis
- Final data validation

---

## 📄 Documentation

I wrote up detailed project documentation, available here: `documentation/Electronic_Sales_and_Revenue_Analysis_Documentation.pdf`

The documentation walks through the full analysis process, visualizations, dashboard, findings, and conclusions.

---

## 💡 Business Insights

Through this analysis, I was able to answer important business questions such as:

- Which products generate the highest sales?
- Which products have the highest quantity sold?
- Which cities and states contribute the most sales?
- During which hours are sales highest?
- How does sales performance change over time?
- Which products are frequently purchased together?
- Are there unusual sales, price, or quantity values?
- What are the key sales performance indicators?

These insights can support better decisions related to:

- Product strategy
- Inventory planning
- Marketing campaigns
- Product bundling
- Cross-selling
- Sales strategy
- Geographic targeting

---

## 🚀 How to Run the Project

1. **Clone the repository**
   ```
   git clone https://github.com/Shiva-6816/Electronics-Sales-Revenue-Analysis.git
   ```

2. **Open the Python notebook**
   Navigate to `python/Sales_Data_Analysis.ipynb` and open it using Jupyter Notebook, JupyterLab, or VS Code.

3. **Run the Python analysis**
   Run the notebook cells to reproduce the data cleaning, data analysis, statistical analysis, visualizations, and product pair analysis.

4. **Open the Power BI dashboard**
   Navigate to `Power bi/Sales_Data_dashboard.pbix` and open the file using Microsoft Power BI Desktop.

---

## 🔮 Future Improvements

Some improvements I'd like to explore next:

- Adding profitability analysis
- Adding customer-level analysis
- Adding more advanced Power BI drill-through pages
- Automating data refresh
- Creating additional interactive dashboard pages
- Expanding product bundle analysis
- Deploying the dashboard as a web application

---

## 👨‍💻 Author

**Shiva Prasad Aroori**
Data Analyst | Data Science Enthusiast

**Skills demonstrated in this project:**
Python, Pandas, NumPy, Matplotlib, Seaborn, Power BI, Power Query, DAX, Exploratory Data Analysis, Data Cleaning, Data Visualization, Business Intelligence

### 🔗 Connect With Me

- GitHub: [Shiva-6816](https://github.com/Shiva-6816)
- LinkedIn: Shiva Prasad Aroori
- Portfolio: My Portfolio

---

## ⭐ Support

If you found this project useful or interesting, consider giving the repository a ⭐ on GitHub.
