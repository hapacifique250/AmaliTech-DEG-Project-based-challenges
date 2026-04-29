# Last Mile Logistics Auditor

## A. Executive Summary
Veridi Logistics has experienced a surge in negative customer reviews, suspected to be linked to inaccurate delivery estimates. This project audits delivery performance by comparing estimated vs. actual delivery dates, analyzing geographic patterns of delays, and correlating customer sentiment with logistics accuracy. Findings highlight whether delays are concentrated in specific regions or represent a nationwide issue, providing actionable insights for leadership.

---

## B. Project Links
- **Notebook:** https://colab.research.google.com/drive/1YcVRERlD8b787n0HxIcrNgY44SLJPOsm?usp=sharing  
- **Dashboard:** https://app.powerbi.com/links/K9NBf3_fif?ctid=c4880333-4814-4622-b63c-2b67c199878c&pbi_source=linkShare
- **Presentation:** https://docs.google.com/presentation/d/1Ue_CBC1ug_sCGTtUfK2D0GpD8e4MCjk9/edit?usp=sharing&ouid=105302457115700410673&rtpof=true&sd=true

---

## C. Technical Explanation
### 1. Data Cleaning
- Loaded datasets from Google Drive (`Amali/datasets` folder).  
- Standardized date formats (`order_delivered_customer_date`, `order_estimated_delivery_date`).  
- Removed canceled/unavailable orders from delay calculations.  
- Ensured joins (Orders ↔ Reviews ↔ Customers ↔ Products) avoided duplication.  
- Translated product categories from Portuguese to English using `product_category_name_translation.csv`.

### 2. Core Analyses
- **Schema Builder:** Created master dataset linking orders, reviews, and customer locations.  
- **Delay Calculator:** Computed `days_difference` and classified orders as *On Time*, *Late*, or *Super Late*.  
- **Geographic Heatmap:** Calculated % late deliveries per state.  
- **Sentiment Correlation:** Compared average review scores across delivery statuses.  
- **Translation Challenge:** Added English product categories for global readability.

### 3. Candidate’s Choice Feature
- **Revenue Impact of Late Deliveries:** Calculated total value lost due to late/canceled orders.  
- **Business Value:** Quantifies the financial cost of poor logistics, strengthening the case for operational improvements.

---

## D. Pre-Submission Checklist
- [x] Repo is public (tested in Incognito).  
- [x] Notebook uploaded (`.ipynb`).  
- [x] Notebook exported (`.html`).  
- [x] Raw datasets excluded from repo.  
- [x] Dashboard link is public.   
- [x] README updated with Executive Summary, Project Links, Technical Notes.   
