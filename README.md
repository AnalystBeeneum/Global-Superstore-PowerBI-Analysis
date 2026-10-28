# Global Superstore Sales & Profitability Analysis

## Executive Summary

I created an interactive Power BI dashboard to analyse Global Superstore's performance from 2011 to 2014. The aim was to understand where sales and profit came from, identify areas of weak performance, and recommend practical ways to improve profitability.

The business generated **12.64 million in sales** and approximately **1.47 million in profit**, with an overall **profit margin of 11.61%**. Technology was the strongest product category, Central led regional performance, and Consumer customers contributed more than half of total revenue.

The main finding was that strong sales did not always translate into strong profit. Furniture generated substantial revenue but had a lower margin than the other categories, while Tables recorded an overall loss. My recommendations focus on investigating these losses, supporting profitable products, and planning inventory around demand.

## Performance Overview

| KPI | Result |
| --- | ---: |
| Total Sales | 12.64M |
| Total Profit | 1.47M |
| Total Orders | Approximately 25.03K |
| Average Sales per Order Line | 246.49 |
| Profit Margin | 11.61% |

*Figures reflect the dashboard with all slicers cleared. M means million and K means thousand. Average Sales is calculated per order line, rather than per order.*

## Key Findings

- **Technology led overall performance**, generating approximately 4.74M in sales and 663.78K in profit, with a margin of 13.99%.
- **Furniture's profitability needs attention.** Its sales reached approximately 4.11M, but its margin was only 6.94%, compared with 13.69% for Office Supplies.
- **Tables recorded a loss of approximately 64.08K**, despite generating around 0.76M in sales. This makes the sub-category a priority for further investigation.
- **Consumer customers contributed 51.48% of sales**, followed by Corporate at 30.25% and Home Office at 18.27%.
- **Central generated the highest regional sales and profit.** The monthly sales chart also showed an upward overall trend across the period, alongside considerable monthly fluctuations.

## Risks and Opportunities

The main risks are continued losses from Tables, limited profit retention in Furniture, and inventory mismatches caused by fluctuating monthly sales.

The strongest opportunities are to grow profitable Technology products, improve Furniture margins, and test targeted offers for Corporate and Home Office customers. These two customer segments together account for 48.52% of sales.

## Recommendations

1. **Investigate losses in Tables.** Review performance by product, market and discount level, then examine purchasing and delivery costs before making pricing or delisting decisions.
2. **Support profitable Technology products.** Maintain availability of leading products and test promotions while monitoring their effect on profit margins.
3. **Improve Furniture margins.** Review low-margin products, discount practices and supplier terms to identify practical improvements.
4. **Plan stock around demand.** Use historical monthly sales by category and market to prepare for stronger periods and reduce excess stock during quieter months.
5. **Target customer segments carefully.** Maintain service quality for Consumer customers and test relevant campaigns for Corporate and Home Office customers, measuring both sales and profit.
6. **Allocate resources using profitability as well as sales.** Compare regional margins and product mix before increasing promotional spending or inventory.

## Dashboard Features

The dashboard includes five KPI indicators and eight analytical visuals covering regional performance, categories, sub-categories, profitable products, customer segments, countries, monthly sales and detailed product results.

Three interactive slicers allow users to filter the report by **Year, Market and Category**.

## Data Preparation and Measures

I used Power Query to inspect the data, check for missing values and duplicate rows, and correct data types. The duplicate check found no exact duplicate rows. I converted the date columns using the English (United Kingdom) locale and retained negative profit values because they represent business losses.

Missing postal codes were retained because the transactions still contained useful sales information. Geographic comparisons use the available location fields.

I used DAX to calculate the main measures:

- Total Sales: sum of Sales.
- Total Profit: sum of Profit.
- Total Orders: distinct count of Order ID.
- Average Sales: average Sales per order line.
- Profit Margin: Total Profit divided by Total Sales.

Sales already represents the amount for each order line, so it was not multiplied by Quantity.

## Tools and Data Source

- Microsoft Power BI
- Power Query
- DAX
- Global Superstore dataset, selected for the AnalystLab Africa Week 2 assignment

## Project Files

The project deliverables include the Power BI report (`.pbix`), a dashboard PDF export, the source dataset, and supporting reports. Open the `.pbix` file in Power BI Desktop to explore the interactive report; the PDF provides a static view.

## Interpretation Notes

The findings describe historical performance in the supplied dataset. The dashboard highlights areas for investigation but does not establish why losses occurred. Recommendations involving discounts, supplier costs or delivery costs require further checks before implementation. Displayed figures are rounded.

---

**Prepared by Analyst Beeneum**  
AnalystLab Africa — Week 2 Business Analytics Case Study
