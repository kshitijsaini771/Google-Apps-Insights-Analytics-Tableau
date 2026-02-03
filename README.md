# Google Play Store Market Intelligence Dashboard (Tableau)
## Overview

This interactive Tableau dashboard examines a curated dataset of 10,300 cleaned Google Play Store apps, delivering real-time analytics on key metrics such as user ratings, installation volumes, category-level performance, and emerging market trends. It equips stakeholders with actionable intelligence to guide strategic decisions in app development, feature prioritization, and marketing initiatives.

---

## Dataset

> Original Dataset - `googleplaystore.csv`

The analysis is based on a refined dataset comprising **10,300 Google Play Store applications**, derived from the original source through rigorous data cleaning—including duplicate removal and imputation of missing values. This curated dataset (`googleplaystore.csv`) was produced using the preprocessing pipeline documented in `Google_Play_Store_Analytics_Cleaned_Data.ipynb`. Key descriptive statistics reveal an **average app rating of 4.2**, with **92.6% of apps offered free of charge** and an **average of 14.2 million installs per app**. The apps span **33 distinct categories**, with **GAME** dominating at **21.51% of total installs**, closely followed by **COMMUNICATION** and **SOCIAL**, each accounting for **8.53%**. Install volumes are grouped into four tiers: **Very High** (>1M installs; 4,059 apps), **High** (100K–1M; 1,645 apps), **Medium** (1K–100K), and **Low** (<1K). User ratings are further classified into five performance bands—**Excellent** (4.5–5.0), **Very Good** (4.0–4.5), **Good** (3.0–4.0), **Fair** (2.0–3.0), and **Poor** (≤2.0)—to enable nuanced evaluation. The dataset covers apps released between **2010 and 2018**, capturing temporal trends in app launches, updates, and market evolution over nearly a decade.

---

## Analysis Outcome

  - Performed comprehensive data cleaning in a Jupyter notebook using Python, addressing missing ratings, converting app size and install counts into numeric formats, and eliminating duplicate entries.  
  - Exported the refined dataset to `googleplaystore.csv` to support seamless integration with Looker Studio, ensuring reliability and uniformity for downstream visualization.  
  - Normalized key fields—including category labels, price representations, and date formats—to facilitate precise filtering, grouping, and aggregation within the dashboard. 
  - Integrated dynamic filters for **Category** and **App Type** (Free/Paid), allowing users to explore performance metrics within specific market segments.  
  - Developed a stacked bar chart visualizing **rating distribution across install tiers**, highlighting that apps in the Very High install group have 44.19% rated as Very Good.  
  - Built a time-series view showing the **distribution of app records by rating year-over-year (2010–2018)**, which identified 2017–2018 as periods of peak activity and quality improvements.
  - The **GAME** category leads significantly in both total app volume and install share, reinforcing its strategic importance for future development investment.  
  - Apps with higher install volumes tend to receive better ratings—**35.75% of Very High install apps are rated Excellent**, compared to only **5.08% in the Low install segment**.  
  - **Free apps represent 92.6% of the ecosystem**, underscoring the prevalence of the freemium model and the need to optimize in-app monetization and user retention.  
  - Overall **rating quality has improved over time**, with apps released between 2016 and 2018 showing notably higher proportions of Good and Very Good ratings than earlier cohorts.

---

## Dashboard

- This dashboard provides a strategic overview of the Google Play Store market, analyzing **10.3K apps** with a combined **147 billion installs** across **33 categories**, and an **average rating of 4.2**.
- The **App Update Trend Over Time** line chart tracks monthly updates from 2010 to 2019, revealing spikes in activity and long-term growth patterns—particularly sharp increases in 2018–2019.
- A treemap highlights the **Top 10 Categories by App Count**, with **FAMILY (1,939 apps)** leading, followed by **GAME (1,121)** and **TOOLS (841)**, indicating dominant development focus areas.
- The **Rating Distribution Across Apps** visualization displays average ratings per category, showing that **FAMILY (4.6)** and **FINANCE (4.7)** lead in user satisfaction, while others hover around 4.2–4.4.
- The **Free vs Paid Distribution** bar chart compares app counts by pricing model across categories, illustrating that **free apps dominate** in nearly all segments—with FAMILY and TOOLS having the highest free-to-paid ratios.
- Designed for product managers, marketers, and investors to identify high-growth categories, benchmark performance, and allocate resources based on real-time market trends and user preferences.

![Tableu](Tableu.PNG)

## Author & Contact
- Name: `Kshitij Saini`   
- LinkedIn: [https://www.linkedin.com/in/kshitijsaini](https://www.linkedin.com/in/kshitij-saini-b950b7299?utm_source=share_via&utm_content=profile&utm_medium=member_android)
