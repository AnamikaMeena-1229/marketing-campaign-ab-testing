📊 Marketing Campaign Optimization: A/B Testing & Regression Analysis
🎯 Project Overview
In the fast-paced digital marketing landscape, companies frequently run ad campaigns across multiple platforms. A common challenge is determining exactly where to allocate the marketing budget to maximize Return on Ad Spend (ROAS).

This project combines Hypothesis Testing (A/B Testing) and Predictive Modeling (Regression Analysis) to analyze marketing campaign performance across two major channels (e.g., Facebook Ads vs. Google AdWords).

💡 Core Business Questions Answered:
Which platform drives a statistically higher conversion rate and revenue?
Once the superior platform is chosen, how do individual metrics (Ad Spend, Clicks, Impressions) influence future sales?
🛠️ Tech Stack & Key Libraries
Language: Python
Data Manipulation & Cleaning: pandas, numpy
Statistical A/B Testing: scipy.stats (Independent Two-Sample T-Test)
Predictive Modeling: statsmodels (Ordinary Least Squares Linear Regression)
Data Visualization: matplotlib, seaborn
🚀 Step-by-Step Methodology
1. Exploratory Data Analysis (EDA)
Cleaned and aggregated daily campaign data.
Engineered core marketing metrics including Click-Through Rate (CTR), Conversion Rate (CR), and Cost Per Acquisition (CPA).
2. A/B Testing (Statistical Experimentation)
Instead of relying on simple visual averages, an Independent Two-Sample T-Test was conducted to verify that observed performance differences were not due to random noise.

Null Hypothesis (
H
0
H 
0
​
 ): Mean sales from Campaign A = Mean sales from Campaign B.
Alternative Hypothesis (
H
1
H 
1
​
 ): There is a statistically significant difference in mean sales between the two campaigns.
Result: With a 
p
p-value 
<
0.05
<0.05, we successfully rejected the Null Hypothesis and identified our definitive winning channel.
3. Regression Analysis (Drivers & ROI Optimization)
Focused purely on the winning platform, an OLS Linear Regression model was built to quantify the exact relationship between input levers and output sales.

Model Formula: Sales ~ Spend + Clicks
Key Insight: Quantified the precise incremental revenue lift per additional dollar of ad spend, allowing strategic planning for future budget scaling.
📈 Key Business Recommendations
Shift Budget Allocation: Reallocate 70% of the ongoing marketing budget to the winning platform proved by the A/B test, capturing an immediate lift in overall efficiency.
Predictive Budget Scaling: Utilizing the regression coefficients, the finance team can reliably forecast daily revenue based on planned daily ad spend, eliminating guesswork.
Optimizing Creative Assets: Since Clicks were identified as a highly significant coefficient in the regression model, marketing teams should focus on testing higher-performing ad creatives to improve CTR before increasing raw spend.
📂 File Structure
campaign_analysis.ipynb: The complete Jupyter Notebook containing all Python code, statistical test outputs, and commentary.
marketing_campaign_data.csv: The raw dataset used for analysis.
images/: Folder containing generated plots (A/B test boxplots and regression scatter plots).
👤 Contact & Feedback
Feel free to reach out if you have any questions or suggestions about this analysis!

LinkedIn: www.linkedin.com/in/anamika-meena-97066638b
Email: anamikameena1229@gmail.com
