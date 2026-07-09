# U.S. Airbnb Market Analysis

An end-to-end SQL-driven analysis of the U.S. short-term rental market, uncovering pricing trends, host distribution, and neighborhood-level demand patterns across major American cities. Built using MS SQL Server for querying and Jupyter Notebook for data preparation.

---

## Project Overview

Short-term rental platforms like Airbnb generate massive amounts of pricing, availability, and host data — but turning that data into decisions requires structured analysis. This project explores the U.S. Airbnb Open Data dataset to answer practical questions: which cities dominate the market, which room types perform best, what drives premium pricing, and where untapped opportunity exists for hosts and travelers.

The goal is to translate raw listing-level data into clear, actionable market insights using SQL-based analysis.

---

## Dataset

- **Source:** [U.S. Airbnb Open Data](https://www.kaggle.com/datasets/kritikseth/us-airbnb-open-data) (Kaggle)
- **Scope:** Listing-level data covering multiple U.S. cities, including price, room type, availability, host counts, neighborhood, and review metrics
- **Preprocessing:** Cleaned and prepared in Jupyter Notebook prior to querying

---

## Project Workflow

1. **Data Collection** — Sourced the U.S. Airbnb Open Data dataset from Kaggle
2. **Data Cleaning** — Preprocessed and structured the raw data in Jupyter Notebook
3. **Database Querying** — Loaded data into MS SQL Server for structured analysis
4. **Exploratory Analysis** — Queried host distribution, pricing, availability, and reviews across cities, room types, and neighborhoods
5. **Business Insights** — Interpreted patterns to explain market behavior
6. **Recommendations** — Converted findings into actionable strategies for hosts and the platform

---

## Exploratory Data Analysis

**Referenced Tables**
- Cities by Total Host Count
- Average Price by Room Type
- Room Availability vs. Host Count
- Top Neighborhoods by Review & Price
- Lowest-Priced High-Value Listings
- Zero-Availability Listings
- Average City-Level Pricing
- Average Reviews by Room Type

### Cities with the Most Hosts

| City | Total Hosts |
|---|---|
| New York City | 45,742 |
| Los Angeles | 31,530 |
| Hawaii | 22,434 |
| San Diego | 12,401 |
| Broward County | 10,855 |
| Austin | 10,433 |
| Clark County | 8,408 |

### Average Price by Room Type

| Room Type | Average Price ($) |
|---|---|
| Hotel room | 281 |
| Entire home/apt | 270 |
| Private room | 106 |
| Shared room | 73 |

### Availability vs. Host Count by Room Type

| Room Type | Avg. Availability (days) | Total Hosts |
|---|---|---|
| Private room | 141 | 65,870 |
| Entire home/apt | 165 | 154,157 |
| Shared room | 186 | 4,029 |
| Hotel room | 187 | 1,941 |

### Top Neighborhoods by Review Score & Price

| Neighborhood | Avg. Reviews | Avg. Price ($) |
|---|---|---|
| Presidio | 249 | 120 |
| Huguenot | 198 | 180 |
| Glenfair | 173 | 87 |
| Sullivan's Gulch | 166 | 101 |
| Boise | 160 | 117 |
| Russell | 155 | 85 |
| Bell | 149 | 57 |

---

## Key Insights

- **Market concentration:** New York City, Los Angeles, and Hawaii together account for the largest share of active hosts, confirming that Airbnb demand is heavily concentrated in high-tourism, high-density metro areas.
- **Entire homes drive engagement:** Entire homes/apartments have both the highest host count (154,157) and the highest average reviews (36), making them the platform's most trusted and in-demand category — ideal for families and groups.
- **Shared rooms underperform:** Shared rooms have the lowest average price ($73), lowest reviews (16), and the highest average availability (186 days) — indicating persistently low demand and limited host interest in this category.
- **Price doesn't always track availability:** Hotel rooms carry the highest average price ($281) despite ranking near the bottom in both host count and reviews, suggesting a small, premium niche rather than broad market demand.
- **Reputation supports premium pricing:** Neighborhoods like Presidio and Huguenot combine high review volume with above-average pricing, showing that strong guest satisfaction sustains higher price points rather than undercutting them.

---

## Business Recommendations

- **Prioritize entire-home listings** in host acquisition efforts, since this category shows the strongest combination of demand, host volume, and guest satisfaction.
- **Reassess shared-room inventory** in low-performing markets — reallocate or convert underused shared-room listings to private rooms, which show stronger booking activity relative to availability.
- **Investigate zero-availability listings** for data integrity issues (misreported availability) or inactive hosts, as these listings distort true market supply figures.
- **Use high-review neighborhoods as pricing benchmarks** — areas like Presidio and Huguenot demonstrate that guests will pay a premium where satisfaction is consistently high, offering a model for pricing strategy in comparable neighborhoods.
- **Target marketing spend toward top-performing metros** (NYC, LA, Hawaii) while testing incentive programs in mid-tier markets (e.g., Austin, San Diego) to diversify host growth beyond saturated cities.

---

## Tools & Technologies

- MS SQL Server (data querying & analysis)
- Jupyter Notebook (data cleaning & preprocessing)
- Kaggle (dataset source)

---

## Project Structure

```text
airbnb-analysis/
│
├── data/
├── notebooks/
├── reports/
├── README.md
└── requirements.txt
```
