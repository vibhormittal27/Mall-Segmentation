# Customer Segmentation using KMeans Clustering + PCA

## Overview
Unsupervised machine learning project that automatically 
discovers 5 distinct customer segments from mall shopping data.
No labels. No supervision. Pure pattern recognition.

## Dataset
200 mall customers with Age, Annual Income and Spending Score.
Source: Kaggle Mall Customer Segmentation Dataset

## Methodology
1. Selected Annual Income and Spending Score as clustering features
2. Applied StandardScaler — mandatory for distance based algorithms
3. Used Elbow Method to find optimal K=5
4. Trained KMeans with K=5
5. Applied PCA to visualize segments in 2D space

## Customer Segments Discovered

| Segment | Age | Income | Spending | Count |
|---------|-----|--------|----------|-------|
| Budget Seniors | 45 | Low | Low | 81 |
| Middle Ground | 42 | Medium | Medium | 39 |
| Young Impulsive | 25 | Low | High | 35 |
| Careful High Earners | 41 | High | Low | 23 |
| Premium High Rollers | 32 | High | High | 22 |

## Business Recommendations

| Segment | Strategy |
|---------|----------|
| Premium High Rollers | VIP treatment, premium products, early access |
| Young Impulsive | Trendy products, buy now pay later options |
| Careful High Earners | Value proposition, quality over quantity |
| Budget Seniors | Loyalty discounts, affordable product lines |
| Middle Ground | Standard loyalty programs, consistent engagement |

## Key Findings
- Budget Seniors are largest segment — 40% of all customers
- Premium High Rollers are smallest but highest revenue per customer
- Young Impulsive customers spend beyond their income — high churn risk
- PCA confirmed Income and Spending Score explain 100% of variance
- A business treating all customers the same is leaving money on the table

## Visualizations
- Elbow curve showing optimal K selection
- Cluster scatter plot — Income vs Spending Score
- PCA 2D visualization of all 5 segments

## Technical Stack
- Python
- Pandas
- Scikit-learn — KMeans, StandardScaler, PCA
- Matplotlib

## What I Learned
- Unsupervised learning finds patterns without any labels
- Feature scaling is mandatory for distance based algorithms
- PCA reduces dimensions while preserving maximum information
- Business interpretation of clusters matters more than technical accuracy
