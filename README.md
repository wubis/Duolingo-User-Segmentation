# Duolingo-User-Segmentation
Data-driven segmentation for building Duolingo user personas

## Project Overview

This project explores Duolingo’s user base by combining survey data (demographics, motivations) with app usage data (lessons completed, streaks, crowns, subscriptions).
Using unsupervised learning (clustering), I identified three actionable user personas that can inform product design and marketing strategy.

The final deliverable includes both a technical notebook and a business-facing report.

## Objectives
1. Understand how Duolingo users differ in behavior and demographics
2. Create meaningful and interpretable user segments using clustering
3. Provide product and marketing recommendations to increase engagement and reduce churn

## Methods & Tools
Data Processing: Pandas, NumPy, scikit-learn
Exploratory Data Analysis: histograms, correlation matrices, summary statistics
Modeling: K-Means, Gaussian Mixture Models (GMMs), PCA for visualization
Evaluation: Silhouette scores to compare clustering performance
Visualization: Matplotlib, Seaborn

## Key Results
Tested K-Means and Gaussian Mixture Models
- K-Means: produced weak clusters (very low silhouette scores)
- GMM: yielded stronger natural separation (silhouette ≈ 0.25)

Final segmentation produced 3 core personas:
- Young Ambitious Students (~10%) – highly engaged, loyal, many paying subscribers
- Steady Casual Adults (~70%) – broad group, low engagement, high churn risk
- Motivated Students (~20%) – moderate activity, younger users, high upgrade potential

## Recommendations
Product
- Engagement-based matchmaking (MMR) for competitive users
- Flexible lesson lengths + streak protection to reduce churn
- Curated media integration (via streaming partnerships) to boost immersion

Marketing
- Persona 1: Promote premium student benefits
- Persona 2: Highlight "learn at your own pace"
- Persona 3: Market Duolingo as a fun daily challenge (like Wordle)

## Future Work
- Explore time-series analysis of streak retention
- Build churn prediction model for at-risk users
- Test other clustering methods (DBSCAN, hierarchical)
