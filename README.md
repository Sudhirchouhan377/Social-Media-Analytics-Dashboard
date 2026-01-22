# Sales Conversion Optimization Analysis


## PowerBI Deshboard
(Social-Media-Analytics-Dashboard.png)

## Project Overview
This project analyzes the **Sales Conversion Optimization** dataset obtained from Kaggle, originally shared by **GOKAGGLERS**.  
The dataset contains marketing and conversion performance data from an anonymous organization’s **social media advertising campaigns**, primarily run through Facebook.

The objective of this project is to:
- Clean and validate the dataset
- Perform exploratory data analysis
- Engineer meaningful marketing KPIs
- Visualize campaign performance using Power BI
- Derive insights to improve conversion efficiency

---

## Dataset Description

- **Source:** Kaggle –  https://www.kaggle.com/datasets/loveall/clicks-conversion-tracking 
- **Total Entries (Original):** 1143  
- **Total Columns:** 11  

### Column Details
| Column Name | Description |
|------------|-------------|
| `ad_id` | Unique identifier for each advertisement |
| `xyzcampaignid` | Campaign ID assigned by XYZ company |
| `fbcampaignid` | Campaign ID tracked by Facebook |
| `age` | Age group of the person shown the ad |
| `gender` | Gender of the person shown the ad |
| `interest` | Interest category code based on Facebook profile |
| `Impressions` | Number of times the ad was displayed |
| `Clicks` | Number of clicks received by the ad |
| `Spent` | Amount spent by XYZ company on the ad |
| `Total_Conversion` | Number of people who enquired about the product |
| `Approved_Conversion` | Number of people who purchased the product |

---

## 🧹 Data Cleaning & Preparation

### Tools Used
- **Microsoft Excel** – Data cleaning & preprocessing  
- **Microsoft Power BI** – Data visualization & dashboard creation  

### Cleaning Steps
- No missing or invalid data types were found.
- **Data inconsistency detected:**  
  - 204 records had `Clicks = 0` but `Total_Conversion > 0`.
  - This is logically incorrect, as conversions cannot occur without clicks.
- These inconsistent rows were removed.

### Final Dataset
- **Cleaned Entries:** 939  
- **Columns:** 11  

---

## Methodology

After observation, it was found that there were no null or invalid type values present in the data. However, it was easy to notice that some entries (204 entries) were having error as Column “Clicks” had value 0 but Column “Total_Conversion” had non-zero values. This is illogical because an ad cannot still gain postive conversions (customers) while no one clicks on it. So, after removing those data, Our dataset consist a total of 939 entries.

### Cost per Mille (CPM)
- It is a metric that represents the cost of displaying an ad to 1,000 people. In other words, it measures how much a business pays for every 1,000 ad impressions.
### Cost per click (CPC) 
- It is a metric that represents the cost of getting a user to click on an ad. It measures how much a business pays for every click on their ad.
### Click-through rate (CTR)
- It is a metric that represents the percentage of users who click on an ad after seeing it. It measures the effectiveness of an ad in getting users to click through to a website or landing page
### CPA (Cost per Acquisition/Action)
- It is a metric that represents the cost of acquiring a new customer through an ad campaign. It measures how much a business pays for every new customer acquired through their ad.
