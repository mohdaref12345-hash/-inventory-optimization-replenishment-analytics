# Inventory Optimization & Replenishment Analytics

**Power BI | Inventory Management | Demand Analysis | Replenishment Planning**

## Project Overview

This project was developed using Microsoft Power BI to analyze inventory performance, product demand, replenishment requirements, and inventory-related costs.

The main idea behind the project is to bring inventory data together in interactive dashboards and make it easier to understand stock levels, identify products that need replenishment, and analyze the costs associated with holding and ordering inventory.

The project includes four dashboard pages, covering inventory overview, replenishment analysis, product-level inventory analysis, and inventory cost analysis.

## Project Preview

The project contains four Power BI dashboards:

1. Inventory Overview
2. Replenishment Analysis
3. Inventory Optimization – Product Analysis
4. Inventory Optimization – Cost Analysis

## Dashboard Screenshots

### 1. Inventory Overview

This dashboard provides an overview of inventory performance, including product information, demand by category, daily demand trends, reorder points, safety stock, inventory value, and ABC classification.

![Inventory Overview](Inventory%20Overview%20.png)

**Main results:**

| KPI | Result |
|---|---:|
| Total Sales | 245K |
| Total Demand | 245K |
| Average Lead Time | 8.08 |
| Total Products | 40 |

**Demand by category:**

| Category | Demand |
|---|---:|
| Electronics | 70K |
| Office | 68K |
| Home | 59K |
| Personal Care | 48K |

**ABC Classification:**

| Class | Products | Percentage |
|---|---:|---:|
| A | 20 | 50% |
| B | 11 | 27.5% |
| C | 9 | 22.5% |
| **Total** | **40** | **100%** |

### 2. Replenishment Analysis

This dashboard focuses on inventory availability and replenishment requirements. It helps identify products that need replenishment by comparing current stock with reorder points and safety stock.

![Replenishment Analysis](Replenishment%20Analysis%20.png)

**Main results:**

| KPI | Result |
|---|---:|
| Inventory Value | 0.15M |
| Recommended Order Quantity | 389 units |
| Current Stock (Simulated) | 1,736 units |
| Reorder Point | 2,125 units |
| Safety Stock | 310 units |

**Recommended order quantity by category:**

| Category | Quantity |
|---|---:|
| Personal Care | 208 |
| Home | 80 |
| Electronics | 64 |
| Office | 37 |
| **Total** | **389** |

### 3. Inventory Optimization – Product Analysis

This dashboard provides a product-level view of lead time demand and annual holding costs. It helps compare inventory requirements and holding costs across different products.

![Inventory Optimization Product Analysis](Inventory%20Optimization%20%20Product%20Analysis%20.png)

**Lead Time Demand results:**

| Measure | Result |
|---|---:|
| Average Daily Demand (summed across products) | 670.50 |
| Lead Time Days (summed across products) | 323 |
| Total Lead Time Demand | 5,328.06 |

**Annual Holding Cost results:**

| Measure | Result |
|---|---:|
| Current Stock (Simulated) | 6,970 units |
| Annual Holding Cost per Unit (summed across products) | 631.40 |
| Total Annual Holding Cost | 109,413.11 |

### 4. Inventory Optimization – Cost Analysis

This dashboard focuses on the cost calculations used in the inventory optimization analysis. It includes Economic Order Quantity (EOQ), annual holding cost, annual ordering cost, and lead time demand.

![Inventory Optimization Cost Analysis](Inventory%20Optimization%20Cost%20Analysis%20.png)

**Main results:**

| KPI | Result |
|---|---:|
| Average EOQ | 220.03 units |
| Total Lead Time Demand | 5.33K units |
| Total Annual Holding Cost | 109.41K |
| Total Annual Ordering Cost | 57.88K |
| Annual Demand | 244,734 units |

**Average EOQ by category:**

| Category | Average EOQ |
|---|---:|
| Electronics | 237 |
| Office | 226 |
| Personal Care | 210 |
| Home | 207 |

**Annual Holding Cost by category:**

| Category | Annual Holding Cost |
|---|---:|
| Office | 38K |
| Electronics | 25K |
| Home | 24K |
| Personal Care | 24K |

**Annual Ordering Cost by category:**

| Category | Annual Ordering Cost |
|---|---:|
| Office | 16.0K |
| Electronics | 15.0K |
| Personal Care | 14.9K |
| Home | 11.9K |

*Category values are rounded as displayed in the Power BI charts.*

## Inventory Management Calculations

The project uses several inventory management calculations to analyze stock requirements and replenishment decisions.

**Safety Stock**

Additional inventory kept to reduce the risk of stockouts when demand or lead time changes.

**Reorder Point (ROP)**

The inventory level at which a replenishment order should be placed.

```text
ROP = Average Daily Demand × Lead Time + Safety Stock
```

**Lead Time Demand**

```text
Lead Time Demand = Average Daily Demand × Lead Time (Days)
```

**Economic Order Quantity (EOQ)**

EOQ estimates an order quantity by balancing ordering costs and holding costs.

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

The ordering cost per order and annual holding cost per unit used in the optimization analysis are assumed values for this project. They are not actual verified company costs.

## Tools & Technologies

- **Microsoft Power BI:** Dashboard development and data visualization.
- **Microsoft Excel:** Inventory data management.
- **DAX:** Measures and KPI calculations.
- **CSV:** Product master data.

## Data Sources

The project uses separate inventory files for the different dashboard sections:

| File | Used for |
|---|---|
| `Inventory_Stock (1).xlsx` | Inventory Overview and Replenishment Analysis |
| `Inventory Stock.xlsx` | Inventory Optimization – Product Analysis and Cost Analysis |
| `daily_demand.xlsx` | Supporting demand data |
| `product_master.csv` | Product information |

## Project Files

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

## How to Use

1. Download `mohammed Sultan.pbix` from the repository.
2. Open the file using Microsoft Power BI Desktop.
3. Explore the four dashboard pages.
4. Use the supporting Excel and CSV files if you need to refresh the data.

## Project Scope

This project focuses on inventory analytics, replenishment reporting, and inventory cost analysis.

The dashboards provide information to support inventory planning and decision-making. The EOQ and cost calculations are based on the available dataset and assumed cost inputs. The project is an analytical reporting tool, not an automated inventory management system or a fully optimized procurement model.

## Live Portfolio

[View the Project Portfolio](https://mohdaref12345-hash.github.io/-inventory-optimization-replenishment-analytics/project.html)

## Author

**Mohammed Aref Ali Sultan**

Industrial Engineering | Inventory Management | Operations Analytics | Power BI

[GitHub Profile](https://github.com/mohdaref12345-hash)
