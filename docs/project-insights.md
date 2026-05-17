# Project Insights  
## Supply Chain Planning Control Tower  
### Demand Review, Stock Rebalancing & Revenue Phasing Dashboard

---

## 1. Project Purpose

This Power BI dashboard was built as a supply chain planning portfolio project.

The main purpose of this report is not only to visualize sales data, but to support supply chain planning decisions by connecting:

- Sales performance
- Demand signals
- Product and category priorities
- Inventory health
- Stock cover risk
- Net demand logic
- Stock surplus and overstock risk
- Stock rebalancing actions
- Revenue phasing performance

In a real supply chain planning context, this dashboard can help planners and managers answer one important question:

> Should the business replenish more stock, hold unnecessary orders, review overstock SKUs, or monitor revenue phasing more closely?

---

## 2. Project Context

Supply chain teams often need to make decisions based on multiple sources of data such as sales, demand, inventory, distributor stock, warehouse stock, and invoicing performance.

Without a structured dashboard, it can be difficult to quickly understand:

- Which SKUs are important
- Which products are selling well
- Which categories drive revenue
- Whether stock is enough or excessive
- Whether replenishment is needed
- Whether revenue is being phased properly across the month

This dashboard was designed to combine these different views into one planning control tower.

---

## 3. Target Users

This report is designed for:

- Supply Chain Interns
- Demand Planning teams
- Inventory Planning teams
- Sales Operations teams
- Supply Chain Managers
- Business analysts supporting supply chain operations

The dashboard can be used as a decision-support tool to improve visibility across sales, inventory, stock cover, and monthly revenue phasing.

---

## 4. Main Business Questions

This dashboard answers the following business questions:

1. Which categories, products, regions, and distributors are driving sales?
2. Which SKUs should be prioritized in demand review?
3. Are there any understock or overstock risks?
4. Is replenishment currently required?
5. Which products have high stock surplus?
6. Which distributors are holding high inventory?
7. Is revenue being phased properly across the month?
8. Are first-half-month sales meeting the 40% phasing target?
9. What planning actions should be taken based on current demand and stock condition?

---

## 5. Dashboard Storyline

The report follows this supply chain planning storyline:

```text
Revenue Signal
→ Demand & SKU Prioritization
→ Inventory Health Check
→ Stock Rebalancing Action
→ Revenue Phasing Follow-up
```

This means the dashboard starts from the overall business performance, then moves into product/category analysis, inventory condition, planning actions, and finally revenue phasing performance.

The logic is:

1. First, understand business performance.
2. Then, identify which products and categories matter most.
3. Next, check whether stock is healthy or risky.
4. Then, convert inventory insights into planning actions.
5. Finally, monitor whether revenue is phased properly across the month.

---

## 6. Dashboard Structure

The dashboard includes 5 pages:

| Page | Page Name | Main Purpose |
|---|---|---|
| Page 1 | Executive Control Tower | Overall business and planning status |
| Page 2 | Demand & Revenue Drivers | Identify key revenue and demand contributors |
| Page 3 | Inventory Health & Stock Cover | Monitor understock and overstock risk |
| Page 4 | Stock Rebalancing & Allocation Readiness | Convert stock insights into planning actions |
| Page 5 | Revenue Phasing & Invoicing Follow-up | Track first-half-month sales performance |

---

# 7. Page-by-Page Business Explanation

---

## Page 1 — Executive Control Tower

![Executive Control Tower](../images/page-1-executive-control-tower.png)

### Purpose

This page provides a high-level overview of business performance and planning status.

It is designed for users who want to quickly understand:

- How the business is performing
- Whether sales and profit are healthy
- Whether there is any immediate replenishment need
- Whether first-half-month sales performance is on track

### Main Metrics

| Metric | Meaning |
|---|---|
| Net Sales | Total revenue after discount |
| Gross Profit | Profit after considering cost |
| Gross Margin % | Profitability ratio |
| Net Demand PCS | Additional stock requirement based on planning logic |
| Order Proposal PCS | Suggested replenishment quantity |
| Sales First Half % | Percentage of sales achieved in the first half of the month |

### What Users Can Know from This Page

Users can quickly know:

- Total business performance
- Gross profit and margin level
- Whether there is any net demand
- Whether order proposal is required
- Which regions and distributors are driving sales
- Whether revenue phasing is healthy

### Key Insight

Total Net Sales reached **78.91bn**, with **14.13bn Gross Profit** and **17.91% Gross Margin**.

Net Demand and Order Proposal are currently **0**, which indicates that there is no immediate replenishment requirement under the current stock cover logic.

First-half-month sales reached **49.27%**, which is above the 40% target.

### Business Meaning

