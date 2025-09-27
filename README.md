# 📊 Ad Campaign Performance Optimization

This project analyzes Facebook Ad Campaign performance data to uncover insights, optimize budget allocation, and forecast future performance.  

## 📂 Dataset
- Source: [Kaggle – Facebook Ad Conversion Dataset](https://www.kaggle.com/datasets/loveall/clicks-conversion-tracking)  
- Shape: 1,143 rows × 11 columns  
- Key Columns:  
  - `Impressions`, `Clicks`, `Spent`, `Total_Conversion`, `Approved_Conversion`  
  - Campaign identifiers: `xyz_campaign_id`, `fb_campaign_id`  
  - Demographics: `age`, `gender`, `interest`  

## 🔑 Key Metrics Calculated
- **CTR (Click-Through Rate)** = Clicks ÷ Impressions  
- **CPC (Cost per Click)** = Spend ÷ Clicks  
- **Conversion Rate** = Total Conversions ÷ Clicks  
- **ROI (Return on Investment)** = Total Conversions ÷ Spend  

## 🛠️ Tech Stack
- Python (Pandas, Matplotlib)  
- Jupyter Notebook  
- Dataset: Kaggle  

## 📊 Analysis Performed
1. **Campaign-Level Performance**
   - CTR, CPC, Conversion Rate, ROI for each campaign.  
   - Identified best vs underperforming campaigns.  

2. **Audience Segmentation**
   - Performance by Age and Gender.  
   - Insights into high-CTR demographics.  

3. **Forecasting (Budget Pacing)**
   - Simulated +20% budget scenario.  
   - Estimated future conversions from extra spend.  

## 📈 Visualizations
- CTR by Campaign  
- ROI vs Spend Scatterplot  
- CTR by Age Group  

Example Plots:  

![CTR by Campaign](images/ctr_by_campaign.png)  
![ROI vs Spend](images/roi_vs_spend.png)  
![CTR by Age](images/ctr_by_age.png)  

## 💡 Key Insights
- Campaign `916` delivered the **highest ROI** while Campaign `1178` had high spend but poor conversions → candidate for budget reallocation.  
- Age group **30-34** had the **highest CTR**, especially among males.  
- With a +20% budget increase in high-performing campaigns, forecast shows a **~15% uplift in conversions**.  

## 🚀 How to Run
```bash
git clone https://github.com/<your-username>/Ad-Campaign-Performance-Optimization.git
cd Ad-Campaign-Performance-Optimization
jupyter notebook ad_campaign_analysis.ipynb
