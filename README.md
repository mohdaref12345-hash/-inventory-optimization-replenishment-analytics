# Inventory Optimization & Replenishment Analytics

### Power BI | Inventory Management | Demand Analysis | Replenishment Planning | Cost Analysis

## Project Overview

This project analyzes inventory levels, product demand, replenishment requirements, and inventory-related costs using Microsoft Power BI.

The objective is to support inventory management and planning decisions by reviewing stock availability, identifying products that may require replenishment, analyzing demand patterns, and exploring inventory optimization measures through interactive dashboards.

The report contains **four dashboard pages** organized into two main areas:

- **Inventory Analytics & Replenishment Planning**
- **Inventory Optimization & Cost Analysis**

## Project Preview

The following screenshots show the four report pages included in the Power BI project.

| Dashboard page | Screenshot |
|---|---|
| Inventory Overview | [View screenshot](Inventory%20Overview%20.png) |
| Replenishment Analysis | [View screenshot](Replenishment%20Analysis%20.png) |
| Inventory Optimization – Product Analysis | [View screenshot](Inventory%20Optimization%20%20Product%20Analysis%20.png) |
| Inventory Optimization – Cost Analysis | [View screenshot](Inventory%20Optimization%20Cost%20Analysis%20.png) |

### 1. Inventory Overview

![Inventory Overview](Inventory%20Overview%20.png)

### 2. Replenishment Analysis

![Replenishment Analysis](Replenishment%20Analysis%20.png)

### 3. Inventory Optimization – Product Analysis

![Inventory Optimization Product Analysis](Inventory%20Optimization%20%20Product%20Analysis%20.png)

### 4. Inventory Optimization – Cost Analysis

![Inventory Optimization Cost Analysis](Inventory%20Optimization%20Cost%20Analysis%20.png)

## Project Objectives

- Analyze product demand and inventory levels.
- Identify products that may require replenishment.
- Monitor inventory performance using key performance indicators (KPIs).
- Explore demand patterns across product categories and time periods.
- Review lead time demand and inventory-related costs.
- Calculate and analyze Economic Order Quantity (EOQ).
- Support inventory and replenishment planning through interactive visualizations.

## Tools & Technologies

- **Microsoft Power BI** — Dashboard development and data visualization
- **Microsoft Excel** — Inventory data management
- **DAX** — Measures and inventory KPI calculations
- **CSV** — Product master data source

## Dashboard Details & Results

### Page 1 — Inventory Overview

Provides an overview of inventory performance, product information, and demand patterns.

**Main KPIs**

| KPI | Dashboard result |
|---|---:|
| Total Sales | 245K |
| Total Demand | 245K |
| Average Lead Time | 8.08 |
| Total Products | 40 |

**Demand by category**

| Category | Demand |
|---|---:|
| Electronics | 70K |
| Office | 68K |
| Home | 59K |
| Personal Care | 48K |

**Average reorder point by category**

| Category | Average reorder point |
|---|---:|
| Office | 192.50 |
| Electronics | 150.70 |
| Home | 139.20 |
| Personal Care | 139.20 |

**Average safety stock by category**

| Category | Average safety stock |
|---|---:|
| Office | 24.90 |
| Electronics | 22.20 |
| Home | 20.00 |
| Personal Care | 19.90 |

**Inventory value by category**

| Category | Inventory value |
|---|---:|
| Office | 0.19M |
| Electronics | 0.12M |
| Home | 0.12M |
| Personal Care | 0.12M |

**ABC product classification**

| Class | Products | Share |
|---|---:|---:|
| A | 20 | 50.0% |
| B | 11 | 27.5% |
| C | 9 | 22.5% |
| **Total** | **40** | **100%** |

**Data source:** `Inventory_Stock (1).xlsx`, with the supporting demand and product data files.

### Page 2 — Replenishment Analysis

Focuses on stock availability and replenishment requirements.

**Main KPIs**

| KPI | Dashboard result |
|---|---:|
| Inventory Value | 0.15M |
| Recommended Order Quantity | 389 units |

**Inventory and replenishment totals**

| Measure | Total |
|---|---:|
| Current Stock (Simulated) | 1,736 units |
| Reorder Point | 2,125 units |
| Safety Stock | 310 units |
| Recommended Order Quantity | 389 units |

**Recommended order quantity by category**

| Category | Recommended quantity |
|---|---:|
| Personal Care | 208 |
| Home | 80 |
| Electronics | 64 |
| Office | 37 |
| **Total** | **389** |

The table identifies products with a **Reorder Needed** status and displays their current stock, reorder point, safety stock, and recommended order quantity.

**Data source:** `Inventory_Stock (1).xlsx`, with the supporting demand and product data files.

### Page 3 — Inventory Optimization: Product Analysis

Provides product-level analysis to support inventory optimization decisions.

**Lead time demand table totals**

| Measure | Total |
|---|---:|
| Average Daily Demand (summed across products) | 670.50 |
| Lead Time Days (summed across products) | 323 |
| Lead Time Demand | 5,328.06 |