This page shows that the business is performing positively from a sales and margin perspective.

From a planning perspective, the current dataset does not show an urgent replenishment need. Instead, the business should monitor stock levels carefully and avoid unnecessary replenishment.

### Planning Action

Recommended actions from this page:

- Monitor top distributors by sales.
- Track whether high-sales regions have enough stock.
- Continue monitoring Net Demand and Order Proposal.
- Maintain first-half-month sales performance above the 40% target.

---

## Page 2 — Demand & Revenue Drivers

![Demand & Revenue Drivers](../images/page-2-demand-revenue-drivers.png)

### Purpose

This page identifies which categories, SKUs, areas, customer segments, and regions are driving sales performance.

The purpose of this page is to support demand planning prioritization.

Before making inventory or replenishment decisions, planners need to know:

- Which products are important
- Which categories drive revenue
- Which areas or customer segments contribute most to sales
- Which products should be reviewed more closely in demand planning

### Main Visuals

| Visual | Purpose |
|---|---|
| Net Sales & Gross Margin % by Category | Compare category revenue and profitability |
| Category Profitability & Discount Analysis | Review sales, margin, and discount by category |
| Priority SKUs by Net Sales | Identify top-selling SKUs |
| Sales Contribution by Area | Identify high-performing areas |
| Sales Mix by Customer Segment and Region | Understand customer segment contribution |

### What Users Can Know from This Page

Users can know:

- Which category contributes the most revenue
- Which SKUs are key revenue drivers
- Which areas are commercially important
- Which customer segments are driving sales
- Whether a category has strong sales but weak margin

### Key Insight

F&B is the largest revenue contributor, accounting for around **42% of total sales**.

Priority SKUs such as **Mì Gói, Sữa Chua, Sữa Tắm, and Khăn Giấy Ướt** should be reviewed closely in demand planning because they strongly contribute to sales performance.

### Business Meaning

This page helps planners focus their attention on the most important products and categories.

In supply chain planning, not all SKUs should be treated equally. High-revenue SKUs need closer monitoring because shortage or overstock in these products can have a stronger impact on business performance.

### Planning Action

Recommended actions from this page:

- Prioritize top-selling SKUs in demand review.
- Monitor F&B category closely because it contributes the largest sales share.
- Compare sales contribution with gross margin to avoid focusing only on high-sales but low-margin products.
- Use SKU priority to support inventory and replenishment review.

---

## Page 3 — Inventory Health & Stock Cover

![Inventory Health & Stock Cover](../images/page-3-inventory-health-stock-cover.png)

### Purpose

This page monitors inventory health, stock cover, understock risk, overstock risk, incoming stock, and distributor-SKU inventory condition.

The main purpose is to help users understand whether inventory is too low, healthy, or excessive.

### Main Metrics

| Metric | Meaning |
|---|---|
| Planning Demand PCS | Demand used for planning calculation |
| NPP Stock PCS | Stock available at distributor level |
| Incoming PCS | Incoming stock quantity |
| Understock SKU Count | Number of SKUs with low stock cover |
| Overstock SKU Count | Number of SKUs with high stock cover |
| Stock Cover Months | How many months current stock can cover demand |

### What Users Can Know from This Page

Users can know:

- Whether stock is enough to cover demand
- Which SKUs have understock risk
- Which SKUs have overstock risk
- Which distributor-SKU combinations need review
- Whether the main issue is shortage or excess inventory

### Key Insight

The dashboard identifies:

- **0 understock SKUs**
- **29 overstock SKUs**

under the selected stock cover logic.

### Business Meaning

The main inventory issue is not shortage.

The bigger issue is **overstock risk**, meaning some SKUs have more stock than needed based on current demand.

This is an important supply chain planning insight because high stock cover can lead to:

- Slow-moving inventory
- Higher holding cost
- Lower inventory efficiency
- Risk of obsolete or expired stock
- Poor working capital efficiency

### Planning Action

Recommended actions from this page:

- Review SKUs with high stock cover.
- Avoid pushing more stock to overstock products.
- Monitor incoming stock carefully.
- Check whether high-stock SKUs have low recent demand.
- Use stock cover status to support replenishment decisions.

---

## Page 4 — Stock Rebalancing & Allocation Readiness

![Stock Rebalancing & Allocation Readiness](../images/page-4-stock-rebalancing-allocation.png)

### Purpose

This page converts inventory insights into planning actions.

The page focuses on answering:

> If there is no immediate replenishment need, what should the planning team do next?

Instead of only asking whether more stock should be ordered, this page helps identify whether the business should:

- Hold unnecessary replenishment
- Review high-surplus SKUs
- Monitor distributor stock imbalance
- Consider stock rebalancing

