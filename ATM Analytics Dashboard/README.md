# ATM Transactions Analysis Dashboard

![ATM Dashboard Home](https://github.com/Ritik574-coder/Bi-Project-/blob/main/ATM%20Analytics%20Dashboard/Assets/image/Home%20Section%20Pictire.png)

## Power BI Dashboard Drill
![ATM Dashboard Drill](https://github.com/Ritik574-coder/Bi-Project-/blob/main/ATM%20Analytics%20Dashboard/Assets/image/Info%20Section%20Picture.png)

---

![ATM Dashboard Drill](https://github.com/Ritik574-coder/Bi-Project-/blob/main/ATM%20Analytics%20Dashboard/Assets/image/Overview%20Section%20Picture.png)

---

![ATM Dashboard Drill](https://github.com/Ritik574-coder/Bi-Project-/blob/main/ATM%20Analytics%20Dashboard/Assets/image/Datils%20Section%20Picture.png)

---

![ATM Dashboard Drill](https://github.com/Ritik574-coder/Bi-Project-/blob/main/ATM%20Analytics%20Dashboard/Assets/image/Datils%20Section%202%20Picture.png)

---

## Introduction

Welcome to the **ATM Transactions Analysis Dashboard**, a dynamic Power BI tool built to supercharge banking operations and financial insights. As a data engineering student from India, Ritik Kumar here—your guide through this project that's become my personal favorite so far! Drawing from real-world banking data, this dashboard unpacks ATM performance, revenue streams, and cost efficiencies to help teams spot winners, fix bottlenecks, and drive smarter decisions in the fast-paced world of financial services.

In an era where every transaction counts, understanding metrics like monthly revenue, gross profit margins, and state-wise ATM health can transform operations. Sourced from anonymized banking datasets (think transaction logs from core systems), this viz covers over 2,790 ATMs across India, revealing trends from 2024—like surging revenues in Jammu & Kashmir (₹146M total) and seasonal dips in maintenance costs. Whether you're an ops analyst hunting low-performers or a regional exec eyeing profitability, dive in to:

- **Revenue & Profit Trends**: Track total ATM revenue (₹296M) and avg monthly gross profit (₹31K).
- **Geographic Hotspots**: Heatmaps showing high-revenue states like Assam and Punjab.
- **ATM Spotlights**: Drill into types (Regular: 80%, Captive: 20%) and ID-specific performance.

Crafted with Power BI's slick visuals and DAX wizardry during late-night coding sessions, this isn't just charts—it's interactive storytelling. Filter by month, state, or ATM type; drill through to transaction counts; or export for boardroom briefs. As my best dashboard yet, it blends my ETL roots with BI flair, proving data can make banking feel less like a vault and more like a vault of opportunities.

**Why this matters**: With India's ATM network booming (27K+ machines analyzed), optimizing for 60%+ gross profits means real ROI. Use this to benchmark, predict, and propel—because in finance, every rupee tells a story.

To give you a full visual tour right here in the intro, check out all the key screenshots below—straight from the dashboard. These capture the essence: from the welcoming home to deep-dive details. (Pro tip: In GitHub, they'll render live; download the .pbix for interactivity!)

### Screenshot Gallery: A Quick Dashboard Walkthrough

| Image | Description | Visual |
|-------|-------------|--------|
| **Home Page** | The landing screen with ATM illustration, navigation tabs (Home/Overview/Detail), and quick social links—sets a professional, engaging tone. | ![ATM Dashboard Home](https://github.com/Ritik574-coder/Bi-Project-/blob/main/ATM%20Analytics%20Dashboard/Assets/image/Home%20Section%20Pictire.png) |
| **Overview** | Core metrics at a glance: Cost analysis donuts (CRA/AMC breakdowns), revenue bars by state/month, and KPI cards (e.g., ₹296M total revenue, 92% uptime). Perfect for high-level scans. | ![ATM Dashboard Overview](https://github.com/Ritik574-coder/Bi-Project-/blob/main/ATM%20Analytics%20Dashboard/Assets/image/Overview%20Section%20Picture.png) |
| **Performance & Profitability** | Trends in action: Line charts for monthly profits, bar comparisons of state revenues (J&K leading at ₹146M), an interactive India map with geo-clusters, and pie for ATM types (Regular vs. Captive/TE). | ![ATM Dashboard Performance](https://github.com/Ritik574-coder/Bi-Project-/blob/main/ATM%20Analytics%20Dashboard/Assets/image/Datils%20Section%202%20Picture.png) |
| **Details** | Drill-down power: Range analysis buckets for margins (e.g., 10-50% txn counts), financial performance matrix (avg 5,457 txns), and gauges for gross profit (60%). Ideal for ATM-specific troubleshooting. | ![ATM Dashboard Detail](https://github.com/Ritik574-coder/Bi-Project-/blob/main/ATM%20Analytics%20Dashboard/Assets/image/Datils%20Section%20Picture.png) |
| **Information Page** | Behind-the-scenes: Objectives (performance/revenue analysis), target users (ops analysts to execs), dashboard structure, and author credits. Keeps it contextual and user-focused. | ![ATM Dashboard Info](https://github.com/Ritik574-coder/Bi-Project-/blob/main/ATM%20Analytics%20Dashboard/Assets/image/Info%20Section%20Picture.png) |

These visuals showcase the blue-themed, responsive design—built for desktops and mobiles alike. Hover for tooltips, click for drills!

## Project Structure

Your repo is organized for easy navigation, collaboration, and scalability. Here's the full folder breakdown—clean, modular, and ready for version control:

```
ATM-Transaction-Dashboard/
│
├── README.md
│
├── PowerBI/
│ ├── ATM_Transaction_Dashboard.pbix
│ └── ATM_Transaction_Dashboard.pbit (optional – template)
│
├── Data/
│ ├── Raw/
│ │ └── atm_transactions_raw.csv
│ │
│ ├── Cleaned/
│ │ └── atm_transactions_cleaned.csv
│ │
│ └── Metadata/
│     └── data_dictionary.md
│
├── Assets/
│ ├── Icons/
│ ├── Images/
│ ├── Backgrounds/
│ └── Logos/
│
├── Layouts/
│ ├── dashboard_wireframe.png
│ └── dashboard_mockup.fig (Figma file if any)
│
├── DAX/
│ ├── Measures.md
│ └── Calculated_Columns.md
│
├── PowerQuery/
│ └── M_Scripts.md
│
├── Documentation/
│ ├── Data_Model.png
│ ├── ETL_Flow.png
│ └── Dashboard_Screenshots/
│     ├── overview.png
│     ├── financial_performance.png
│     └── atm_usage_analysis.png
│
└── Version_History/
    └── changelog.md
```

This setup keeps raw data separate from polished assets, docs in one spot for quick refs, and code (DAX/M queries) documented for handoffs. Pro move—love the metadata and changelog for audit trails!

## Key Features

This dashboard packs interactivity and clarity into every pixel. Here's the spotlight:

- **Overview Cards**: Snap stats like total ATM revenue (₹296M), avg monthly txn (₹5K), and uptime (92%) for at-a-glance wins.
- **Trend Analysis**: Line charts for monthly revenue vs. cost (e.g., Aug peaks at ₹200M+), highlighting Q4 surges.
- **Cost & Revenue Visuals**:
  - Donut charts for CRA/AMC breakdowns (14% CRA sum) and Fin/Non-Fin txns.
  - Bar graphs comparing state revenues (J&K leads) and monthly txns/gross profits.
- **Performance Breakdown**: Horizontal bars for ATM count by state (Assam tops) and pie for cost by type (Regular ATMs at 80%).
- **India Map**: Geo-heatmap of total revenue by state—dense clusters in the Northeast.
- **Drill-Through Pages**: Click an ATM ID for deep dives, including:
  - Gauges for gross profit % (60%) and financial performance matrices.
  - Scatter plots for txn vs. revenue (e.g., 668 avg monthly txns).
  - Range analysis: Current vs. previous month margins (10-50% buckets).

Responsive design, slicers for dates/states/types, and tooltips make it mobile-ready and user-proof.

## Screenshots

(Now condensed since the intro has the full gallery— these are for reference if you scroll down!)

| Section | Description | Screenshot |
|---------|-------------|------------|
| **Home** | Welcoming overview with ATM illustration and nav. | ![Home](https://github.com/Ritik574-coder/Bi-Project-/blob/main/ATM%20Analytics%20Dashboard/Assets/image/Home%20Section%20Pictire.png) |
| **Overview** | Cost/revenue trends and KPIs. | ![Overview](https://github.com/Ritik574-coder/Bi-Project-/blob/main/ATM%20Analytics%20Dashboard/Assets/image/Overview%20Section%20Picture.png) |
| **Performance** | Maps and profit lines. | ![Performance](https://github.com/Ritik574-coder/Bi-Project-/blob/main/ATM%20Analytics%20Dashboard/Assets/image/Datils%20Section%202%20Picture.png) |
| **Details** | ATM-specific analytics. | ![Details](https://github.com/Ritik574-coder/Bi-Project-/blob/main/ATM%20Analytics%20Dashboard/Assets/image/Datils%20Section%20Picture.png) |
| **Info** | Objectives and structure. | ![Info](https://github.com/Ritik574-coder/Bi-Project-/blob/main/ATM%20Analytics%20Dashboard/Assets/image/Info%20Section%20Picture.png) |

*Note: Static captures here. Full interactivity? Download .pbix from [Releases](https://github.com/Ritik574-coder/Bi-Project-/tree/main/ATM%20Analytics%20Dashboard) or publish to Power BI Service for live viewing (requires free account—access via app.powerbi.com).*

## Data Sources & Methodology

- **Primary Dataset**: Anonymized ATM transaction logs from banking cores (e.g., Finacle-inspired aggregates via public/open datasets on Kaggle).
- **Key Columns Analyzed**: ATM ID, monthly revenue/txn, cost (CRA/AMC/UPS/VST), state (for mapping), date, type (Regular/Captive/TE), uptime %, gross profit.
- **Tools Used**:
  - **ETL**: Python (Pandas, NumPy) for cleaning (e.g., imputing missing txns, aggregating states) and export to CSV.
  - **Visualization**: Power BI with DAX measures like `Avg Monthly Revenue = AVERAGE(Revenue[Monthly])`, `Gross Profit % = DIVIDE([Total Revenue] - [Total Cost], [Total Revenue])`.
  - **Mapping**: Bing Maps integration for state-level geo-viz.
- **Assumptions**: All in INR; 2024 data quarterly refreshed. No sensitive PII—privacy first.

Replicate it: Load CSV into Power BI, apply DAX, hook up maps, and voila. Check `Data/Metadata/data_dictionary.md` for column deets!

## Skills Showcased

This project—my crowning achievement so far—spotlights the full-stack data skills I've leveled up through grit and GitHub:

- **Data Engineering**: Robust ETL in Python—handling messy txn data (e.g., outlier costs via z-score filtering) and scaling for 27K+ rows.
- **Business Intelligence**: Power BI mastery with drill-throughs, conditional formatting, and dynamic slicers. DAX deep dives for % calcs and matrices.
- **Data Visualization**: Strategic charts (e.g., geo-maps for regional insights, matrices for perf buckets) that balance density and digestibility.
- **SQL & Analytics**: Prep queries (e.g., GROUP BY state on revenue tables) and trend forecasting nods from my SQL bootcamp days.
- **Soft Skills**: Stakeholder focus—tackling "How do we cut maintenance 20%?"—plus end-to-end ownership from data ingest to dashboard polish.

From debugging geo-joins to palette tweaks for that pro blue theme, this dashboard marks my evolution into a BI powerhouse. Dive into `DAX/` and `PowerQuery/` for the code guts.

## How to Use This Dashboard

1. **Download**: Hit [GitHub Releases](https://github.com/Ritik574-coder/Bi-Project-/tree/main/ATM%20Analytics%20Dashboard) for the .pbix.
2. **Open in Power BI**: Fire up Power BI Desktop (free from Microsoft) and import.
3. **Interact**:
   - Slicers (top) for months, states, or ATM types.
   - Click a state bar to drill into performance.
   - Export to PDF or embed in PowerPoint.
4. **Customize**: Swap themes, plug in live SQL feeds, or add alerts for low uptime. See `Layouts/` for wireframes to inspire tweaks.

Pro Tip: Publish to Power BI Service for sharing—access via app.powerbi.com on any device. ETL flow in `Documentation/ETL_Flow.png`.

## Roadmap & Future Enhancements

- Real-time feeds from banking APIs for live txn monitoring.
- Predictive ML: Forecast 2026 revenue dips using ARIMA in Python.
- Multi-currency: USD/INR toggles for global ops.
- AI Insights: Natural language Q&A via Power BI Copilot.

| Feature | Status | ETA |
|---------|--------|-----|
| Real-time APIs | Planned | Q1 2026 |
| ML Forecasts | In Progress | Q2 2026 |
| Multi-currency | Planned | Q3 2026 |
| AI Q&A | Planned | Q4 2026 |

Fork and PR your ideas—let's build together! Track changes in `Version_History/changelog.md`.

## About the Author

Hey, **Ritik Kumar** here, data engineering student from India with a knack for turning transaction chaos into crystal-clear insights. This ATM dashboard? My best work yet—born from a passion for finance data and endless coffee-fueled iterations. When not viz-ing, I'm jamming to playlists or plotting my next career hack. It's all about that blend of tech and impact in my portfolio.

Connect? I'm all in for chats on BI trends, banking analytics, or collab vibes!

## Connect With Me

I'm always up for chatting about data, AI, or business ideas. Reach out!

<div align="center">
  <a href="https://www.linkedin.com/in/ritik-kumar-b81b32375/">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin" alt="LinkedIn" />
  </a>
  <a href="https://public.tableau.com/app/profile/ritik.sky">
    <img src="https://img.shields.io/badge/Tableau-Public%20Vizzes-orange?style=for-the-badge&logo=tableau" alt="Tableau" />
  </a>
  <a href="https://x.com/KarlX279873">
    <img src="https://img.shields.io/badge/X-Tweets-black?style=for-the-badge&logo=x-twitter" alt="X" />
  </a>
  <a href="https://www.instagram.com/ritik_sky1/?__pwa=1">
    <img src="https://img.shields.io/badge/Instagram-Stories-purple?style=for-the-badge&logo=instagram" alt="Instagram" />
  </a>
  <a href="https://github.com/Ritik574-coder">
    <img src="https://img.shields.io/badge/GitHub-Profile-green?style=for-the-badge&logo=github" alt="GitHub" />
  </a>
</div>

<div align="center">
  <img src="https://komarev.com/ghpvc/?username=Ritik574-coder&style=flat-square&color=blue" alt="Profile Views" />
</div>

---

## License

MIT License—see [LICENSE](https://github.com/Ritik574-coder/Bi-Project-/edit/main/LICENSE) for deets. Remix, share, just shoutout the source!

---

*Last Updated: January 01, 2026*  
*Built with ❤️ in India*
