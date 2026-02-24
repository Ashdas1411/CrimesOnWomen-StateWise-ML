# Crime Against Women in India  
## A State-Wise Analytical Investigation  
**Author:** Arka Das  

---

## Project Overview

This project analyzes state-wise crimes against women in India using exploratory data analysis, normalization, clustering, and PCA. The goal is to identify high-burden states, compare crime patterns, and uncover structural similarities across regions.

---

## Dataset

The dataset contains state-level crime data across multiple years with the following categories:

- Rape  
- Kidnap & Assault  
- Dowry Deaths  
- Assault against Women  
- Assault on Modesty  
- Domestic Violence  
- Women Trafficking  

Data was cleaned, column names standardized, and crime counts aggregated at the state level.

---

## Methodology

### 1. Data Cleaning
- Renamed columns for clarity
- Removed unnecessary columns
- Standardized state names
- Aggregated crime totals by state

### 2. Total Crime Analysis
A `Total_Crimes` column was created by summing all categories to identify states with the highest reported burden.

**Top states by total crimes:**
- Uttar Pradesh  
- Madhya Pradesh  
- West Bengal  
- Andhra Pradesh  
- Rajasthan  

Large and populous states dominate absolute crime counts.

---

### 3. Crime Category Analysis
Top 5 states were identified for each crime type.

Key observations:
- Madhya Pradesh leads in rape cases.
- Uttar Pradesh dominates kidnapping and dowry deaths.
- West Bengal reports highest domestic violence.
- Tamil Nadu leads in women trafficking.

Crime dominance varies significantly by category.

---

### 4. Normalization & Heatmap
MinMax scaling was applied to compare relative crime intensity across states.

This revealed:
- Domestic violence and assault-related crimes are most prevalent.
- Crime patterns differ structurally across states.
- States do not share a uniform crime profile.

---

### 5. Clustering (K-Means)

States were grouped into 3 clusters based on normalized crime patterns:

- Cluster 0 → Moderate-to-high crime intensity  
- Cluster 1 → Lower overall intensity  
- Cluster 2 → Very high multi-category intensity  

Clustering shows structural segmentation rather than a simple ranking hierarchy.

---

### 6. PCA (Principal Component Analysis)

PCA was used to visualize pattern separation.

- **PC1** captures overall crime intensity.
- **PC2** captures crime composition differences (e.g., trafficking vs assault-heavy states).

This confirms that states differ both in magnitude and in crime structure.

---

## Key Insights

- Crime against women is concentrated in a few high-burden states.
- No single state dominates all crime categories.
- Domestic violence and assault categories account for most reported cases.
- States exhibit distinct structural crime patterns.
- Clustering reveals meaningful regional segmentation.

---

## Tools Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn (MinMaxScaler, KMeans, PCA)

---

## Conclusion

Crime against women in India varies significantly across states in both scale and structure. This analysis demonstrates how data-driven methods such as normalization, clustering, and PCA can uncover regional crime patterns beyond simple rankings, emphasizing the need for targeted, state-specific policy interventions.
