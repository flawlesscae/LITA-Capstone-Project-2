# LITA-Capstone-Project-2
This analysis report offers a succinct overview of customer behavior regarding subscription patterns and the associated revenue for the services division of company XYZ, utilizing tools like Microsoft Excel, SQL Server, and Power BI.

## Analyzing Customer Data for Subscription Patterns and Revenue
## Outline
[Overview](#Overview)

[Tools and Technologies](#Tool-and-Technologies)

[Objectives](#Objectives)

[Data Collected](#Data-Collected)

[Data Preparation and Cleaning](#Data-Preparation-and-Cleaning)

[Exploratory Data Analysis](#Exploratory-Data-Analysis)

[Analysis, Visualization and Inference](#Analysis-Visualization-and-Inference)

[Analysis](#Analysis)

[Visualization](#Visualization)

[Inference](#Inference)


### Overview
---
The primary goal of this analysis report is to gain insights into customer behaviour regarding their subscription patterns and the associated revenue generated for the services arm of company XYZ. 

### Tools and Technologies
---
1. Microsft excel: for data storage, cleaning and integration.
2. Microsoft SQL Server: for indept analysis of the data provided.
3. Microsoft Power Bi: for data visualization and reporting.

### Objectives
---
The goals/objectives of this report is to:
1. **Identify key metrics such as:**
   - **Customer Lifetime Value (CLTV):** Measures the total revenue a customer genetrates over the period of 2 years as provided in the dataset.
   - **Customer Acquisition Cost (CAC):** Cost of acquiring a new customer.
   - **Churn Rate:** Percentage of customers who stop subscribing within a specific period.
   - **Monthly Recurring Revenue (MRR):** Total recurring revenue generated each month.**Average Revenue Per User (ARPU):** Average revenue generated per user.
2. **Analyze subscription patterns:**
   - **Subscription Length:** How long customers typically stay subscribed.
   - **Upgrade/Downgrade Frequency:** How often customers change their subscription plans.
   - **Payment Patterns:** How customers pay (e.g monthly, annually).
4. **Identify revenue trends:**
   - **Revenue Growth:** Overall growth in revenue over the period of 2 years (as provided in the dataset).
   - **Seasonal Trends:** Patterns in revenue based on specific periods (e.g holidays, seasons).
   - **Revenue by Customer Segments:** Revenue generated by different customer groups or regions.

### Data Collected
---
**Exerpts from the Customer Data provided:**
![CustomerData](https://github.com/user-attachments/assets/a0b95f67-6e24-42fc-aea1-cc4ee65687fb)


### Data Preparation and Cleaning
---
The dataset (as seen in the exerpts above) was cleaned and prepared using Microsoft Excel and certain formulas were employed to calculate 
1. average subscription duration,
2. to identify the most subscription type as shown below and
3. total revenue by region.

```
1. =AVERAGEIF(D:D, D2, L:L) 

2. =COUNTIF(D:D, D2)

3. =SUMIF(C:C, C2, H:H)

where C:C represents the column which contains the data for region, D:D - suscription types, H:H - revenue and L:L is a calculated column containing subscription duration.
```

Below are screenshots showing the results for average subscription duration and the identification of the the most popular subscription type using excel formulas and also pivot tables alongside other interesting reports from the data provided.

**Average Subscription Duration** 

**Using Formula** ![Avg  Sub Formula](https://github.com/user-attachments/assets/247a3f55-9b48-4240-8426-5bc5e4d988ae)

**Using Pivot Tables** ![avg  sub  duration B](https://github.com/user-attachments/assets/8bdf310c-428d-4b8b-9ea7-a2f1fa454f38)


**Most Popular Subscription Type**

**Using Formula** ![count of sub  type](https://github.com/user-attachments/assets/78416198-e8af-4b25-b469-610a23c54730)

**Using Pivot Table** ![count of sub  type B](https://github.com/user-attachments/assets/7be3d30d-f3f3-4dc4-af92-5682bab16a2d)


**Total Revenue** 

**Using Formula** ![Total Revenue Formula](https://github.com/user-attachments/assets/afd33935-9e20-402f-93f0-6d33ddb90441)

**Using Pivot Table** ![sum of revenue by region](https://github.com/user-attachments/assets/e968c8f2-8eaa-4fee-8360-0c2e986e4f7e)


**Using pivot tables to find subscription patterns**
![revenue by sub  type](https://github.com/user-attachments/assets/a18b2fe9-4c3c-41d8-93df-1166b3114889)

![revenue,sub  type, canceled](https://github.com/user-attachments/assets/3a0ab653-3c11-4685-949e-b113c28a2ee7)

![region,revenue,sub  canceled](https://github.com/user-attachments/assets/39ac6e8e-c5a0-4abc-94b5-79f9d0fb5eaa)


**Top 10 Customers by Revenue**
![top 10 customers](https://github.com/user-attachments/assets/ad437247-2ea2-46b8-848f-119899d1e102)


## Exploratory Data Analysis
## Analysis, Visualization and Inference

### Analysis
---
Shown below are the analysis and insights generated from the dataset provided using Microsoft SQL SSMS Queries.

![0  CustomerData](https://github.com/user-attachments/assets/09eb643e-524f-4df1-a02a-feebad5d3e7f)

![1  CustomerData](https://github.com/user-attachments/assets/8fcadd1c-5fa4-4242-8e3c-9e59838043de)

![2  CustomerData](https://github.com/user-attachments/assets/a2104259-a0f0-4966-8d92-68301c08baca)

![3  CustomerData](https://github.com/user-attachments/assets/56c46569-44ff-4181-963f-1408cb70eb26)

![4  CustomerData](https://github.com/user-attachments/assets/89b4665b-3d61-4ab3-9f74-d115db92e1d1)

![5  CustomerData](https://github.com/user-attachments/assets/30dfd434-1c84-4a2d-b958-b29ebf8688b3)

![6  CustomerData](https://github.com/user-attachments/assets/8aab8ba1-851a-426a-bd9d-1a72a63668bb)

![7  CustomerData](https://github.com/user-attachments/assets/a5ecff4d-84e7-49f2-ba42-dcda8de029c0)

![8  CustomerData](https://github.com/user-attachments/assets/3aebec64-2fbe-4e44-9610-ae87ab09ee39)


### Visualization
---
Visual Representation for all the Regions
![General 1](https://github.com/user-attachments/assets/68a68e67-efbe-4cdc-a6b3-e21ac92993f0)

![General 2](https://github.com/user-attachments/assets/a1bf85c1-ce56-45ce-b4e5-603219dab2b8)

![General 3](https://github.com/user-attachments/assets/6f5d47e8-20d5-43dd-83f7-3f298f59f918)

Visuals for East Region
![East 1](https://github.com/user-attachments/assets/bc79e4f9-8cf7-4fd8-b281-f4aa1b47b7b1)

![East 2](https://github.com/user-attachments/assets/9a38e098-6a3b-4e1a-8c00-65e8899668a9)

![East 3](https://github.com/user-attachments/assets/5d619e14-1c15-41de-9b0b-d5285486b1c3)

Visuals for North Region
![North 1](https://github.com/user-attachments/assets/9ded5a6c-a671-47a5-8ace-60d8aea22d12)

![North 2](https://github.com/user-attachments/assets/26707d94-5233-49ac-9a7d-b8db0e2849c7)

![North 3](https://github.com/user-attachments/assets/e331721b-09e2-489a-9674-a21304e7b8a9)

Visuals for South Region
![South 1](https://github.com/user-attachments/assets/28b0b63a-6cb8-4acf-b67a-f39fbb5b707a)

![South 2](https://github.com/user-attachments/assets/0fbbcaf1-b499-4e2d-8058-de2c86e31037)

![South 3](https://github.com/user-attachments/assets/47d36c63-9f22-49ea-8865-e6e15564ada2)

Visuals for West Region
![West 1](https://github.com/user-attachments/assets/02efc403-fcb1-4838-8260-de9626e0ff7f)

![West 2](https://github.com/user-attachments/assets/1d9efeb6-7118-43dc-88a8-7d03e57bed79)

![West 3](https://github.com/user-attachments/assets/897d8005-077f-48b7-aebd-eb51942e7004)


### Inference
---
- **Revenue and Customers:**
The company generated a total revenue of $67,540,175 and has a total of 33,787 customers.
- **Subscription Types and Renewals:**
There are three types of subscriptions: Basic, Premium, and Standard. The majority of customers (15,175) have the Standard subscription.
A significant number of customers (18,612) did not renew their subscriptions.
- **Regions and Average Subscription Duration:**
The company operates in four regions: East, North, South, and West.
The average subscription duration across all regions is 365 days.
There is a variation in average subscription duration by region, with some regions having higher average durations than others.
- **Overall:**
The company has a significant number of customers and generates substantial revenue.
However, the high number of canceled subscriptions suggests that there may be issues with customer retention.
Further analysis is needed to understand the reasons for cancellations and to improve customer retention strategies.

**Additional Insights:**
- **Subscription Renewal:** The company could focus on improving its renewal rates, especially for the Standard subscription type, which has the highest number of cancellations.
- **Customer Segmentation:** Segmenting customers based on their subscription type and region could help identify specific areas for improvement.
- **Customer Satisfaction:** Conducting customer surveys to understand their satisfaction levels and pain points could provide valuable insights for enhancing the customer experience.


**Link for Tools Download**
1. Microsoft Excel [Download Microsoft Excel Here](https://www.microsoft.com)
   
2. Microsoft SQL Server [Download Microsoft SQL SSMS Here](https://www.microsoft.com)

3. Microsoft Power Bi [Download Microsoft Power Bi Here](https://www.microsoft.com)

