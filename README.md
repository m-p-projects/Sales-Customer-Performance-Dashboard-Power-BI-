Global Sales & Customer Performance Dashboard

1. Project Overview

This project represents the final capstone for Case Study 14, focusing on the development of a comprehensive business intelligence solution. The dashboard provides a high-level executive summary of global sales performance while allowing for deep dives into customer demographics and product-level profitability.

The Problem: A fictional global retailer struggled to unify transactional data from multiple regions, resulting in delayed reporting and missed opportunities for regional growth.

The Solution: An end-to-end Power BI implementation featuring a refined Star Schema, custom DAX measures for comparative analysis, and a high-accessibility design theme.

2. Technical Toolkit

Platform: Power BI Desktop

Theme: Accessible City Park (Customised for high contrast and readability)

Calculations: Advanced DAX (Data Analysis Expressions) including Time Intelligence and Ranking.

3. Data Architecture & Modelling

The project utilises a robust Star Schema to optimise query performance and ensure a clear "single source of truth" for the business.

Central Fact Table: Sales_Data (containing transactional records).

Dimension Tables: Customers, Products, Regions, and a dedicated Calendar table for time-series analysis.

Modelling Best Practices: Implemented one-to-many (1:*) relationships and ensured accurate filter propagation across all report pages.

4. Analytical Features & DAX

I used several complex measures to provide stakeholders with actionable insights. Key formulas include:

Total Sales (Revenue):

Total Sales = SUM(Sales[Revenue])


Total Profit:

Total Profit = SUM(Sales[Profit])


Profit Margin %:

Profit Margin = DIVIDE([Total Profit], [Total Sales], 0)


Year-to-Date (YTD) Sales:

YTD Sales = TOTALYTD([Total Sales], 'Calendar'[Date])


Previous Year Sales (for YoY comparison):

Previous Year Sales = CALCULATE([Total Sales], SAMEPERIODLASTYEAR('Calendar'[Date]))


5. Visual Design & UX

Accessibility First: Utilised an accessible colour palette to ensure the report is inclusive for users with visual impairments.

Drill-Through Functionality: Enabled users to right-click on any region or product category to navigate to a "Details" page for granular transactional analysis.

Interactivity: Integrated Slicers and Cross-Filtering to allow for dynamic exploration of the data by Year, Quarter, and Product Category.

6. Business Impact

Efficiency: Automated the reporting workflow, reducing the manual effort required to generate monthly performance summaries.

Insight Discovery: Uncovered seasonal trends in specific product categories, allowing for better inventory management during peak periods.

7. Repository Structure

Casestudy 14 FINAL PROJECT.pbix: The primary Power BI source file.

Dashboard_Presentation.pdf: A walkthrough of the key visual pages.

/assets: Screenshots demonstrating the Data Model view and primary report pages.

8. Usage

To explore the interactivity, download the .pbix file and open it in Power BI Desktop. For a quick overview, please refer to the visual assets in the /assets folder.
