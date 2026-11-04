# Inventory Optimization & Replenishment Analytics

**Power BI | Inventory Management | Replenishment Planning | Cost Analysis**

[**View the project portfolio**](https://mohdaref12345-hash.github.io/-inventory-optimization-replenishment-analytics/project.html) · [**View the GitHub repository**](https://github.com/mohdaref12345-hash/-inventory-optimization-replenishment-analytics) · [**Download the Power BI report**](./mohammed%20Sultan.pbix)

## About the project

I built this project in Power BI to explore how inventory data can be used to understand stock levels, product demand, replenishment needs, and inventory-related costs.

The report is organized into four dashboard pages. Each page looks at inventory from a different angle, from the overall position and replenishment requirements to product-level demand and cost calculations.

## Dashboard pages

### 1. Inventory Overview

This page gives a general view of inventory performance. It includes demand by category, lead time, reorder points, safety stock, inventory value, and ABC classification.

![Inventory Overview dashboard](./Inventory%20Overview%20.png)

Some of the main figures shown on this page:

| Measure | Result |
|---|---:|
| Total Sales | 245K |
| Total Demand | 245K |
| Average Lead Time | 8.08 |
| Total Products | 40 |

**ABC classification**

| Class | Products | Share |
|---|---:|---:|
| A | 20 | 50% |
| B | 11 | 27.5% |
| C | 9 | 22.5% |
| **Total** | **40** | **100%** |

### 2. Replenishment Analysis

This page compares simulated current stock with reorder points and safety stock to show the replenishment quantity indicated by the analysis. It also breaks the recommended quantity down by product category.

![Replenishment Analysis dashboard](./Replenishment%20Analysis%20.png)

| Measure | Result |
|---|---:|
| Inventory Value | 0.15M |
| Current Stock (Simulated) | 1,736 units |
| Reorder Point | 2,125 units |
| Safety Stock | 310 units |
| Recommended Order Quantity | 389 units |

**Recommended order quantity by category**

| Category | Quantity |
|---|---:|
| Personal Care | 208 |
| Home | 80 |
| Electronics | 64 |
| Office | 37 |
| **Total** | **389** |

### 3. Inventory Optimization – Product Analysis

This page looks at inventory calculations at product level, with a focus on lead time demand and annual holding cost.

![Inventory Optimization Product Analysis dashboard](./Inventory%20Optimization%20%20Product%20Analysis%20.png)

| Measure | Result |
|---|---:|
| Average Daily Demand (summed across products) | 670.50 |
| Lead Time Days (summed across products) | 323 |
| Total Lead Time Demand | 5,328.06 |
| Current Stock (Simulated) | 6,970 units |
| Annual Holding Cost per Unit (summed across products) | 631.40 |
| Total Annual Holding Cost | 109,413.11 |

### 4. Inventory Optimization – Cost Analysis

This page brings together the main inventory cost measures, including Economic Order Quantity (EOQ), annual holding cost, annual ordering cost, and lead time demand.

![Inventory Optimization Cost Analysis dashboard](./Inventory%20Optimization%20Cost%20Analysis%20.png)

| Measure | Result |
|---|---:|
| Average EOQ | 220.03 units |
| Total Lead Time Demand | 5.33K units |
| Total Annual Holding Cost | 109.41K |
| Total Annual Ordering Cost | 57.88K |
| Annual Demand | 244,734 units |

**Average EOQ by category**

| Category | Average EOQ |
|---|---:|
| Electronics | 237 |
| Office | 226 |
| Personal Care | 210 |
| Home | 207 |

**Annual holding cost by category**

| Category | Annual Holding Cost |
|---|---:|
| Office | 38K |
| Electronics | 25K |
| Home | 24K |
| Personal Care | 24K |

**Annual ordering cost by category**

| Category | Annual Ordering Cost |
|---|---:|
| Office | 16.0K |
| Electronics | 15.0K |
| Personal Care | 14.9K |
| Home | 11.9K |

*Category figures are rounded as displayed in the Power BI charts.*

## Inventory calculations

The report uses standard inventory management calculations to help interpret stock requirements and costs.

**Reorder Point (ROP)**

```text
ROP = Average Daily Demand × Lead Time + Safety Stock
```

**Lead Time Demand**

```text
Lead Time Demand = Average Daily Demand × Lead Time (Days)
```

**Economic Order Quantity (EOQ)**

```text
EOQ = √((2 × Annual Demand × Ordering Cost per Order) / Annual Holding Cost per Unit)
```

**Annual Holding Cost**

```text
Annual Holding Cost = Current Stock × Annual Holding Cost per Unit
```

**Annual Ordering Cost**

```text
Annual Ordering Cost = (Annual Demand / EOQ) × Ordering Cost per Order
```

The ordering cost per order and annual holding cost per unit are assumed inputs used for this project. They should not be interpreted as verified costs from a real company.

## Tools and technologies

- **Microsoft Power BI** – building the report pages and visualizations.
- **DAX** – creating measures and KPI calculations.
- **Microsoft Excel** – storing and preparing inventory and demand data.
- **CSV** – providing product master information.

## Data files

The repository includes the source files used across the report:

| File | Used for |
|---|---|
| `Inventory_Stock (1).xlsx` | Inventory Overview and Replenishment Analysis |
| `Inventory Stock.xlsx` | Inventory Optimization – Product Analysis and Cost Analysis |
| `daily_demand.xlsx` | Supporting demand data |
| `product_master.csv` | Product information |

## Repository contents

```text
.
├── README.md
├── project.html
├── mohammed Sultan.pbix
├── Inventory_Stock (1).xlsx
├── Inventory Stock.xlsx
├── daily_demand.xlsx
├── product_master.csv
├── Inventory Overview .png
├── Replenishment Analysis .png
├── Inventory Optimization  Product Analysis .png
└── Inventory Optimization Cost Analysis .png
```

The portfolio page is `project.html`. It includes the dashboard screenshots directly in the page, so the portfolio does not depend on separate image links to display them.

## Open the report

1. Download [`mohammed Sultan.pbix`](./mohammed%20Sultan.pbix).
2. Open it with **Microsoft Power BI Desktop**.
3. Navigate through the four report pages to explore the dashboards.

## Project scope

This is an inventory analytics and reporting project. It presents stock, demand, replenishment, and cost information to support analysis and planning. It does not automatically place purchase orders or operate as a live inventory management system.

## Portfolio and source code

- [View the live portfolio](https://mohdaref12345-hash.github.io/-inventory-optimization-replenishment-analytics/project.html)
- [View the GitHub repository](https://github.com/mohdaref12345-hash/-inventory-optimization-replenishment-analytics)
- [View my GitHub profile](https://github.com/mohdaref12345-hash)

## Author

**Mohammed Aref Ali Sultan**

Industrial Engineering | Inventory Management | Operations Analytics | Power BI
