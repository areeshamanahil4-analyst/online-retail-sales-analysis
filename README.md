# Online Retail Sales Analysis

One year of sales (1 Dec 2010 to 9 Dec 2011) from a UK online gift shop: 19,773 orders from 4,334 customers in 38 countries.
I cleaned the data and answered five questions with **Python (pandas)**, then built a **Power BI** dashboard.

# What I found

- Net revenue was **£9.77M** after £476K of cancellations.
- Sales are highest from **September to November**.
- The UK gives about **85%** of sales.
- About a quarter of customers bring about two thirds of the sales to customers with an ID (Champions: 26% of customers, 68% of that revenue).
- **4.6%** of sales were cancelled. About half of that came from two huge orders cancelled within minutes (about 2.3% without them).
- In 4 of the 10 biggest countries outside the UK, one customer gives more than half of the sales.

# What I recommend

1. Win back the 657 customers who stopped buying (they had spent about £774K).
2. Buy stock and plan staff before September.
3. Look after the few customers that carry whole countries.
4. Check very big orders before accepting them.


# Dashboard preview

![Intro](images/01_intro.png)
![Business Overview](images/02_business_overview.png)
![Products and Countries](images/03_products_countries.png)
![Customers (RFM)](images/04_customers_rfm.png)
![Findings and Actions](images/05_findings_actions.png)

## What is in this repository

 File | What it is |

Retail_Analysis_Final.ipynb | Cleaning and analysis in Python |
rfm_segments.csv`, `products.csv | Output tables used by the dashboard |
Retail_sales_Analysis_Project.pbix | The Power BI dashboard |
images/` | Dashboard screenshots |

## How to run it

1. Download `Online Retail.xlsx` from the link below and put it in the same folder as the notebook.
2. Open the notebook and run all cells.
3. The notebook creates `retail_clean.csv`, `rfm_segments.csv` and `products.csv`.

## About the data

- Source: [Online Retail dataset, UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/352/online+retail), licensed CC BY 4.0.
- Data by Daqing Chen, Sai Liang Sain and Kun Guo (2012). The data owner says many customers of the company are wholesalers.
- I removed 5,268 duplicate rows. Cancellations, postage and fees are labelled and kept apart from sales.

## Limits

- Only one year of data, so "Lost" customers may just be seasonal.
- About 15% of sales have no customer ID, so the customer pages leave them out.
- December 2010 and December 2011 are partial months.

**Author:** Areesha · Tools: Python (pandas), Power BI

