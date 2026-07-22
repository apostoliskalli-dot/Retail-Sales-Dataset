# ⚙️ Automated End-to-End BI Data Pipeline & Reporting System

An enterprise-grade, fully automated data pipeline that connects directly to a Google Cloud Platform (BigQuery) data warehouse, programmatically engineers messy e-commerce logs, performs statistical hypothesis testing, and dynamically compiles an interactive, production-ready Business Intelligence Report with zero manual intervention.

# 🚀 Live Automated Dashboard Demo
Instead of reviewing static code outputs, you can experience the dynamically generated executive dashboard live on your browser

👉 * [Launch Live BI Report Dashboard] (https://apostoliskalli-dot.github.io/Retail-Sales-Dataset/)*

---

# 🛠️ Project Architecture & Workflow

### 1. Data Ingestion & Warehouse Connection
* Established secure authentication and connection between Google Colab environment and **GCP BigQuery**.
* Executed structured SQL queries to fetch transactional data streams directly from warehouse datasets.

### 2. Data Engineering & Advanced Cleansing (Pandas & NumPy)
* **Text & Format Standardization:** Trimmed whitespace and unified letter-casing across categorical columns. Applied regex mutations to replace hidden empty string spaces with actual `NaN` values to enforce strict data integrity.
* **Type Casting & Coercion:** Resolved mixed formatting conflicts. Enforced valid categorical schema types and strict numerical data constraints.
* **Feature Engineering & Time-Series Grouping:** Built custom date components. Formulated an operational **bi-monthly index matrix** to accurately monitor seasonal revenue pacing across 6 equal multi-month annual cycles.

### 3. Automated Auditing & EDA
* Implemented 'fg-data-profiling' to compile an exhaustive data health blueprint (report.html), systematically identifying column sparsity, null distribution frequencies, and variance behaviors prior to visual modeling.
* **Statistical Hypothesis Testing:** Applied parametric and non-parametric statistical tests (e.g., ANOVA, Chi-Square, T-Tests) to validate data-driven assumptions, evaluate variance significance across customer segments, and confirm performance trends with statistical rigor.
---

# 📈 Core BI Metrics Formulation (KPI Cards)

The header of the report utilizes unified Plotly subplots wrapped in stylized CSS card constructs to track primary high-level financial and operational health logs:
* **Total Revenue:** Aggregated multi-year gross transactional value.
* **Average Order Value (AOV)**
* **Total Orders:** Net structural transaction volume.
* **Volume Performance:** Total units distributed.

---

# 🔬 Visual Deep-Dives Developed

* **Sales Contribution by Category:** Integrated data matrix tables side-by-side with localized multi-colored horizontal charts to track leading inventory segments.
* **Elasticity Price vs. Quantity:** Multi-variable bubble chart tracking sales velocity correlation against unit pricing, scaling bubble dimensions to display gross revenue contributions per item.
* **Temporal Distributions:** Visualizing multi-year transaction velocity through daily linear timelines outfitted with integrated custom range-slider window macro zoom panels.
* **Seasonality Breakdown:** Proportional donut charts tracking distribution weights across months and specific days of the week, exposing critical cycle spikes (Thursdays & Sundays).
* **Statistical Hypothesis Testing & Demographic Analysis:** 
  * Evaluated continuous metrics using normality checks, confirming non-normal distributions and justifying the use of non-parametric methods.
  * Executed **Kruskal-Wallis** tests to determine whether gender is a statistically significant factor influencing purchasing behavior.
  * Segmented customers into distinct age cohorts and applied the **Kruskal-Wallis H-test** to identify statistically significant variance in spending patterns across age groups without assuming normality.
---

# 🖥️ Executive Deployment & Deliverables

* Configured a custom compiler loop script in Python to translate separate, active visualization objects into an integrated, lightweight, standalone **HTML/CSS executive document**.
* Automated live continuous hosting infrastructure utilizing **GitHub Pages**, providing instantly accessible asset links for non-technical leadership and corporate stakeholders.

---

👉 **[Δείτε το Live Dashboard εδώ!] (https://apostoliskalli-dot.github.io/Retail-Sales-Dataset/)**
