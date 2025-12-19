# Sales & Customers Dashboard Overview

![Sales Dashboard Overview](https://github.com/Ritik574-coder/Bi-Project-/blob/main/Sales%20%26%20Customers%20Dashboard%20overview/Customers%20Dashboard.png)

## Tableau Dashboard Custoemrs
![Customers Dashboard Details](https://github.com/Ritik574-coder/Bi-Project-/blob/main/Sales%20%26%20Customers%20Dashboard%20overview/Sales%20Dashboard.png)

## Introduction

Welcome to the **Sales & Customers Dashboard Overview**, a comprehensive Tableau visualization tool designed to empower sales teams, business analysts, and executives in driving revenue growth and customer-centric strategies. Created as a personal learning project by Ritik Kumar, a passionate data engineering student from India, this dashboard dives deep into 2023 sales performance, profitability trends, and customer behaviors—highlighting key metrics like total sales ($733K), profit ($93K), and top performers.

In today's dynamic retail landscape, understanding year-over-year growth, subcategory hotspots, and customer loyalty is vital for optimizing inventory, targeting campaigns, and boosting margins. This dashboard pulls from real-world sales datasets (sourced from anonymized e-commerce records or public benchmarks like Superstore datasets on Kaggle) to deliver actionable insights. Whether you're a sales manager spotting underperforming subcategories or a marketer analyzing order patterns, this tool highlights:

- **Sales Trends**: Total sales up 20.36% YoY to $733K, with quantity surging 26.83% to 12K units.
- **Profit Breakdowns**: $93K total profit (↑14.24% YoY), with Phones leading subcategories.
- **Customer Insights**: 693 customers (↑8.62% YoY) driving 1,687 orders, averaging $1,058 per customer.
- **Performance Spotlights**: Top 10 customers by profit (e.g., Raymond Buch at $6,781) and distribution by order volume.

Built with Tableau for its intuitive drag-and-drop interface and powerful calculated fields, this dashboard isn't just a report—it's a dynamic analytics hub! Filter by month, subcategory, or customer segment; drill down into trends; or explore profit waterfalls to uncover opportunities like upselling to high-order customers. As a student aspiring to data engineering roles, I built this to apply my skills in ETL, Tableau calculations, and BI while tackling real business challenges like revenue forecasting and customer segmentation.

**Why this matters**: With 2023 data analyzed (as of late 2025), businesses can leverage this to identify growth levers, refine pricing, and personalize engagement—because in sales, data-driven decisions turn insights into dollars.

## Key Features

This dashboard excels through its interactive visuals and revenue-focused storytelling. Here's what you'll find:

- **Overview Cards**: Quick stats on total sales ($733K), profit ($93K), quantity (12K), customers (693), sales per customer ($1,058), and orders (1,687)—all with YoY growth indicators.
- **Trend Analysis**: Line charts for monthly sales, profit, and orders fluctuations (e.g., peaks in Q4), comparing 2023 vs. 2022 with highest/lowest markers.
- **Subcategory Visuals**: 
  - Stacked bars for sales & profit by subcategory (e.g., Phones dominate sales at ~$200K+; Copiers lead profit).
  - Waterfall-style trends over time, highlighting above/below average performance.
- **Customer Breakdown**: Bar charts for order distribution (e.g., 200+ customers with 1 order) and tables for top 10 by profit (e.g., Hunter Lopez at $5,046 profit).
- **Geographic & Temporal Maps**: Optional heatmaps (extendable) for sales density by region/month.
- **Drill-Through Views**: Click into a subcategory like "Phones" for granular profit vs. sales splits, or a customer name for order history.

All visuals are filter-driven for effortless slicing by date, subcategory, or customer metrics, with mobile responsiveness for on-the-go sales reviews.

## Screenshots

Explore the dashboard through these key views:

| Section | Description | Screenshot |
|---------|-------------|------------|
| **Sales Overview** | High-level KPIs, monthly trends (sales/profit/quantity), and subcategory bars showing $733K total sales. | ![Sales Overview](https://github.com/Ritik574-coder/Bi-Project-/blob/main/Sales%20%26%20Customers%20Dashboard%20overview/Customers%20Dashboard.png) |
| **Sales Trends & Subcategories** | Profit/loss bars by subcategory and over-time lines (above/below avg) for 2023 vs. 2022. | ![Sales Trends](https://github.com/Ritik574-coder/Bi-Project-/blob/main/Sales%20%26%20Customers%20Dashboard%20overview/Sales%20Dashboard.png) (bottom sections) |
| **Customers Overview** | Total customers/orders metrics, distribution by order count, and top 10 profit table (e.g., Raymond Buch #1). | ![Customers Overview](/Project%20Image/Customers_Details.png) |
| **Top Customers Drill-Down** | Ranked table with profit/sales/#orders, plus YoY growth charts for customer acquisition. | ![Top Customers](https://github.com/Ritik574-coder/Bi-Project-/blob/main/Sales%20%26%20Customers%20Dashboard%20overview/image/Top%20Customers%20.png) (expanded table) |

*Note: Screenshots are static captures. For the full interactive experience, download the .twbx file from the [Releases](https://github.com/Ritik574-coder/sales-customers-dashboard/releases) section or view the live version on my Tableau Public profile (linked below).*

## Data Sources & Methodology

- **Primary Dataset**: Derived from anonymized sales records (e.g., Superstore-style CSV with ~10K rows from a mid-sized retailer in office supplies/furniture).
- **Key Columns Analyzed**: Order ID, date, subcategory (e.g., Phones, Chairs), sales, profit, quantity, customer name/ID, segment, and ship mode.
- **Tools Used**:
  - **ETL**: Python (Pandas, NumPy) for data cleaning and feature engineering (e.g., YoY % calculations via date diffs and pivots).
  - **Visualization**: Tableau Desktop with custom calculated fields (e.g., `{FIXED [Month]: SUM([Sales])}` for trends, `SUM([Profit])/SUM([Sales])` for margins sliced by parameters).
  - **Mapping**: Tableau's built-in maps for potential geo extensions (e.g., sales by state).
- **Assumptions**: All figures in USD; data for 2022-2023 as of December 19, 2025. No PII; profits computed as sales minus costs.

To replicate: Import the CSV into Tableau, refresh extracts, and apply the calculated fields for live metrics.

## Skills Showcased

As a data engineering student refining my expertise, this project demonstrates a mix of technical and analytical skills gained through coursework and projects:

- **Data Engineering**: ETL workflows in Python—handling transactional sales data (e.g., aggregating subcategories, imputing missing profits), and preparing for efficient Tableau hyper extracts.
- **Business Intelligence**: Tableau mastery including quick filters, dashboard actions (e.g., highlight on subcategory click), and conditional formatting. Advanced LOD expressions for aggregations like YoY growth and top-N rankings.
- **Data Visualization**: Strategic chart selection (e.g., stacked bars for subcategory splits, lines for temporal trends) to balance detail and clarity for sales users.
- **SQL & Analytics**: Prep queries for joins (e.g., orders and customers tables) and cohort analysis, drawing from retail analytics practices.
- **Soft Skills**: Stakeholder-focused design—addressing sales needs like "top profit drivers"—plus iterative testing for intuitive navigation.

This dashboard reflects my evolution from basic queries to full BI solutions, with emphasis on actionable storytelling in revenue domains.

## How to Use This Dashboard

1. **Download**: Grab the .twbx file from [GitHub Releases](https://github.com/Ritik574-coder/sales-customers-dashboard/releases).
2. **Open in Tableau**: Launch Tableau Desktop (free trial or Public edition) and load the file.
3. **Interact**:
   - Use top-right filters to slice by month, subcategory, or customer segment.
   - Click a bar (e.g., "Phones") to highlight trends across views via actions.
   - Export sheets or dashboards as PDFs for sales reports.
4. **Customize**: Adjust themes, integrate live CRM data (e.g., via connectors), or expand with custom parameters like profit thresholds.

Pro Tip: Publish to Tableau Public or Server for team sharing and scheduled refreshes.

## Roadmap & Future Enhancements

- Integrate live e-commerce feeds (e.g., Shopify connectors) for real-time updates.
- Add predictive elements: Forecast Q4 sales using ML models (e.g., ARIMA in Python, blended into Tableau).
- Segmentation Focus: RFM analysis for customer lifetime value.
- Accessibility: Alt-text for all visuals and high-contrast modes.

Contributions welcome—fork the repo and submit a PR!

## About the Author

Hi, I'm **Ritik Kumar**, a dedicated data engineering student based in India. Currently bridging academia and industry, I'm passionate about turning raw data into revenue-boosting insights. From debugging LOD expressions late into the night to exploring sales forecasting ethics, I thrive on impactful problem-solving. This dashboard is one of many in my portfolio, highlighting my growth in BI and commercial analytics.

Let's connect—I'd love to discuss sales trends, collaborate on tools, or exchange tips on data careers!

## Connect With Me

- **GitHub**: [Ritik574-coder](https://github.com/Ritik574-coder) – Fork this repo and star for updates!
- **LinkedIn**: [Ritikkumar](https://www.linkedin.com/in/ritik-kumar-b81b32375/) – Let's network on data and sales opportunities.
- **Tableau Public**: [Ritik Sky](https://public.tableau.com/app/profile/ritik.sky) – Check out my other viz experiments.
- **X (Twitter)**: [@KarlX279873](https://x.com/KarlX279873) – Quick takes on tech and trends.
- **Instagram**: [@ritik_sky1](https://www.instagram.com/ritik_sky1/?__pwa=1) – Behind-the-scenes of my learning journey.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details. Feel free to use, modify, and share—just give credit where it's due!

---

*Last Updated: December 19, 2025*  
*Built with ❤️ in India*