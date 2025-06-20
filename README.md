# Customer Churn Analysis
Use Power BI to monitor and analyze customer churn of a fictional telecom company called Databel
## :one: Project Overview:
- This project analyzes a telecom customer dataset to understand why customers stop using services (churn).
- The main goal is to identify customer characteristics, behaviors, and contract details linked to high churn rates and provide actionable insights for creating effective customer retention strategies.
## :two: Dataset Description:
- **Source:** Datacamp
- **Time period:** Not given
- **Company:** Databel (a fictional telecom company)
- **Key fields:** Churn Reason, Churn Category, Age, Contract Type, Payment Method, Monthly Charges, Data Unlimited Plan, Intl Plan
- **Data dictionary:** [attached file](https://github.com/NguyenPhuongNghi/Customer-Churn-Analysis/blob/main/data%20dictionary%20(customer%20churn%20analysis).pdf)
## :three: Tool used:
- Power BI (Power Query, DAX measures, Visuals)
## :four: Key features:
- Churn rates = Number of Churned Customer / Total Number of Customer
## :five: Dashboard: [attached file](https://github.com/NguyenPhuongNghi/Customer-Churn-Analysis/blob/main/Customer%20Churn%20Analysis.pbix)
### :pushpin: Page 1: Overview
![alt](https://github.com/NguyenPhuongNghi/Customer-Churn-Analysis/blob/main/photo/Screenshot%202025-05-28%20151950.png?raw=true)
#### By Age Group:
- The largest customer segments appear to be in the Young to Mid Adults (25-44) and Middle-Aged Adults (45-64).
- The churn rates show a generally increasing trend with age, particularly noticeable in the 65+ age group. This suggests that older customers might be more likely to churn.
#### By Payment Method:
- Direct Debit has the highest number of customers (55.36%), followed by Credit Card (39.09%) and then Paper Check (5.55%).
#### By State:
- West Virginia (WV) has the highest number of customers among all states, with 213 customers.
- The differences between most other states are not very large. Aside from WV, the customer numbers across states mostly range between 168 and 68, indicating a fairly even distribution.
#### By Number of Customer in Group:
- The average monthly charge of individual customers (group size 0) is, on average, approximately 1.5 times as high as that of group customers
- The churn rates for individual customers are, on average, 5 times as high as that for group customers. This suggests that customers in larger groups are less likely to churn due to lower charges, highlighting the effectiveness of group contracts for retention.
#### By Contract Category and Account Length:
- The percentage of customers with Monthly Contracts (51.01%) is relatively equal to that of Yearly Contracts (48.99%)
- Customers with Monthly Contracts had higher average churn rates (46.3%) than those with Yearly Contracts (6.6%). This suggests that longer contracts may lead to greater customer retention. 
- The churn rate for Monthly contracts is significantly higher and more volatile throughout the customer lifecycle. It generally decreases over the account length but with considerable fluctuations.
- The churn rate for Yearly contracts is consistently much lower than monthly contracts and shows a more stable, generally decreasing trend over the account length. This reinforces the idea that longer-term contracts lead to better customer retention.
### :pushpin: Page 2: Analyze Churn rates by Charges:
![alt](https://github.com/NguyenPhuongNghi/Customer-Churn-Analysis/blob/main/photo/Screenshot%202025-05-28%20174007.png?raw=true)
- **Brief Explanation:** Customers without an unlimited data plan have to pay extra data charges. Customer without International Plan have to pay extra charges for international calls.
#### By Unlimited Data Plan (UDP) And Download Volume:
- 67.21% total customers use UDP
- For those consuming "Less than 5 GB": the churn rate for those with UDP (34.7%) is almost 3 times as high as that for those without UDP (12.3%). This might be because the average monthly charge for those with UDP ($37.7) is almost 3 times higher than that for those without UDP ($13.9) and users think that the avg monthly charge is too high for their low demands
- For those consuming "Between 5 and 10 GB" and "More than 10 GB": the churn rates for those with and without UDP are relatively the same. This might be because the avg monthly charges for those with and without UDP are relatively equal.
#### By International Plan (IP) And Download Volume:
- 9.74% total customers use IP
- For those making less than 50 calls: the churn rate for those with IP (48.3%) is approximately 1.7 times as high as that for those without IP (27.2%). This might be because the average monthly charges for those with and without IP are relatively the same and they don't need IP for such low demands
- For those making more than 50 calls: the churn rate for those with IP is significantly lower than that for those without IP and generally decreasing over calls volume. This might be cause their demands are higher and they use IP to save expenses and get preferential prices.
### :pushpin: Page 3: Analyze Churn rates by Churn Category and Reason
![alt](https://github.com/NguyenPhuongNghi/Customer-Churn-Analysis/blob/main/photo/Screenshot%202025-05-28%20152442.png?raw=true)
#### By Churn Reasons/Categories:
- The top reasons for churn are related to competitor offerings, with "Competitor made better offers" (4.5%) and "Competitor had better devices" (4.4%) being the leading causes.
- "Attitude of support person & service provider" (4.3%) is also a significant factor, highlighting the importance of customer service<br>
- Regarding Unlimited Data Plan and International Plan, the most popular churn category for both plans is competitor, followed by attitude of support person & service provider and dissatisfaction with product and service.
### :pushpin: Page 4: Analyze Churn rates by Customer Service:
![alt](https://github.com/NguyenPhuongNghi/Customer-Churn-Analysis/blob/main/photo/Screenshot%202025-05-28%20162114.png?raw=true)
#### Average Customer Service Calls and Churn Rate by State:
- California (CA) has the highest churn rate of 63.2%, followed by Ohio (34.8%) and Pennsylvania (33.3%) . California has a relatively low average customer calls compared to its high churn, suggesting that when customers in California decide to leave, they might not even bother contacting customer service. 
- Churned Customers have a higher average number of customer service calls (2.4 calls) than those who didn't churn (0.4 calls). This suggests that customers reaching out to customer support more frequently might be experiencing issues that eventually lead to them leaving. This hightlight the needs to improve customer service
## :six: Insights:
### :round_pushpin: 1. Customer Service:
- **Target Engagement for Older Customers:** Develop tailored communication or support to help them with technical difficulties or different needs, etc because % total churned customer aged 65 and above is considerable (38.5%)
- **Customer Service Training & Improvement:** Invest in comprehensive training for support staff focusing on empathy, problem-solving, and positive communication. Implement quality assurance measures and feedback mechanisms.
- **Improve First Call Resolution:** Focus on resolving customer issues effectively on the first contact to reduce the need for repeated calls and potential frustration.
- **Analyze Customer Service Interactions:** Identify common issues and pain points raised by customers contacting support and address them proactively. Provide sufficient training for all customer service staff. 
### :round_pushpin: 2. Pricing strategies:
- **Competitor Analysis & Offer Improvement:** Conduct competitor analysis to understand their strengths and offers. Develop more attractive pricing, bundles, and device options to compete effectively.
- **Incentivize Longer-Term Contracts:** Offer discounts, exclusive features, or other benefits to encourage customers to commit to one or two-year contracts.
- **Promote Group Contracts:** Actively market group plans and their advantages to increase adoption.
- **Promote Unlimited Plans:** Actively market the benefits of unlimited data and international plans to customers who have high demands for download volume and making international calls.
- **Offer Flexible Plan Options:** Consider offering tiered plans or add-ons that better suit different usage patterns categorized by consumption level, reducing the likelihood of unexpected overages.
- **Review Overage Pricing:** Evaluate the pricing structure for extra data and international calls to ensure it is fair and doesn't lead to significant customer dissatisfaction.




