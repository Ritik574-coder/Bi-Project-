
# Data Jobs Dashboard Overview

![Power BI Dashboard](https://github.com/Ritik574-coder/Bi-Project-/blob/main/Data%20Job%20Dashboard%20Overview/Project%20Image%20two.png)

## Power BI Dashboard Drill
![Power BI Dashboard Drill](https://github.com/Ritik574-coder/Bi-Project-/blob/main/Data%20Job%20Dashboard%20Overview/Project%20Image%20three%20.png)

## Introduction

Welcome to the **Data Jobs Dashboard Overview**, a comprehensive Power BI visualization tool designed to empower job seekers, aspiring data professionals, and career enthusiasts in the ever-evolving world of data careers. Created as a personal learning project by Ritik Kumar, a passionate data engineering student from India, this dashboard dives deep into the landscape of data-related jobs—think data engineers, scientists, analysts, and more.

In today's competitive job market, understanding trends like salary benchmarks, geographic hotspots, and role popularity can make all the difference. This dashboard pulls from real-world job data (sourced from public datasets like those on Kaggle or LinkedIn aggregates) to provide actionable insights. Whether you're a student like me plotting your next career move or a professional scouting opportunities, this tool highlights:

- **Job Market Trends**: Track the rise (or dips) in data job postings throughout 2024.
- **Salary Breakdowns**: Median annual and hourly rates, with comparisons across roles.
- **Geographic Insights**: Where the hottest data job markets are globally—spoiler: North America and Asia lead the pack.
- **Role Spotlights**: From high-paying machine learning engineers to in-demand data analysts.

Built with Power BI for its intuitive drag-and-drop interface and powerful DAX measures, this dashboard isn't just a static report—it's interactive! Drill down into specific job titles, filter by location, or explore salary distributions to uncover patterns that inform your decisions. As a student transitioning into a data engineer role, I crafted this to bridge my learning in visualization, ETL processes, and business intelligence while helping others navigate the data job ecosystem.

**Why this matters**: With over 478K data jobs analyzed (as of late 2024), the field is booming, but so is the competition. Use this dashboard to spot opportunities, benchmark your skills, and stay ahead—because in data, knowledge truly is power.

## Key Features

This dashboard shines through its interactive elements and data-driven storytelling. Here's what you'll find:

- **Overview Cards**: Quick stats on total job count (478,895K+), median salaries ($113K annual, $47.62 hourly), and a star rating for overall market health.
- **Trend Analysis**: Line charts showing monthly job count fluctuations in 2024, revealing seasonal peaks (e.g., Q2 surges).
- **Salary Visuals**: 
  - Bar charts for highest-paying roles (e.g., Senior Machine Learning Engineer at ~$150K+).
  - Scatter plots comparing hourly vs. annual salaries across job types.
- **Top Jobs Breakdown**: Horizontal bars ranking roles by count and salary (Data Engineer tops with 98K+ postings).
- **Global Map**: Heatmap-style visualization of job density by region—North America dominates with dense clusters in the US.
- **Drill-Through Pages**: Click into a role like "Senior Data Scientist" for deeper dives, including:
  - Donut charts for degree requirements (74% true mention) and health insurance perks (19% true).
  - Platform breakdowns (e.g., LinkedIn leads with 50%+ of postings).
  - Data type filters (94% full-time roles).

All visuals are responsive, mobile-friendly, and powered by slicers for easy filtering by date, location, or job attributes.

## Screenshots

Explore the dashboard through these key views:

| Section | Description | Screenshot |
|---------|-------------|------------|
| **Main Overview** | High-level KPIs, trends, and global map showing 339K+ jobs with $115.5K avg salary. | ![Main Overview](/Project%20Image/Project%20image%20oen%20.png) |
| **Job Trends & Salaries** | 2024 job count trends and hourly vs. annual salary bubbles for top roles. | ![Trends & Salaries](/Project%20Image/Project%20Image%20two.png) |
| **Highest Paying Roles** | Bar chart of top salaries (e.g., Software Engineer at $150K) and job trends table. | ![Highest Paying](images/dashboard-overview-1.png) (bottom section) |
| **Drill-Through: Senior Data Scientist** | Salary gauges, global job map, platform bars, and employment type pie. | ![Drill-Through](/Project%20Image/Project%20Image%20three%20.png) |

*Note: Screenshots are static captures. For the full interactive experience, download the .pbix file from the [Releases](https://github.com/Ritik574-coder/data-jobs-dashboard/releases) section or view the live version on my Tableau Public profile (linked below).*

## Data Sources & Methodology

- **Primary Dataset**: Aggregated from public sources like Indeed, LinkedIn, and Glassdoor APIs (anonymized and cleaned via Python/Pandas for ETL).
- **Key Columns Analyzed**: Job title, salary (annual/hourly), location (lat/long for mapping), posting date, platform, degree requirement, insurance perks, and employment type.
- **Tools Used**:
  - **ETL**: Python (Pandas, NumPy) for data cleaning and transformation.
  - **Visualization**: Power BI Desktop with custom DAX measures (e.g., `Average Salary = AVERAGE(Salary[Annual])`, `YoY Growth = DIVIDE([Total 2024] - [Total 2023], [Total 2023])`).
  - **Mapping**: Integrated Bing Maps for geospatial visuals.
- **Assumptions**: Salaries in USD; data refreshed quarterly. No PII included for privacy.

To replicate: Import the CSV into Power BI, apply the provided DAX, and connect to a map visual.

## Skills Showcased

As a data engineering student honing my craft, this project highlights a blend of technical and soft skills I've built through self-study and hands-on practice:

- **Data Engineering**: ETL pipelines in Python—scraping, cleaning noisy job data (e.g., handling missing salaries with imputation), and optimizing for Power BI import.
- **Business Intelligence**: Advanced Power BI features like drill-throughs, bookmarks, and conditional formatting. Custom DAX for metrics like median calculations and percentage slicers.
- **Data Visualization**: Choosing the right chart types (e.g., bubbles for salary correlations, maps for geo-trends) to tell a compelling story without overwhelming the user.
- **SQL & Analytics**: Underlying queries for data prep (e.g., JOINs on job_postings and locations tables) and trend analysis inspired by AdventureWorks practice.
- **Soft Skills**: User-centric design—focusing on job seekers' pain points like "What's the ROI on a data science degree?"—plus project management from ideation to deployment.

This dashboard is part of my journey from SQL newbie to BI enthusiast, incorporating lessons from DAX troubleshooting and color palette experiments for professional appeal.

## How to Use This Dashboard

1. **Download**: Grab the .pbix file from [GitHub Releases](https://github.com/Ritik574-coder/data-jobs-dashboard/releases).
2. **Open in Power BI**: Launch Power BI Desktop (free from Microsoft) and load the file.
3. **Interact**:
   - Use slicers (top-right) to filter by year, region, or role.
   - Click a bar on the "Top Jobs" chart to drill through.
   - Export visuals as PDFs or embed in reports.
4. **Customize**: Tweak themes, add your data, or connect to live sources like Azure SQL.

Pro Tip: For mobile viewing, publish to Power BI Service (requires free account) and share via app.powerbi.com.

## Roadmap & Future Enhancements

- Integrate real-time APIs (e.g., LinkedIn Jobs) for live updates.
- Add predictive analytics: Forecast 2025 job growth using Python ML models (e.g., Prophet for trends).
- Multilingual support: Hindi/English toggles for Indian users.
- Accessibility: Alt-text for all visuals and color-blind friendly palettes.

Contributions welcome—fork the repo and submit a PR!

## About the Author

Hi, I'm **Ritik Kumar**, a dedicated data engineering student based in India. Currently bridging academia and industry, I'm passionate about turning raw data into career-boosting insights. From crafting viral song lyrics in my downtime to debugging DAX at midnight, I thrive on creative problem-solving. This dashboard is one of many projects in my portfolio, showcasing my growth in BI and visualization.

Let's connect—I'd love to chat about data trends, collab on projects, or share job hunt tips!

## Connect With Me

- **GitHub**: [Ritik574-coder](https://github.com/Ritik574-coder) – Fork this repo and star for updates!
- **LinkedIn**: [Ritikkumar](https://www.linkedin.com/in/ritik-kumar-b81b32375/) – Let's network on data opportunities.
- **Tableau Public**: [Ritik Sky](https://public.tableau.com/app/profile/ritik.sky) – Check out my other viz experiments.
- **X (Twitter)**: [@KarlX279873](https://x.com/KarlX279873) – Quick takes on tech and trends.
- **Instagram**: [@ritik_sky1](https://www.instagram.com/ritik_sky1/?__pwa=1) – Behind-the-scenes of my learning journey.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details. Feel free to use, modify, and share—just give credit where it's due!

---

*Last Updated: December 17, 2025*  

*Built with ❤️ in India*
