
# Google Play Store Market Intelligence Dashboard (Tableau)


</div>


## Overview
Interactive Tableau dashboard analyzing 10,300+ cleaned Google Play Store apps across 33 categories. Delivers real-time insights on market share, category performance, rating distributions, and download patterns to inform app development and marketing strategies.

## Dataset Overview
- **Size**: 10,300+ apps processed through Python data cleaning pipeline, exported from `google-play-store-analytics.ipynb` to `cleaned_googleplaystore.csv`.
- **Source**: Clean, structured dataset with standardized formats for installs (numeric ranges converted to averages), sizes (MB), prices, and dates for Tableau compatibility.
- **Key Metrics**: Total apps tracked, average ratings across categories, high-rated apps threshold, total downloads in millions, percentage of free apps in marketplace.
- **Categories**: Complete coverage of 33 app categories including GAME, COMMUNICATION, SOCIAL, PRODUCTIVITY, TOOLS, FAMILY, PHOTOGRAPHY, and specialized segments.
- **Install Ranges**: Segmented from 0-50 downloads up to 1 billion+ installs with average install calculations for accurate market sizing and performance benchmarking.
- **Content Ratings**: Distribution across Everyone, Teen, Mature 17+, Everyone 10+, Adults only 18+, and Unrated categories for demographic targeting insights.
- **Data Quality**: Cleaned dataset with handled nulls, standardized text fields, proper data types, and validated ranges ensuring accurate visualization and analysis.

## Analysis & Dashboard
- **Data Preparation Workflow**:  
  - Executed comprehensive data cleaning in `google-play-store-analytics.ipynb` including duplicate removal, missing value treatment, install range standardization.
  - Converted size strings to numeric MB values, extracted minimum Android versions, standardized category and content rating text fields.
  - Exported refined dataset to `cleaned_googleplaystore.csv` with proper column names and data types optimized for Tableau's data engine.
  - Connected Tableau to CSV file, created calculated fields for metrics like free app percentage, average installs per category, and high-rated app filters.

- **Dashboard Architecture**:  
  - Built comprehensive KPI panel displaying Total Apps count, Average Rating across all apps, High Rated Apps count (4+ rating), Downloads in millions, and Free Apps percentage.
  - Designed Market Share horizontal bar chart ranking categories by app count with color-coded performance indicators showing market dominance patterns.
  - Created detailed Category Distribution visualization showing percentage breakdown with GAME, COMMUNICATION, and SOCIAL as top segments.
  - Developed Reviews Performance Score scatter plot correlating review counts with ratings to identify high-engagement apps with strong satisfaction metrics.

- **Advanced Visualizations**:  
  - Implemented Size-Content Distribution stacked bar chart showing app size distribution across content ratings with count breakdowns for capacity planning.
  - Built Category Install Breakdown bar chart with total installs per category and trend indicators (Increase/Decrease arrows) for performance tracking.
  - Designed App Success Journey funnel visualization showing progression from All Apps through With Reviews, Popular (1K+), Successful (100K+), Top Tier (10M+), to Elite (100M+).
  - Added interactive filters for Category and Content Rating enabling drill-down analysis and cross-filtering across all dashboard components.

- **Interactive Features & Parameters**:  
  - Implemented Top N parameter allowing users to dynamically adjust number of categories displayed in rankings and comparisons.
  - Created category and content rating filters with cascading effects updating all visualizations simultaneously for focused analysis.
  - Added tooltip enhancements showing detailed app information, exact values, and percentage calculations on hover for comprehensive data exploration.
  - Configured dashboard actions enabling click-to-filter functionality where selecting any element filters related visualizations for interactive storytelling.

- **Key Business Insights**:  
  - Success Journey funnel reveals significant drop-offs with 94.29% apps having reviews but only 1.06% achieving Elite status, highlighting competitive market reality.
  - GAME category dominates market share with highest app count and total installs, validating gaming as primary growth opportunity for developers.
  - Reviews Performance Score correlation shows higher review counts generally correlate with better ratings, emphasizing importance of user engagement strategies.
  - Free apps constitute overwhelming majority demonstrating freemium as dominant business model requiring focus on in-app monetization and user retention.

![Tableau](Tableau.PNG)



## How to Use

- Explore interactive features:  
  - Use **Category** filter dropdown to analyze specific app categories (GAME, COMMUNICATION, TOOLS, etc.) across all visualizations
  - Apply **Content Rating** filter to focus on specific demographic segments (Everyone, Teen, Mature 17+, Everyone 10+)
  - Adjust **Top N** parameter slider to control number of categories displayed in ranking charts for focused comparison
  - Click any chart element (bar, data point, category) to filter entire dashboard and explore relationships
- Navigate dashboard components:  
  - View top KPI row for instant market overview metrics and key performance indicators
  - Analyze Market Share chart to understand category distribution and competitive landscape positioning
  - Explore Category Install Breakdown for detailed performance comparison with install volumes and growth trends
  - Review App Success Journey funnel to understand conversion rates across different success milestones
  - Examine Reviews Performance Score scatter plot to identify high-engagement opportunities
- Update with new data:  
  - Run `google-play-store-analytics.ipynb` with updated raw data source
  - Generate fresh `cleaned_googleplaystore.csv` export file
  - In Tableau, right-click data source and select "Refresh" or "Update Now" to reload data
  - Alternatively, replace CSV file and reopen workbook for automatic data refresh
  - Validate refresh by checking Total Apps count and latest update timestamp
- Export and share insights:  
  - Download dashboard as PDF or PNG image for presentations using Export menu
  - Share Tableau Public link with stakeholders for interactive web-based access
  - Create Story points to guide users through key insights and findings
  - Export filtered data tables to Excel for further analysis or reporting
- Best practices for analysis:  
  - Start with Success Journey funnel to understand overall market competitiveness and conversion rates
  - Use category filter to benchmark your app category against market standards
  - Compare Free vs Paid performance patterns by applying Type filters and analyzing metrics
  - Monitor Reviews Performance Score to identify engagement opportunities and quality benchmarks
  - Cross-reference multiple charts to validate insights and identify actionable patterns
  - Apply Top N parameter to focus on most relevant categories for your analysis scope



## Author & Contact
- Name: `Kshitij Saini`   
- LinkedIn: [https://www.linkedin.com/in/kshitijsaini](https://www.linkedin.com/in/kshitij-saini-b950b7299?utm_source=share_via&utm_content=profile&utm_medium=member_android)
