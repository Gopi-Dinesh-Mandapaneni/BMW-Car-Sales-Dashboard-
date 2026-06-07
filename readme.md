### **BMW Car Sales Dashboard**



###### **Project Details**

Tool:	      Microsoft Power BI Desktop

File:	      bmw\_car\_sales.pbix

Created:	      November 2025

Data Source:   BMW Car Sales Dataset (Internal)

Report Pages:  1 (single-page interactive dashboard)

Visuals:	      10 interactive visuals + 4 slicers



###### **Data Structure**

The report is built on a single table called bmw\_car\_sales. Here's what each column contains:



Column:	       Description

Model:	       BMW car model (e.g., 3 Series, X5, M3, etc.)

Color	:       Exterior color of the vehicle

Fuel\_Type:      Type of fuel (Petrol, Diesel, Electric, Hybrid, etc.)

Region:	       Sales region or geographic market

sales\_year:     Year the sale was recorded.

Sales\_Volume:   Number of units sold



###### **Revenue	Revenue generated from sales (numeric)**



Two calculated measures have also been added on top of the raw data:

• total revenue — a DAX measure that computes the sum of revenue across filtered selections

• total sales volume — a DAX measure for the total number of cars sold

Dashboard Visuals

The report is a single-page dashboard. Here's a breakdown of what each visual does:



**KPI Summary Cards**

Right at the top, you'll find four summary cards showing the headline numbers: total revenue, total sales volume, the top-performing region (with its revenue), and the best-selling car model. These update dynamically as you apply any filters.



**Revenue \& Units Sold Over Time (Combo Chart)**

A combined bar and line chart plotted against year. The bars show total units sold (Sales\_Volume), while the line overlays total revenue. This makes it easy to spot whether revenue growth matches unit growth, or whether there are years when revenue outpaced volume (or vice versa).



**Revenue by Car Colour (Column Chart)**

A vertical bar chart breaking down total revenue by car colour. Useful for understanding which colours are most popular with buyers and, more importantly, which ones generate the most revenue.



**Revenue by Car Model (Treemap)**

A treemap in which each tile represents a BMW model, sized in proportion to its contribution to total revenue. Models that dominate the revenue mix stand out immediately at a glance.



**Revenue by Region (Doughnut Chart)**

A doughnut chart showing the revenue split across sales regions. Hovering or clicking a segment filters the entire dashboard to that region.



**Revenue by Fuel Type (Doughnut Chart)**

Similar to the region doughnut, this chart shows the revenue share for each fuel type. Tooltips also show the number of cars sold per fuel type, giving you volume context alongside revenue.



**Slicers (Filters)**

Four slicers sit on the dashboard, letting you slice the data however you need:

• Year — 	 filter by one or more sales years

• Sales Region — focus on a specific market

• Car Model — 	 narrow down to particular BMW models

• Fuel Type — 	 filter by engine/fuel type



All slicers interact with every visual on the page, so any selection you make cascades across the entire dashboard instantly.



###### **How to Use This Report**

• Open bmw\_car\_sales.pbix in Power BI Desktop (or publish to Power BI Service).

• Use the four slicers on the left side to filter down to the time period, region, model, or fuel type you care about.

• Click any element in a chart (a bar, a treemap tile, a doughnut slice) to cross-filter the other visuals.

• The KPI cards at the top always reflect your current filter context.

• To reset all filters, click the reset/clear button in the slicer or use Ctrl+Z to undo.



###### **File \& Environment Info**

File Name:		bmw\_car\_sales.pbix

File Size:		\~2.1 MB

Power BI Version:	2025.11 (November 2024)

Data Refresh:		Static dataset embedded in the file.

External Connections:	None (self-contained)

Theme:			CY25SU11 base theme with Temperature accent



The dataset is embedded directly in the DataModel (VertiPaq/xVelocity engine), so no external database connection is needed to open and interact with the report.



**Notes \& Limitations**

• This is a static dataset — the data does not refresh automatically. To update it, the source data would need to be re-imported.

• The report has a single page. If additional breakdowns (e.g., by dealer, by country sub-region) are needed, new report pages can be added.