**Annual holding cost table totals**

| Measure | Total |
|---|---:|
| Current Stock (Simulated) | 6,970 units |
| Annual Holding Cost per Unit (Assumed, summed across products) | 631.40 |
| Annual Holding Cost | 109,413.11 |

The page presents product-level lead time demand and annual holding cost to help compare inventory requirements and holding costs across products.

**Data source:** `Inventory Stock.xlsx`.

### Page 4 — Inventory Optimization: Cost Analysis

Focuses on the cost-related calculations used in the inventory optimization analysis.

**Main KPIs**

| KPI | Dashboard result |
|---|---:|
| Average EOQ | 220.03 units |
| Total Lead Time Demand | 5.33K units |
| Total Annual Holding Cost | 109.41K |
| Total Annual Ordering Cost | 57.88K |

**Additional totals visible in the product table**

| Measure | Total |
|---|---:|
| Annual Demand | 244,734 units |
| Ordering Cost per Order (assumed) | 50 |
| Annual Ordering Cost | 57,882.84 |

**Average EOQ by category**

| Category | Average EOQ (approximately) |
|---|---:|
| Electronics | 237 |
| Office | 226 |
| Personal Care | 210 |
| Home | 207 |

**Annual holding cost by category**  
*Values are rounded as displayed in the chart.*

| Category | Annual holding cost |
|---|---:|
| Office | 38K |
| Electronics | 25K |
| Home | 24K |
| Personal Care | 24K |

**Lead time demand by category**  
*Values are rounded as displayed in the chart.*

| Category | Lead time demand |
|---|---:|
| Office | 1.7K |
| Electronics | 1.3K |
| Home | 1.2K |
| Personal Care | 1.2K |

**Annual ordering cost by category**  
*Values are rounded as displayed in the chart.*

| Category | Annual ordering cost |
|---|---:|
| Office | 16.0K |
| Electronics | 15.0K |
| Personal Care | 14.9K |
| Home | 11.9K |

**Data source:** `Inventory Stock.xlsx`.

## Inventory Management & Optimization Calculations

### Safety Stock

Safety stock is additional inventory held to help reduce the risk of stockouts when demand or replenishment lead time varies.

### Reorder Point (ROP)

The reorder point is the inventory level that signals when a replenishment order should be placed.

```text
Reorder Point = Average Daily Demand × Lead Time + Safety Stock
```

### Lead Time Demand

```text
Lead Time Demand = Average Daily Demand × Lead Time (Days)
```

### Economic Order Quantity (EOQ)

EOQ estimates an order quantity that balances ordering costs and inventory holding costs.

```text
EOQ = √((2 × Annual Demand × Ordering Cost per Order) / Annual Holding Cost per Unit)
```

### Annual Holding Cost

```text
Annual Holding Cost = Current Stock × Annual Holding Cost per Unit
```

### Annual Ordering Cost

```text
Annual Ordering Cost = (Annual Demand / EOQ) × Ordering Cost per Order
```

**Assumptions:** The ordering cost per order and annual holding cost per unit used in the optimization analysis are assumed input values for analytical purposes. They should be interpreted as project assumptions, not verified actual company costs.

## Key Insights & Analytical Use

The dashboards allow users to:

- Review demand patterns across product categories and time periods.
- Compare average reorder points and safety stock by category.
- View product distribution by ABC classification.
- Identify inventory items that may need replenishment.
- Analyze product-level lead time demand.
- Compare annual holding and ordering costs.
- Review EOQ as a decision-support measure for replenishment planning.

The figures above are the values visible in the supplied dashboard screenshots. Chart labels may be rounded, and results can change when report filters or selections are applied.

## Project Files

```text
.
├── README.md
├── mohammed Sultan.pbix
├── index.html
├── Inventory_Stock (1).xlsx
├── Inventory Stock.xlsx
├── daily_demand.xlsx
├── product_master.csv
├── Inventory Overview .png
├── Replenishment Analysis .png
├── Inventory Optimization  Product Analysis .png
└── Inventory Optimization Cost Analysis .png
```

## How to Use

1. Download the Power BI file from this repository.
2. Open it using Microsoft Power BI Desktop.
3. Explore the four dashboard pages and their interactive visualizations.
4. Keep the supporting Excel and CSV files available if you need to refresh the data sources.

## Project Scope & Limitations

The recommended order quantity represents the replenishment quantity calculated and displayed in the current report.

The inventory optimization pages provide analytical calculations and cost comparisons based on the available dataset and assumed cost inputs. This project focuses on inventory analytics, replenishment reporting, and decision support. It should not be interpreted as a fully optimized procurement model or an automated inventory management system.

Results depend on the underlying dataset, report filters, DAX calculations, and assumptions used.

## Live Portfolio

[View the Live Project Website](https://mohdaref12345-hash.github.io/-inventory-optimization-replenishment-analytics/)

## Author

**Mohammed Aref Ali Sultan**

Industrial Engineering | Inventory Management | Operations Analytics | Power BI

[GitHub Profile](https://github.com/mohdaref12345-hash)
