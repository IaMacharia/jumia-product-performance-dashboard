# jumia-product-performance-dashboard
# Jumia Product Performance Dashboard

## Project Overview

This project analyzes product performance data from Jumia and presents insights through an interactive Excel dashboard. The objective is to transform raw product data into meaningful business insights by performing data cleaning, analysis, and visualization using Microsoft Excel.

The dashboard enables users to evaluate product pricing, discounts, customer engagement, and ratings to identify top-performing products and areas for improvement.

---

## Project Objectives

The project aims to:

- Analyze product pricing and discount strategies.
- Evaluate customer engagement through reviews and ratings.
- Identify top-performing and underperforming products.
- Explore relationships between discounts, ratings, and reviews.
- Create an interactive dashboard for decision-making.

---

## Dataset Description

The dataset contains product information collected from Jumia, including:

| Column | Description |
|----------|------------|
| Product Name | Name of the product |
| Current Price | Current selling price |
| Old Price | Original price before discount |
| Absolute Discount | Difference between old and current price |
| Discount (%) | Percentage discount offered |
| Reviews | Number of customer reviews |
| Ratings | Product rating score |
| Price Category | Low, Medium, or High price classification |
| Discount Category | Low, Medium, or High discount classification |
| Rating Category | Poor, Average, or Excellent classification |

---

## Tools Used

- **Microsoft Excel**
  - Data Cleaning
  - Pivot Tables
  - Pivot Charts
  - Scatter Plots
  - Dashboard Design
  - Statistical Analysis
  - Formulas and Functions

- **GitHub**
  - Version control
  - Project documentation

---

## Data Cleaning Process

Several data quality issues were addressed before analysis:

### 1. Missing Values
- Checked for blank cells.
- Removed or handled incomplete records where necessary.

### 2. Data Type Validation
- Ensured prices and discounts were stored as numeric values.
- Confirmed ratings and review counts used appropriate formats.

### 3. Derived Columns Created

Absolute Discount

```excel
=Old Price - Current Price
```

Discount Percentage

```excel
=(Absolute Discount/Old Price)*100
```

Price Category

Products were classified using Quartiles:

```excel
=IF(Current price<=Q1,"Low Price",
IF(CurrentPrice<=Q3,"Medium Price",
"High Pricee))
```

Discount Category

``*excel
=IF(Discount%<=Q1,"Low Discount",
IF(Discount*<=Q3,"Medium Discount",
"High Disc*unt"))
```

Rating Category

*``excel*=IF (Rating<3,"Poor",
IF(Rating<=4.5,"Average",
"Excellent"))
```

---

Analysis Performed

Descriptive Statistics

Thefollowing metrics were calculated:
- Average Price
- Average Discount
- Average Rating
- Total Reviews
* Maximum and Minimum Prices

orrelation Analysis

Pearson Correlation was used to determine relationships between:

```excel
=CORREL(Discount Range, Reviews Range)
```

```excel
=CORREL(Rating Range, Reviews Range)
```

*``excel
=CORREL(Discount Range, Rating Range)
```
*Scatter plots were used to visualiZe these relationships.

Top Products Analysis

Ranked tables were created to identify:

- Top 5 highest-rated products
- Top 5 most-reviewed products
- Products with large discounts
- High-discount but low rated products

---

Dashboard features

The dashboard includes:

KPI Cards

- Total Products
- Average Rating
- Average Discount (%)
- Total Reviews

Visualizations

Product Distribution by Price Category
Shows the number of products in each pricing segment.

Product Distribution by Discount Category
Displays discount patterns across products.

Rating Distribution
Highlights product quality trends.

op Rated Products
Ranks products based on customer ratings.

Most Reviewed Products
Identifies products with the highest customer engagement.

Discount vs Revie*s Scatter Plot
Visualizes the rela*ionship between discounts and reviews.

Rating vs Reviews Scatte* Plot
Shows how ratings influence customer engagement.

Interactive Features

- Slicers for easy fil*ering
- Dynamic Pivot Tables
- Dynamic Pivot Charts

---

Key Findings

Pricing Insights
- Most products fall within the medium-price category.
- High-priced products represent a smaller share of the catalogue.

Discount Insights
- Products with larger discounts generally attracts more customer attention.
- Some hi*hly discounted products still receive poor ratings.

ustomer Engagement
- Products with higher review counts are generally better known among customers.
- Customer reviews provide a useful indicator of product popularity.

Product Performance
- Several products achieved*excellent ratings while maintainin* competitive pricing.
- Certain pr*ducts require quality improvements*despite aggressive discounting.

*--

## Recommendations

1.*Prioritize products with high ratings and strong customer engagement.*2. Review products receiving poor ratings despite large discounts.
3.*Use discounts strategically rather*than relying solely on price reductions.
4. Focus marketing efforts on products with strong customer feedback.
5. Continuously monitor cust*mer reviews to identify improvement opportunities.

---

## Limitations

- Analysis is limited to the av*ilable dataset.
- Customer demogra*hics were not included.
- Product *ategories were not analyzed separa*ely.
- Findings may change as prod*ct prices and reviews are updated.*
---

## File Structure

```text
jumia-product-performance-dashboard/*│
├── README.md
│
├── data/
│   └─* Excel_jumia_data.csv
│
├── dashboard*
│   └── Jumia Finals.xlsx
│
└── images/
    ├── DashBoard.png
    ├*─ Raw_Data.png
   *└── Cleaned_Data.png
```

*--

## How to Open and Use the Wor*book

1. Download the Excel workbo*k.
2. Open the file using Microsof* Excel 2016 or later.
3. Navigate *o the Dashboard sheet.
4. Use slicers and filters to explore the data*
5. Review charts and KPIs for insights.
6. Refer to the Analysis sheet for calculations and supporting statistics.

---






✅ Completed

This project demonstrates practical data cleaning, Excel analytics, dashboard development, and business intelligence reporting skills using product performance data.