### Main Metrics

| Metric | Meaning |
|---|---|
| Total Stock PCS | Total stock across the system |
| NPP Stock PCS | Stock at distributor level |
| WH Stock PCS | Stock at warehouse level |
| Net Demand PCS | Additional demand after considering stock cover logic |
| Stock Surplus PCS | Stock quantity above target level |
| Overstock SKU Count | Number of SKUs with overstock risk |

### What Users Can Know from This Page

Users can know:

- Whether replenishment is required
- Which products have the highest stock surplus
- Which distributors are holding high inventory
- Which SKUs should be reviewed for overstock
- What planning action should be taken by distributor-SKU

### Key Insight

Net Demand and Order Proposal are currently **0**, while Stock Surplus is around **3.41M PCS**.

### Business Meaning

The recommended action is not to replenish more stock immediately.

Instead, the planning team should:

- Hold unnecessary replenishment
- Review high-surplus SKUs
- Monitor stock movement
- Consider stock rebalancing where needed

This is an important supply chain planning insight because good planning is not only about ordering more stock.

Sometimes the correct action is to avoid over-ordering and reduce overstock risk.

### Planning Action

Recommended actions from this page:

1. **Hold unnecessary replenishment**  
   Since Net Demand is 0, new replenishment orders should be reviewed carefully.

2. **Review high-surplus SKUs**  
   Products with high surplus should be checked for slow movement or demand changes.

3. **Monitor distributor stock imbalance**  
   Distributors with high stock should be reviewed to avoid excess inventory.

4. **Consider stock rebalancing**  
   If some distributors have excess stock while others have lower stock, rebalancing may be considered.

---

## Page 5 — Revenue Phasing & Invoicing Follow-up

![Revenue Phasing & Invoicing Follow-up](../images/page-5-revenue-phasing-invoicing.png)

### Purpose

This page tracks first-half-month sales performance and checks whether revenue is phased properly across the month.

The purpose is to support revenue phasing and invoicing follow-up.

In supply chain operations, revenue or invoicing may sometimes be delayed toward the end of the month. This can create pressure on operations, logistics, and invoicing teams.

This page helps monitor whether sales are achieved earlier in the month or skewed toward the second half.

### Main Metrics

| Metric | Meaning |
|---|---|
| Net Sales | Total sales value |
| H1 Sales | Sales in the first half of the month |
| H1 Sales % | Percentage of sales achieved in the first half |
| Gap to 40% Target | Difference between actual H1 Sales % and target |
| H1 Target Status | Whether H1 sales performance is on track |

### What Users Can Know from This Page

Users can know:

- How much sales happened in the first half of the month
- Whether H1 Sales % reached the 40% target
- Whether sales are skewed toward the second half
- Which months are on track or behind target
- Whether daily sales show an end-of-month spike

### Key Insight

H1 Sales % is **49.27%**, which is **9.27 percentage points above** the 40% target.

The revenue phasing status is currently **On Track**.

### Business Meaning

Sales are not heavily delayed toward the end of the month.

This suggests that current revenue phasing is healthy under the available dataset.

### Planning Action

Recommended actions from this page:

- Maintain first-half-month sales performance above 40%.
- Monitor months where H1 Sales % drops below target.
- Check daily sales patterns for end-of-month spikes.
- In future versions, connect this analysis with Bill of Lading status and invoicing delay root causes.

---

# 8. Main Findings

The main findings from this dashboard are:

1. Business performance is positive, with **78.91bn Net Sales** and **17.91% Gross Margin**.
2. F&B is the strongest revenue-driving category.
3. Key sales-driving SKUs should be prioritized in demand review.
4. There is no immediate replenishment requirement because Net Demand is currently **0**.
5. The main inventory issue is overstock, not understock.
6. Stock Surplus is approximately **3.41M PCS**.
7. The planning recommendation is to hold unnecessary replenishment and review high-surplus SKUs.
8. Revenue phasing is On Track, with H1 Sales % above the 40% target.

---

# 9. Recommended Planning Actions

Based on the current dashboard results, the recommended planning actions are:

## 9.1 Review Overstock SKUs

Focus on products with high stock surplus and high stock cover.

These SKUs should be reviewed because excessive inventory can increase holding cost and reduce inventory efficiency.

## 9.2 Hold Unnecessary Replenishment

Since Net Demand is currently 0, new replenishment orders should be reviewed carefully before execution.

The current data does not support immediate additional replenishment.

## 9.3 Monitor Distributor Stock Imbalance

Distributors with high NPP stock should be monitored to avoid slow-moving inventory.

If needed, the planning team can investigate whether stock can be rebalanced between distributors.

## 9.4 Prioritize Key Revenue SKUs

