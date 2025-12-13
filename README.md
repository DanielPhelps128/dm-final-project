# dm-final-project — Data/Text Mining (Fall 2025)

**Student:** Daniel Phelps  

**Email:** dphelps9693@floridapoly.edu  

**Website:** [https://danielphelps128.github.io/dm-final-project/ ](https://danielphelps128.github.io/dm-final-project/index_updated.html) 

**Repo:** https://github.com/DanielPhelps128/dm-final-project  

---

## Project in One Sentence
Analyze what drives higher vs. lower home prices using course-approved techniques:  
**EDA / visualization**, **PCA**, and **k-means clustering**.

> Predictive modeling and association rules were intentionally **not included** to maintain transparency and stay within the project scope.

---

## Objective
The goal of this project is to better understand how key home characteristics relate to price in the Ames housing market.  
We use exploratory data mining techniques to:
1) Identify which physical and neighborhood features relate most to price  
2) Summarize structure in the dataset via PCA  
3) Group homes into meaningful market segments using k-means  

This provides a digestible interpretation of the housing market without fitting supervised prediction models.

---

## Dataset
- **Primary structured data:** Ames Housing (Kaggle) — target `SalePrice`  
  https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data  

- Features include:
  - Square footage (above ground + basement)
  - Quality & condition ratings
  - Year built / remodeled
  - Neighborhood
  - Room counts
  - Garage capacity and size

- **License notice:** Follow Kaggle terms.  
  Raw competition files **should not be committed** if not allowed by license.

> You must download the data from Kaggle separately and place `train.csv` under `./data/`.

---

## Methods Used
**Exploratory Data Analysis (EDA)**
- Price distribution (raw + log)
- Scatterplots: living area vs. price
- Boxplots: price by neighborhood + quality

**Dimensionality Reduction (PCA)**
- Scree plot
- PC1–PC2 projection
- Loadings to interpret components

**Clustering (k-means)**
- Performed on PCA space (first 8 PCs)
- Chosen K via silhouette + elbow
- Cluster profiling (price, size, age, quality)

> Result: Three clear segments — entry-level, mid-range, and premium homes.

---

## Key Findings
- Larger above-grade living area + high overall quality are the strongest price drivers.
- PC1 captures a “size/quality” dimension; PC2 captures “layout/verticality.”
- K-means identified three market segments with distinct size, price, age, and quality profiles.

---
