# Health Data Analytics Case Study
This case study explores user behavior and asset performance using a simulated dataset from a healthcare company. The goal was to analyze a dataset of 200K+ entries related to web user behavior and asset performance to identify opportunities to optimize content strategies and improve overall conversion rates. My analysis was conducted in **Jupyter Notebook**, with visualizations built in **Tableau** and **Excel**.

## Key Insights for the healthcare media page:


- **Top Performing Asset:** Asset A achieved the highest impressions (55,000 impressions), indicating strong user interest.
- **Popular Content Category:** "Nausea and Vomiting" (36,475 views), which also converted to the highest sales
- **Trending Topic:** "Gastrointestinal Bleeding" (9,165 views) was the most discussed topic, suggesting a focus area for content development.
- **Optimal Engagement Time:** Hour 5 (4,283 visits) saw the highest visits, providing a key time window for targeted campaigns.


## Methodology
### Data Cleaning & EDA
The dataset was first cleaned and processed to handle missing values and ensure consistency. I then performed exploratory data analysis to understand basic trends in user behavior, content engagement, and conversion outcomes.

Key initial findings included:

Asset A had the highest number of impressions (~55,000).

Page Category most frequently viewed: Nausea and Vomiting (~36,000 views).

Page Topic Description most common: Gastrointestinal Bleeding (~9,000 views).

Peak Hour for Page Visits: Hour 5 (between 5–6 AM), with ~4,283 sessions.

### Modeling Conversion Drivers
I developed a feature importance model to identify the most influential factors driving conversion rates using a classification algorithm. The results were:

Top 3 Most Influential Variables:

- Page Category (17.8%): Especially strong influence from inflammatory bowel disease topics like Crohn's Disease and Ulcerative Colitis.

- Return Visitor Status (17.3%): Returning users showed significantly higher conversion rates.

- Time Spent on Page (15.5%): Users who converted spent on average 72.8 seconds on the page vs. 56.9 seconds for those who didn’t.



Less Influential Variables:

- Device Type (0.3%)

- Time of Day (~2.5%)

- Page Topic Description (near-zero importance despite content variability)

## Recommendations

### For Page Content:

#### Targeted User-Asset Matching:

- For users with Crohn’s Disease using mobile devices, Asset A had a conversion rate of 44.19%.

- For the same condition, Asset B had a similar conversion rate (~44.04%) but fewer impressions — indicating a possible trade-off between revenue potential and reach.

- The combination Asset A + Ulcerative Colitis Diagnosis + Crohn’s Disease Page yielded a 69.23% conversion rate, though infrequent in the dataset.

#### Default Strategy:

In cases where no highly-matched segments exist, prioritize Asset C due to its overall superior performance and consistency across categories and user types.

### Focus Areas for Future Development:
- Develop content for high-performing categories: Inflammatory Bowel Disease (IBD), Crohn's Disease, Ulcerative Colitis

- Boost Return Visitor Rates: First-time visitors have significantly lower conversion; strategies such as personalized follow-ups, email capture, or retargeting could improve return rates.

- Reassess Asset B: Asset B underperforms, potentially due to cost-related factors. A redesign or repositioning may improve ROI.

- Create Tailored Content: Focus on users with known diagnoses and deliver customized content to improve relevance and conversion.