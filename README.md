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
- Google Colab Notebook  
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
- Campaign **916** delivered the **highest ROI (0.387)** while Campaign **1178** had high spend ($55.7K) but **lowest ROI (0.048)** → prime candidate for budget reallocation.  
- **Older age groups (45-49)** showed the **highest CTR**, with CTR increasing monotonically from younger to older cohorts (30-34 to 45-49).  
- **Gender patterns**: Female cohorts demonstrate lower CPC in multiple age bands, improving cost efficiency potential.  
- **Budget forecast**: +20% budget increase projects proportional conversion gains, but low-ROI campaigns remain inefficient → scale selectively, not uniformly.
 

## 🚀 How to Run
```bash
git clone https://github.com/<your-username>/Ad-Campaign-Performance-Optimization.git
cd Ad-Campaign-Performance-Optimization
jupyter notebook ad_campaign_analysis.ipynb
