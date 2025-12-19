# HR Dashboard Overview

![HR Dashboard Overview](https://github.com/Ritik574-coder/Bi-Project-/blob/main/HR%20Analytics%20Dashboard/HR%20_%20Summary.png)

## Tableau Dashboard Details
![HR Dashboard Details](https://github.com/Ritik574-coder/Bi-Project-/blob/main/HR%20Analytics%20Dashboard/HR%20_%20Details.png)

## Introduction

Welcome to the **HR Dashboard Overview**, a comprehensive Tableau visualization tool designed to empower HR leaders, managers, and teams in optimizing workforce strategies and fostering inclusive workplaces. Created as a personal learning project by Ritik Kumar, a passionate data engineering student from India, this dashboard dives deep into the dynamics of employee data—covering demographics, performance, compensation, and retention trends.

In today's fast-paced business environment, gaining clarity on metrics like turnover rates, salary equity, and departmental health is essential for strategic decisions. This dashboard pulls from real-world HR datasets (sourced from anonymized company records or public benchmarks like those on Kaggle) to deliver actionable insights. Whether you're an HR professional analyzing retention risks or a manager reviewing team performance, this tool highlights:

- **Workforce Trends**: Track active headcount (7,984 employees), hiring spikes (8,950 total hires), and termination patterns (966 cases).
- **Demographic Breakdowns**: Gender balance (46% Female, 54% Male), age distributions (peak 35-44), and education levels (Bachelor's dominant at ~70%).
- **Compensation Insights**: Average salaries (~$60K-$90K), with equity checks across education and roles.
- **Retention Spotlights**: Tenure averages (~6 years), longest in Finance (9+ years), and location hotspots (e.g., New York City and Buffalo).

Built with Tableau for its intuitive drag-and-drop interface and powerful calculated fields, this dashboard isn't just a report—it's a living analytics hub! Filter by department, drill down into employee details, or explore performance heatmaps to uncover opportunities like reducing high-turnover in recent hires. As a student aspiring to data engineering roles, I built this to apply my skills in ETL, Tableau calculations, and BI while addressing real HR challenges like diversity audits and talent planning.

**Why this matters**: With 7,984 active employees analyzed (as of late 2025), organizations can use this to boost engagement, ensure fair pay, and align talent with business goals—because in HR, data-driven empathy drives success.

## Key Features

This dashboard excels through its interactive visuals and insightful storytelling. Here's what you'll find:

- **Overview Cards**: Quick stats on active employees (7,984), total hires (8,950), terminations (966), and overall retention health.
- **Trend Analysis**: Line charts for hiring/termination fluctuations, showing steady growth in 2023-2025.
- **Demographic Visuals**: 
  - Pie charts for gender and education breakdowns.
  - Bubble charts for age-salary correlations (e.g., Masters earners at $80K+).
- **Department Breakdown**: Horizontal bars ranking departments by size (Customer Service leads at 1,489; HR smallest at 20).
- **Location Map**: Heatmap of employee density—New York and Michigan dominate with clusters in NYC and Buffalo.
- **Performance & Details Views**: 
  - Heatmaps for performance by education (50% "Good" rating).
  - Filterable employee table with 13+ samples, sortable by salary ($55K–$92K), hire date, and tenure bars (up to 10 years).

All visuals are filter-driven for effortless slicing by status, location, or demographics, with mobile responsiveness for remote HR reviews.

## Screenshots

Explore the dashboard through these key views:

| Section | Description | Screenshot |
|---------|-------------|------------|
| **Main Overview** | High-level KPIs, department bars, demographics pies, and location map showing 7,984 active employees. | ![Main Overview](https://github.com/Ritik574-coder/Bi-Project-/blob/main/HR%20Analytics%20Dashboard/HR%20_%20Summary.png) |
| **Demographics & Income** | Education-age distributions, gender-salary bubbles, and performance heatmaps. | ![Demographics & Income](https://github.com/Ritik574-coder/Bi-Project-/blob/main/HR%20Analytics%20Dashboard/image/Screenshot%202025-12-01%20122119.png) (bottom sections) |
| **Employee Details** | Filterable list with demographics, roles, geographies, salaries, statuses, and tenure visuals. | ![Employee Details](https://github.com/Ritik574-coder/Bi-Project-/blob/main/HR%20Analytics%20Dashboard/HR%20_%20Details.png) |


*Note: Screenshots are static captures. For the full interactive experience, download the .twbx file from the [Releases](https://github.com/Ritik574-coder/hr-dashboard-overview/releases) section or view the live version on my Tableau Public profile (linked below).*

## Data Sources & Methodology

- **Primary Dataset**: Derived from anonymized HR records (e.g., employee CSV with ~8K rows from a mid-sized US firm in tech/services).
- **Key Columns Analyzed**: Employee ID, demographics (gender/age/education), role, location, salary, hire date, status, tenure, and performance ratings.
- **Tools Used**:
  - **ETL**: Python (Pandas, NumPy) for data cleaning and feature engineering (e.g., calculating tenure via date diffs).
  - **Visualization**: Tableau Desktop with custom calculated fields (e.g., `{FIXED [Department]: COUNTD([Employee ID])}` for active counts, `AVG([Salary])` sliced by parameters).
  - **Mapping**: Tableau's built-in maps for state-level geo visuals.
- **Assumptions**: Salaries in USD; data as of December 19, 2025. No PII; tenure computed dynamically.

To replicate: Import the CSV into Tableau, refresh extracts, and apply the calculated fields for live metrics.

## Skills Showcased

As a data engineering student refining my expertise, this project demonstrates a mix of technical and analytical skills gained through coursework and projects:

- **Data Engineering**: ETL workflows in Python—handling sensitive HR data (e.g., anonymizing demographics, imputing missing tenures), and preparing for efficient Tableau hyper extracts.
- **Business Intelligence**: Tableau mastery including quick filters, dashboard actions, and conditional formatting. Advanced LOD expressions for aggregations like percentage distributions and filtered averages.
- **Data Visualization**: Strategic chart selection (e.g., heatmaps for performance matrices, scatters for age-salary trends) to balance detail and clarity for HR users.
- **SQL & Analytics**: Prep queries for joins (e.g., employees and departments tables) and trend computations, drawing from HR analytics practices.
- **Soft Skills**: Stakeholder-focused design—addressing HR needs like "equity gaps by gender"—plus iterative testing for intuitive navigation.

This dashboard reflects my evolution from basic queries to full BI solutions, with emphasis on ethical data handling in sensitive domains like HR.

## How to Use This Dashboard

1. **Download**: Grab the .twbx file from [GitHub Releases](https://github.com/Ritik574-coder/hr-dashboard-overview/releases).
2. **Open in Tableau**: Launch Tableau Desktop (free trial or Public edition) and load the file.
3. **Interact**:
   - Use top-right filters to slice by department, location, or education.
   - Click a pie slice (e.g., "Male") to update the employee table via actions.
   - Export sheets or dashboards as PDFs for reports.
4. **Customize**: Adjust themes, integrate live HR systems (e.g., via connectors), or expand with custom parameters.

Pro Tip: Publish to Tableau Public or Server for team sharing and scheduled refreshes.

## Roadmap & Future Enhancements

- Integrate live HRIS feeds (e.g., Workday connectors) for real-time updates.
- Add predictive elements: Forecast turnover using ML models (e.g., survival analysis in Python, blended into Tableau).
- DEI Focus: Enhanced diversity metrics with benchmark comparisons.
- Accessibility: Alt-text for all visuals and high-contrast modes.

Contributions welcome—fork the repo and submit a PR!

## About the Author

Hi, I'm **Ritik Kumar**, a dedicated data engineering student based in India. Currently bridging academia and industry, I'm passionate about turning raw data into people-centric insights. From debugging LOD expressions late into the night to exploring HR ethics in analytics, I thrive on impactful problem-solving. This dashboard is one of many in my portfolio, highlighting my growth in BI and workforce analytics.

Let's connect—I'd love to discuss HR trends, collaborate on tools, or exchange tips on data careers!

## Connect With Me

- **GitHub**: [Ritik574-coder](https://github.com/Ritik574-coder) – Fork this repo and star for updates!
- **LinkedIn**: [Ritikkumar](https://www.linkedin.com/in/ritik-kumar-b81b32375/) – Let's network on data and HR opportunities.
- **Tableau Public**: [Ritik Sky](https://public.tableau.com/app/profile/ritik.sky) – Check out my other viz experiments.
- **X (Twitter)**: [@KarlX279873](https://x.com/KarlX279873) – Quick takes on tech and trends.
- **Instagram**: [@ritik_sky1](https://www.instagram.com/ritik_sky1/?__pwa=1) – Behind-the-scenes of my learning journey.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details. Feel free to use, modify, and share—just give credit where it's due!

---

*Last Updated: December 19, 2025*  
*Built with ❤️ in India*