# High-Income Targeting & Segmentation Project

**Author:** Yoon Nam  

## Overview

This project builds a predictive model to identify high-income individuals and translates the results into actionable customer segments to improve marketing ROI.

Workflow:
Data → Classification Model → Ranked Customers → Segmentation → Targeting Strategy


---

## Files Included

### 1️⃣ YoonNam_JPMC_1_classifier.ipynb  
Builds and evaluates the high-income classification model.

- Data preprocessing & feature engineering  
- Model training and lift analysis  
- SHAP-based feature importance  
- Exports scored dataset for segmentation  

**Key Results**
- Top 5% customers → ~16x lift  
- Top 20% → ~4–5x lift  

---

### 2️⃣ YoonNam_JPMC_2_segmentation.ipynb  
Performs customer segmentation and strategy design.

> ⚠️ This notebook loads the scored output file generated from `YoonNam_JPMC_1_classifier.ipynb`.  
> Please run Notebook 1 first to generate the required dataset.

- Segment creation based on model score  
- Segment-level performance comparison  

---

### 3️⃣ YoonNam_JPMC_Project_Report.pdf  
Executive summary of modeling results, lift performance, key drivers, and strategic recommendations for a retail business client.

---

## How to Run

1. Run `YoonNam_JPMC_1_classifier.ipynb`  
   → This generates and saves the scored dataset  

2. Run `YoonNam_JPMC_2_segmentation.ipynb`  
   → This loads the saved dataset and performs segmentation  

**Required libraries**
pandas, numpy, scikit-learn, matplotlib, shap
