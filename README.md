# Customer Segmentation Using CART – Dunnhumby Retail Dataset

This project applies a complete data science workflow to segment customers based on household demographics, purchasing patterns, and response to marketing campaigns. The analysis is built around the **Dunnhumby “The Complete Journey”** dataset and uses a **Decision Tree Regressor (CART)** to model behavior and uncover actionable insights.

---

##  Dataset

We used the publicly available [Dunnhumby - The Complete Journey](https://www.kaggle.com/datasets/frtgnn/dunnhumby-the-complete-journey) dataset, which includes:

- `transactions`: Purchase history of households  
- `product`: Product-level details and categories  
- `coupon`: Coupon information  
- `hh_demographic`: Household characteristics  
- `campaign_table`: Campaign assignments  
- `causal_data`: Display and promotion data  
- `campaign_desc`: Campaign descriptions  
- `coupon_redempt`: Coupon redemption records  

---

##  Workflow Summary

1. **Data Ingestion & Cleaning**
   - Read large CSVs in chunks to handle memory efficiently
   - Cleaned nulls and inconsistencies across all tables

2. **Data Integration**
   - Joined tables to construct household-level profiles
   - Created a relational ERD to define table connections

3. **Feature Engineering**
   - Metrics: 
     - Average Transaction Value (ATV)  
     - Average Basket Size (ABS)  
     - Average Price Point (APP)  
     - Visit Frequency & Latency  
     - Coupon Redemption Rate  
     - Response to promotions

4. **Exploratory Data Analysis**
   - Visualized key metrics using `seaborn` and `matplotlib`
   - Identified behavioral patterns across customer segments

5. **Modeling**
   - Normalized feature set for training
   - Trained a CART (Decision Tree Regressor) model
   - Interpreted tree outputs to define segmentation logic

6. **Output**
   - CSV exports for intermediate and final cleaned datasets
   - Segment profiles with distinct behavioral traits

---

## Tools & Libraries

- Python 3.x  
- `pandas`, `numpy`, `sqlalchemy`  
- `matplotlib`, `seaborn`  
- `scikit-learn`  
- `tqdm`, `gdown`  

---

##  Getting Started

1. Clone the repo  
2. Ensure all dependencies are installed (`requirements.txt` recommended)  
3. Run the notebook sequentially  
4. Inspect exported CSVs and visualizations  

---

##  Contributors

- Gratus Richard Anthuvan Rosario  
- Fahad M Mujawar  
- Sachin Joseph Fernando  

This project was developed as part of an academic assessment for the *Data Science with Machine Learning* module (COMP4030).

---

##  License

For academic and educational use only.
