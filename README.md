# Awesome-Sales-Marketing-Reporting

## Top Sales & Marketing Reporting Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Cross-Channel Attribution, KPI Dashboards & Self-Hosted Marketing Analytics*  

**Last updated: November 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Sales & Marketing Reporting**. These tools enable revenue teams to unify data from CRM, advertising, email, and web analytics into a single view—measuring pipeline velocity, campaign ROI, and customer acquisition costs without drowning in disconnected spreadsheets.



**Examples** include HubSpot Performance Reporting, Tableau, Power BI, Databox, Klipfolio, Looker, Domo, Geckoboard, AgencyAnalytics, and Supermetrics (the category leaders).



**Open-source emphasis**: Sales & Marketing Reporting is a domain where open-source tooling is **fragmented across the pipeline but genuinely viable when assembled thoughtfully**. The strongest active projects are **Multiwoven** (an open-source Reverse ETL platform that syncs warehouse data to Salesforce, HubSpot, and ad platforms—the data activation layer that makes reporting possible) , **dashbordina** (a complete marketing analytics stack with PostgreSQL, Airflow ETL, FastAPI, and Plotly Dash, measuring CAC, CLV, and ROAS) , and **KPI-Insight-Companion** (a GPT-powered SaaS KPI dashboard for natural-language querying of CAC, LTV, MRR, and churn) . For Superset-based strategic dashboards, **superset-supremacy** provides a Docker-ready prototype with channel ROI, budget analysis, and funnel visualization . The critical caveat: **no open-source project matches Databox or AgencyAnalytics for turnkey multi-client reporting**—those platforms bundle 100+ pre-built connectors and white-label dashboards that open-source requires assembly to replicate.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-products)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[HubSpot Performance Reporting](https://www.hubspot.com/)**  

  Native reporting within HubSpot's Marketing and Sales Hubs; dashboards for campaign ROI, deal pipeline, email performance, and attribution tied directly to CRM records.



- **[Tableau](https://www.tableau.com/)**  

  Enterprise visual analytics platform; widely used for marketing dashboards when connected to a data warehouse or CRM exports, with deep interactivity and governed data sources.



- **[Power BI](https://powerbi.microsoft.com/)**  

  Microsoft's BI platform; common for sales and marketing reporting in Microsoft-centric organizations, with DAX for custom metrics and Power Query for data transformation.



- **[Databox](https://databox.com/)**  

  Dashboard platform with 100+ pre-built integrations for marketing and sales tools; focused on goal tracking, alerts, and client-facing reporting for agencies.



- **[Klipfolio](https://www.klipfolio.com/)**  

  BI and dashboard platform with a library of pre-built metrics; positioned for marketing teams wanting customizable KPI dashboards without a data warehouse.



- **[Looker](https://looker.com/)**  

  Google Cloud BI platform built on LookML for governed metric definitions; strongest when standardized on BigQuery for unified sales and marketing data models.



- **[Domo](https://www.domo.com/)**  

  Cloud BI platform with a broad connector library and business-user-friendly dashboard creation; positioned for operational and executive reporting.



- **[Geckoboard](https://www.geckoboard.com/)**  

  Dashboard platform focused on real-time KPI visibility for teams; popular for sales floor TVs and marketing performance snapshots.



- **[AgencyAnalytics](https://agencyanalytics.com/)**  

  Reporting platform built for marketing agencies; multi-client dashboards, white-labeling, and 80+ integrations for SEO, PPC, social, and call tracking.



- **[Supermetrics](https://supermetrics.com/)**  

  Data connector platform that pulls marketing data (Google Ads, Facebook, HubSpot, etc.) into Google Sheets, Excel, Looker Studio, or a data warehouse—the pipeline layer for custom reporting.



## Open-Source GitHub Projects



### Reverse ETL & Data Activation (Reporting Pipeline)



- **[Multiwoven](https://github.com/Multiwoven/multiwoven)**  

  Open-source **Reverse ETL and data activation platform** (AGPLv3), positioned as an alternative to Hightouch, Census, and RudderStack . Syncs data **from your warehouse** (Snowflake, BigQuery, Redshift, Databricks, PostgreSQL) **to business tools** (Salesforce, HubSpot, Klaviyo, Google Ads, Facebook Ads, Slack) . This is the pipeline layer that makes unified sales and marketing reporting possible—keeping CRM and ad platforms enriched with warehouse-derived metrics . Docker Compose, Helm, and cloud deployment guides available. **Best for teams needing to operationalize reporting data** by pushing computed metrics back into the tools where sales and marketing teams work—but it is infrastructure, not a dashboard itself.



### Complete Marketing Analytics Stacks



- **[dashbordina](https://github.com/avrtt/dashbordina)**  

  Open-source **marketing analytics dashboard** for audience segmentation and multi-channel ROI analysis . Features: **CAC, CLV, ROAS, and segment-specific analytics**; PostgreSQL data warehouse with raw/archive/analytics schemas; **Apache Airflow ETL** with hourly and daily DAGs; FastAPI backend exposing metrics via REST; **Plotly Dash dark-themed UI** with drill-down; Docker Compose deployment; GitHub Actions CI/CD for AWS ECS/EKS . **Best for teams wanting a complete, self-hosted marketing analytics stack** with real ETL and API layers—but it is a prototype architecture requiring data pipeline customization for your sources.



- **[superset-supremacy](https://github.com/avrtt/superset-supremacy)**  

  Open-source **Apache Superset dashboard prototype** for strategic marketing decisions . Features: **channel prioritization, budget allocation, and ROI forecasting**; strategic KPIs (ROI, ROAS, CAC, CLV); **marketing funnel visualization** with conversion rates by channel; **budget vs actual** comparison with utilization metrics; **ROI forecasting** accuracy tracking; interactive filters and dark mode; direct PostgreSQL connection with materialized views for performance . Quick demo mode (`./quick-demo.sh`) spins up a fully configured Superset environment with sample data . **Best for teams wanting a Superset-based marketing dashboard** with strategic decision-making focus—but it is a prototype replica of a portfolio project, requiring adaptation for production data sources.



### KPI Dashboards & AI-Assisted Reporting



- **[KPI-Insight-Companion-for-SaaS](https://github.com/femi-oloye/KPI-Insight-Companion-for-SaaS)**  

  Open-source **AI-powered SaaS KPI dashboard** (Python, Streamlit, GPT via OpenRouter, Plotly) . Tracks **CAC, LTV, Churn Rate, MRR, ARR, and Conversion Rate**; visualizes revenue, customer growth, and email performance; features **GPT-powered insight summarizer** (automatic natural language summaries), **KPI Q&A** ("Why did CAC spike last month?"), and **smart alerts** for abnormal churn or CAC spikes with suggested fixes . **Best for SaaS teams wanting an AI-augmented KPI dashboard** with natural language querying—but it is a Streamlit prototype, not a production BI platform.



### E-commerce & Sales Operations Dashboards



- **[OverSeek](https://github.com/MerlinStacks/overseek)**  

  Open-source **eCommerce operations dashboard for WooCommerce** (self-hosted, privacy-first) . Features: **analytics module** with revenue, attribution, cohorts, CLV, reports, live acquisition views, and conversion API health checks; **custom dashboard** with drag-and-drop widgets for revenue, live visitors, SEO keywords, and ads; **growth module** with paid ads, reviews, SEO content tools, and product feeds . Docker Compose deployment. **Best for WooCommerce merchants** wanting unified reporting across sales, marketing, and operations—but it is WooCommerce-specific and requires syncing your store data into its PostgreSQL backend .



- **[MakerMetrics](https://hub.docker.com/r/buttermygit/makermetrics)**  

  Open-source **offline sales analytics dashboard for Etsy shops** . Drop in Etsy CSV exports for a live, filterable view of orders, top products, buyers, geographic sales, forecasts, and more—running locally or in Docker . Features: KPI cards (orders, units, net revenue, AOV, repeat buyers), sales over time, US choropleth map, **sales projection with historical training range**, buyer analysis (VIP/Returning/New tiers), coupon effectiveness, and fulfillment speed . **Best for Etsy sellers** wanting private, offline sales reporting—but it is Etsy-specific and CSV-driven, not a general marketing analytics platform .



- **[SalesIQ](https://github.com/badrr06/SalesIq)**  

  Open-source **sales management and forecasting system** (Flask, Chart.js) . Features: CRUD for products, customers, and sales; dashboard with KPIs, **monthly sales + 6-month forecast** (ARIMA or Linear Regression), top products, and CSV export . MySQL or SQLite via SQLAlchemy. **Best for small businesses** wanting lightweight sales tracking and forecasting—but it is sales-only, without marketing channel or campaign analytics .



### Additional Strong Open-Source Options



- **luemartinez-dashboard** — Open-source influencer marketing dashboard (Flask, Tailwind, SVG charts) with KPI cards, sales funnel, platform performance, product performance, and monthly sales trend . **Niche**—for influencer campaign reporting, but demonstrates the pattern for marketing channel dashboards .

- **crm-dashboard** — Open-source CRM dashboard backend extracting data from Kommo (Portuguese) . **Niche/regional**—for teams using Kommo CRM wanting custom dashboards, but requires manual pipeline configuration .



**Frameworks for building custom systems**: For **data activation and warehouse-to-CRM syncing**, Multiwoven provides the Reverse ETL layer . For a **complete marketing analytics stack with ETL**, dashbordina offers PostgreSQL + Airflow + FastAPI + Dash . For **Superset-based strategic dashboards**, superset-supremacy provides channel ROI and budget analysis . For **AI-assisted KPI querying**, KPI-Insight-Companion . For **WooCommerce operations reporting**, OverSeek . No open-source project matches Databox or AgencyAnalytics for **turnkey multi-client reporting with 100+ pre-built connectors**—those require commercial platforms or significant integration work.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Sales and marketing reporting platforms handling customer and revenue data must comply with applicable privacy regulations (GDPR, CCPA) and data security policies; **self-hosted solutions place full responsibility for data pipeline reliability, metric accuracy, and access controls on the operator**.

- **Open-source sales and marketing reporting is fragmented but viable when assembled**—Multiwoven provides the Reverse ETL layer , dashbordina and superset-supremacy provide complete analytics stacks , and KPI-Insight-Companion provides AI-assisted KPI querying . However, **no open-source project matches Databox or AgencyAnalytics for turnkey multi-client reporting with pre-built connectors**—organizations requiring that depth should evaluate commercial platforms or invest in custom integration.

- Verify license terms for commercial use; Multiwoven uses AGPLv3 , dashbordina and superset-supremacy are open-source prototypes (check repositories), and KPI-Insight-Companion is open-source .



---



**Made for marketing operations leaders, sales analysts, and revenue teams building reporting infrastructure.**  

Let's make sales and marketing reporting more open, but with clear eyes about the connector ecosystem and turnkey reporting gaps that commercial platforms still fill.
