# Customer Churn Analysis
Use Power BI to monitor and analyze customer churn of a fictional telecom company called Databel
## 1. Project Overview:
- This project analyzes a telecom customer dataset to understand why customers stop using services (churn).
- The main goal is to identify customer characteristics, behaviors, and contract details linked to high churn rates and provide actionable insights for creating effective customer retention strategies.
## 2. Dataset Description:
- **Source:** Datacamp
- **Time period:** Not given
- **Company:** Databel (a fictional telecom company)
- **Key fields:** Churn Reason, Churn Category, Age, Contract Type, Payment Method, Monthly Charges, Data Unlimited Plan, Intl Plan
- **Data dictionary:** [attached file](https://github.com/NguyenPhuongNghi/Customer-Churn-Analysis/blob/main/data%20dictionary%20(customer%20churn%20analysis).pdf)
## 3. Tool used:
- Power BI (Power Query, DAX measures, Visuals)
## 4. Key features:
- Churn rates = Number of Churned Customer / Total Number of Customer
## 5. Dashboard: [attached file](https://github.com/NguyenPhuongNghi/Customer-Churn-Analysis/blob/main/Customer%20Churn%20Analysis.pbix)
### Page 1: Overview
![alt](https://github.com/NguyenPhuongNghi/Customer-Churn-Analysis/blob/main/photo/Screenshot%202025-05-28%20151950.png?raw=true)
#### By Churn Reasons/Categories:
- The top reasons for churn are related to competitor offerings, with "Competitor made better offers" (16.87%) and "Competitor had better devices" (16.54%) being the leading causes.
- "Attitude of support person" (11.30%) is also a significant factor, highlighting the importance of customer service<br>
#### By Contract type:
- A significantly large portion of churn comes from customers with "Month-to-Month" contracts (87.92%). This suggests that customers without long-term commitments are more likely to switch providers.
- "One Year" (9.33%) and "Two Year" (2.75%) contract holders churn at much lower rates, indicating that longer contracts may lead to greater customer retention.<br>
#### By State:
- Churn rates varies geographically and the state with the highest churn rates is California (63.24%)
### Page 2: Analyze Churn rates by Age, Payment Method and Contract type
![alt](https://github.com/NguyenPhuongNghi/Customer-Churn-Analysis/blob/main/photo/Screenshot%202025-05-28%20152442.png?raw=true)
#### By Age Group:
- The largest customer segments appear to be in the middle age ranges (20s to 50s).
- The churn rates show a generally increasing trend with age, particularly noticeable in the 70-80 age group. This suggests that older customers might be more likely to churn.
#### By Payment Method:
- Direct Debit has the highest number of customers (55.36%), followed by Credit Card (39.09%) and then Paper Check (5.55%).
- Paper Check has the highest churn rates (38.01%), followed by Direct Debit (34.49%) and Credit Card (14.46%). This might be due to the inconvenience of Paper Check
#### By Number of Customer in Group:
- The average monthly charge of individual customers (group size 0) is, on average, approximately 1.5 times as high as that of group customers
- The churn rates for individual customers are, on average, 5 times as high as that for group customers. This suggests that customers in larger groups are less likely to churn due to lower charges, highlighting the effectiveness of group contracts for retention.
#### By Account Length and Contract Type:
- The churn rate for Monthly contracts is significantly higher and more volatile throughout the customer lifecycle. It generally decreases over the account length but with considerable fluctuations.
- The churn rate for Yearly contracts is consistently much lower than monthly contracts and shows a more stable, generally decreasing trend over the account length. This reinforces the idea that longer-term contracts lead to better customer retention.
### Page 3: Analyze Churn rates by Extra Charges:
![alt](https://github.com/NguyenPhuongNghi/Customer-Churn-Analysis/blob/main/photo/Screenshot%202025-05-28%20152208.png?raw=true)
- Brief Explanation: Customers without an unlimited data plan have to pay extra data charges. Customer without International Plan have to pay extra charges for international calls.
#### By Unlimited Data Plan (UDP) And Download Volume:
- 67.21% total customers use UDP
- For those consuming "Less than 5 GB": the churn rate for those with UDP is almost 3 times as high as that for those without UDP. This might be because the average monthly charge for those with UDP is almost 3 times higher than that for those without UDP and users think that the avg monthly charge is too high for their low demands
- For those consuming "Between 5 and 10 GB" and "More than 10 GB": the churn rates for those with and without UDP are relatively the same. This might be because the avg monthly charges for those with and without UDP are relatively equal.
#### By International Plan (IP) And Download Volume:
- 9.74% total customers use IP
- For those making less than 50 calls: the churn rate for those with IP is approximately 1.7 times as high as that for those without IP. This might be because the average monthly charges for those with and without IP are relatively the same and they don't need IP for such low demands
- For those making more than 50 calls: the churn rate for those with IP is significantly lower than that for those without IP and generally decreasing over calls volume. This might be cause their demands are higher and they use IP to save expenses and get preferential prices.
### Page 4: Analyze Churn rates by Customer Service:
![alt](https://github.com/NguyenPhuongNghi/Customer-Churn-Analysis/blob/main/photo/Screenshot%202025-05-28%20162114.png?raw=true)
#### Average Customer Service Calls and Churn Rate by State:
- California (CA) has the highest churn rate of 63.24%, followed by Ohio (34.81%) and Pennsylvania (33.33%) . California has a relatively low number of total calls compared to its high churn, suggesting that when customers in California decide to leave, they might not even bother contacting customer service 
- Churned Customers tend to have a higher average number of customer service calls (2.4 calls) than those who didn't churn (0.4 calls). This suggests that customers reaching out to customer support more frequently might be experiencing issues that eventually lead to them leaving.
- % Total customers that churned because of "attitude" (of support person/service provider) and dissatisfaction are considerable, at 15.98% and 15.92%. This hightlight the needs to improve customer service, especially in Alabama and Maryland.
## 6. Insights:
**- Competitor Analysis & Offer Improvement:** Conduct competitor analysis to understand their strengths and offers. Develop more attractive pricing, bundles, and device options to compete effectively.
<br> **- Target Engagement for Older Customers:** Develop tailored communication or support to help them with technical difficulties or different needs, etc because % total churned customer aged 70 and above is consider (30-35%)
<br> **- Incentivize Longer-Term Contracts:** Offer discounts, exclusive features, or other benefits to encourage customers to commit to one or two-year contracts.
<br> **- Promote Group Contracts:** Actively market group plans and their advantages to increase adoption.
<br> **- Customer Service Training & Improvement:** Invest in comprehensive training for support staff focusing on empathy, problem-solving, and positive communication. Implement quality assurance measures and feedback mechanisms.
<br> **-Promote Unlimited Plans:** Actively market the benefits of unlimited data and international plans to customers who have high demands for download volume and making international calls.
<br> **- Offer Flexible Plan Options:** Consider offering tiered plans or add-ons that better suit different usage patterns categorized by consumption level, reducing the likelihood of unexpected overages.
<br> **- Review Overage Pricing:** Evaluate the pricing structure for extra data and international calls to ensure it is fair and doesn't lead to significant customer dissatisfaction.
<br> **- Improve First Call Resolution:** Focus on resolving customer issues effectively on the first contact to reduce the need for repeated calls and potential frustration.
<br> **- Analyze Customer Service Interactions:** Identify common issues and pain points raised by customers contacting support and address them proactively. Provide sufficient training for all customer service staff. 



