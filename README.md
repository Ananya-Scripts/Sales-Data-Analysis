# Sales-Data-Analysis
Power BI dashboard analysing 3 years of B2B sales data revenue, profit, regional split, and sales-rep attainment. Built with Power Query, DAX, and a star-schema model.

Sales Performance Dashboard (2022–2024)

•	Short description-

An end-to-end Power BI analytics project that tracks revenue, profit, and sales-rep attainment for a fictional B2B reseller across four regions over three years. The project covers the full BI workflow data exploration in Python, modelling and DAX in Power BI Desktop, and an interactive three-page dashboard built for executive review.
The purpose is twofold: Demonstrate practical proficiency in Power BI modelling, DAX, Power Query, and dashboard design.
Show how the same dataset can be interrogated from multiple angles time, geography, product, and individual performance to surface decisions a sales director would actually act on.

•	Tech stack-

Data exploration - Python · pandas · NumPy · Jupyter Lab
Data transformation- Power Query (M)
Modelling- Power BI Desktop · star schema
Calculations- DAX (measures, time intelligence)
Version control- Git · GitHub · PBIP format

•	Data source-

The dataset is synthetic, generated using OpenAI. ChatGPT was prompted to produce a realistic-looking B2B sales history covering 2022–2024:

	Orders — 11,306 transactional rows (Order ID, dates, customer, product, rep, region, quantity, price, discount, sales, cost, profit).

	Targets — 180 rows of quarterly revenue targets per sales rep.

(The data is fictional. No real person, customer, or organisation is depicted, and no GDPR-relevant processing takes place. This makes the project safe to publish openly while still being structurally identical to the kind of dataset used in real sales analytics.)

•	Features-

Three-page interactive dashboard designed for a 16:9 executive review layout.

	Page 1 – Overview: KPI cards (Total Revenue, Total Profit, Average Order Value, Profit Margin) and a smoothed monthly trend of sales against profit.

	Page 2 – Regional & Product Breakdown: revenue by region, donut of category mix, and top-10 products by revenue.

	Page 3 – Sales-Rep Attainment: attainment percentage per rep against target, plus yearly and segment views.

Star-schema data model with Orders and Targets as fact tables, joined to Customer, Product, Sales Rep, and a generated Date dimension.

DAX measures for Profit Margin, Average Order Value, Attainment %, year-over-year growth, and time-intelligence comparisons (same period last year).
Power Query transformations with explicit type coercion to avoid locale-sensitive parsing errors.

Custom tooltip pages on every visual so the underlying numbers are always one hover away.

Reproducible EDA notebook in Jupyter that re-derives every headline figure shown on the dashboard, providing an independent check on the DAX.

•	Business impact & insights-

The dashboard surfaces several findings that would shape commercial strategy:

Revenue grew year-on-year: 2022 → 2.43 M, 2023 → 2.51 M, 2024 → 2.87 M. That is roughly 18 % growth from 2022 to 2024, with the steepest jump coming in the most recent year a signal that whatever changed in 2024 (new rep, new region focus, pricing) is worth replicating.

North America is the volume leader, but not the only story: NA contributes 3.32 M (≈ 42 % of revenue), Europe 2.24 M, APAC 1.67 M, and LATAM 0.59 M. LATAM is small enough to flag either as an under-invested opportunity or as a market to deprioritise a decision the dashboard frames clearly.

Technology is the engine: the Technology category accounts for 63 % of total sales, with Laptop Pro 15 (1.03 M) and Desktop Tower (0.77 M) as the two highest-grossing SKUs. Office Supplies are negligible at 1.4 %  a candidate for catalogue rationalisation.

The Consumer segment outweighs Corporate and Small Business combined for revenue, suggesting that the go-to-market motion is more transactional than enterprise which has direct implications for headcount allocation between SDRs and account executives.

Rep attainment is tightly clustered: 3 of 15 reps cleared 100 % of target; the remaining 12 land between 95 % and 100 %. There are no severe under-performers, which means coaching investment is better spent on lifting the median than on remediation.

Profit margin is healthy and stable at 33.74 % across the three-year window, indicating that growth has not come at the cost of discounting.

•	Screenshots/ Demo Pictures-

<img width="827" height="345" alt="Screenshot4" src="https://github.com/user-attachments/assets/52a0ebab-4281-4967-a35e-dcb978f12555" />
<img width="734" height="347" alt="Screenshot 5" src="https://github.com/user-attachments/assets/97548760-05fd-41cd-81aa-da451db88b6b" />
<img width="814" height="347" alt="Screenshot 3" src="https://github.com/user-attachments/assets/7214510f-9860-4ff3-94f1-93b203447d7c" />
<img width="817" height="346" alt="Screenshot 2" src="https://github.com/user-attachments/assets/25dd0856-1212-41c0-9e20-22f12bea5fb5" />
<img width="740" height="372" alt="Screenshot " src="https://github.com/user-attachments/assets/f232d9f0-c100-4cfd-bb16-98a99d7cda7d" />
<img width="725" height="402" alt="sales data SS" src="https://github.com/user-attachments/assets/cc2a50b9-a728-4417-85a5-44f49f77dfa9" />
<img width="714" height="407" alt="sales data SS 3" src="https://github.com/user-attachments/assets/3623046c-2661-4f09-b406-56f0515af4ca" />
<img width="720" height="407" alt="sales data SS 2" src="https://github.com/user-attachments/assets/73486fe4-a96d-43d1-874c-5b55994d4eb7" />
