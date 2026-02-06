# Google Play Store Market Intelligence Dashboard (Tableau)

## Problem Statement
Understanding app market dynamics in the **Google Play Store ecosystem** is critical for developers, investors, and marketers. However, insights are often buried under unstructured data. This project addresses that by transforming a raw dataset of **10,300 apps (2010–2018)** into an interactive Tableau dashboard that reveals **category performance**, **user ratings**, **install trends**, and **pricing strategies**, enabling **data-driven product and market decisions**.

---

## Analysis Done
- Cleaned and standardized raw Google Play Store data (`googleplaystore.csv`) using Python (`Google_Play_Store_Analytics_Cleaned_Data.ipynb`).
- Processed missing values, normalized price and category fields, and converted installs/sizes into numeric units for reliable aggregation.
- Established **rating bands**: Excellent (4.5–5.0), Very Good (4.0–4.5), Good (3.0–4.0), Fair (2.0–3.0), Poor (≤2.0).
- Identified **33 app categories**, dominated by **GAME (21.5% installs)**, followed by **COMMUNICATION** and **SOCIAL**.
- Classified installation tiers: Very High (>1M), High (100K–1M), Medium (1K–100K), and Low (<1K).
- Found **92.6% apps are free** and **average rating = 4.2**, indicating a freemium-heavy market.
- Time-series analysis (2010–2018) highlighted **2017–2018** as peak years for quality and launch volume.
- Observed a positive link between installs and rating — apps with higher install counts tend to receive better ratings.

---

## Dashboard Overview
The Tableau dashboard delivers actionable intelligence through:
- **App Update Trend Over Time:** Tracks monthly updates (2010–2019), showing accelerated activity in 2018–2019.
- **Top Categories Treemap:** Highlights **FAMILY (1,939 apps)**, **GAME (1,121)**, and **TOOLS (841)** as leading segments.
- **Rating Distribution Across Categories:** Shows user satisfaction leaders — **FINANCE (4.7)** and **FAMILY (4.6)**.
- **Free vs Paid Analysis:** Visualizes dominance of **free apps (92.6%)** and high free-to-paid ratios in FAMILY and TOOLS.
- **Install vs Rating Analysis:** Displays that **35.75% of Very High install apps** are rated Excellent, compared to **5.08% in Low tier**.

**Scope:**  
Covers **10.3K apps**, **147B installs**, **33 categories**, and **8-year historical trends**, enabling users to explore performance by category, type, or rating with interactive filters.

![Tableau Dashboard](Tableu.PNG)

---

## Recommendations
- **Focus on High-Volume Categories:** Prioritize GAME, FAMILY, and TOOL apps for competitive advantage.
- **Leverage Freemium Models:** With 92.6% apps free, optimize monetization through ads or in-app purchases.
- **Enhance Quality:** Maintain high user satisfaction (≥4.0 rating) to improve install growth potential.
- **Invest in Ongoing Updates:** Frequent app updates (noted post-2017) align with higher engagement and ratings.
- **Monitor Emerging Segments:** Track underrepresented but high-rated niches like FINANCE and EDUCATION for growth.

---

**Author:** [Kshitij Saini](https://www.linkedin.com/in/kshitijsaini-b950b7299?utm_source=share_via&utm_content=profile&utm_medium=member_android)