High-sales SKUs should still be reviewed regularly to prevent future shortage.

Even though the current issue is overstock, priority SKUs should remain under close monitoring because they have high business impact.

## 9.5 Maintain Revenue Phasing Performance

Since H1 Sales % is above the 40% target, the current phasing performance should be maintained.

The team should continue tracking whether future months stay above the target.

---

# 10. Key DAX Logic Used

The report uses DAX measures to calculate business metrics and planning indicators.

## 10.1 Sales and Profitability

```DAX
Net Sales = SUMX(FactSales, FactSales[Qty Sold] * FactSales[Unit Price] * (1 - FactSales[Discount Rate]))

Gross Profit = [Net Sales] - [COGS]

Gross Margin % = DIVIDE([Gross Profit], [Net Sales])
```

These measures help evaluate business performance and profitability.

## 10.2 Demand and Stock Cover

```DAX
Planning Demand PCS = COALESCE([Avg Monthly Demand 3M PCS], [Avg Monthly Demand PCS], [Demand PCS])

Stock Cover Months = DIVIDE([NPP Stock After Incoming PCS], [Planning Demand PCS])
```

These measures help estimate how many months the current stock can cover demand.

## 10.3 Net Demand and Order Proposal

```DAX
Target Stock PCS = [Planning Demand PCS] * [Target Stock Cover Months]

Net Demand PCS = MAX(0, [Target Stock PCS] - [NPP Stock After Incoming PCS])

Order Proposal PCS = [Net Demand PCS]
```

These measures help determine whether replenishment is required.

## 10.4 Stock Surplus

```DAX
Stock Surplus PCS = MAX(0, [NPP Stock After Incoming PCS] - [Target Stock PCS])
```

This measure identifies excess stock above the target level.

## 10.5 Revenue Phasing

```DAX
Sales First Half Month =
CALCULATE(
    [Net Sales],
    KEEPFILTERS(DimDate[DayOfMonth] <= 15)
)

Sales First Half % = DIVIDE([Sales First Half Month], [Net Sales])

H1 Gap pp = [Sales First Half %] - 0.4
```

These measures track whether first-half-month sales meet the 40% target.

---

# 11. Data Limitation

The current dataset does not include some advanced supply chain fields such as:

- Bill of Lading linking status
- Stock-in-transit details
- Customer inventory
- Confirmed open orders
- Actual service level
- Forecast accuracy
- Shipment lead time
- Delivery performance

Because of this, some planning logic is simplified for portfolio demonstration purposes.

For example:

- Net Demand is calculated using available demand and inventory data.
- Stock-in-transit and customer inventory are not fully included.
- BL linking impact is listed as a future enhancement.
- Invoicing root-cause analysis is limited because document-level data is not available.

---

# 12. Future Improvements

This report can be improved by adding:

1. **Stock-in-transit data**  
   To improve Net Demand calculation.

2. **Customer inventory data**  
   To better understand stock available at customer/distributor side.

3. **Open order data**  
   To avoid over-replenishment and improve order proposal accuracy.

4. **Bill of Lading status**  
   To analyze how document linking affects invoicing performance.

5. **Forecast vs actual demand comparison**  
   To measure forecast accuracy and demand volatility.

6. **Service level tracking**  
   To understand whether stock availability supports customer fulfillment.

7. **Automated replenishment proposal export**  
   To make the dashboard more useful for operational follow-up.

8. **Scenario planning for different stock cover targets**  
   To test how different target cover assumptions affect Net Demand and Stock Surplus.

---

# 13. What This Project Demonstrates

This project demonstrates my ability to:

- Build a structured Power BI dashboard
- Use DAX measures for business calculations
- Analyze sales and inventory data
- Understand basic supply chain planning logic
- Connect dashboard visuals with business decisions
- Translate data insights into recommended actions
- Present supply chain problems clearly
- Communicate dashboard findings in a business-oriented way

The project reflects a fresher-level but business-oriented understanding of supply chain planning, inventory monitoring, replenishment logic, and revenue phasing analysis.

---

# 14. Final Business Summary

This dashboard shows that the current business performance is positive, with strong Net Sales and healthy first-half-month revenue phasing.

However, from a supply chain planning perspective, the main issue is not shortage. The dashboard indicates that Net Demand and Order Proposal are currently zero, while Stock Surplus and Overstock SKU Count are significant.

Therefore, the key recommendation is:

> Do not immediately replenish more stock. Instead, review overstock SKUs, hold unnecessary replenishment, monitor distributor stock imbalance, and maintain healthy revenue phasing performance.

This project shows how Power BI can be used as a decision-support tool for supply chain planning, not just as a sales visualization report.
