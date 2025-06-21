# Soccer Player Valuations Using Unsupervised Learning

A project exploring whether unsupervised machine learning can effectively group soccer players and predict their market valuations, compared to traditional supervised learning approaches.

## Project Overview

This project investigates how well unsupervised learning methods can understand and predict soccer player market valuations by discovering natural groupings in player characteristics and performance data.

**Main Research Question**: Can we group soccer players into meaningful clusters based on their attributes and performance, and use these clusters to predict market valuations without initially knowing the target values?

## Dataset

You can download the data from here: https://www.kaggle.com/datasets/davidcariboo/player-scores/data

The project uses soccer data from Transfermarkt including:
- **30,000+ players** with characteristics (age, position, height, etc.)
- **400,000+ market valuations** over time
- **1.6M+ performance records** (goals, assists, playing time, etc.)
- **Multiple seasons** of data from major European leagues

## Methodology

### Unsupervised Learning Approach
1. **Player Clustering**: Group players using K-Means, Hierarchical Clustering, and DBSCAN based on:
   - Player characteristics (age, position, physical attributes)
   - Performance metrics (goals, assists, playing time)
   - Career statistics (games played, disciplinary records)

2. **Valuation Prediction**: Use cluster membership to predict market values by assigning cluster median/mean values

3. **Cluster Analysis**: Understand what makes each player group unique and valuable

### Supervised Learning Comparison
- **Linear Regression** and **Random Forest** models using the same features
- **Hyperparameter optimization** for fair comparison
- **Performance evaluation** using R² scores and MSE

## Getting Started

1. Open `soccer_player_valuation.ipynb` in Jupyter Notebook
2. Install required packages: `pandas`, `scikit-learn`, `matplotlib`, `seaborn`
3. Run all cells to reproduce the complete analysis

## Conclusion

This analysis demonstrates that unsupervised learning can effectively discover meaningful patterns in soccer player data and provide reasonable valuation predictions. While supervised methods achieve higher accuracy, unsupervised approaches offer valuable insights into market structure and player categorization that can complement traditional valuation methods.

The clustering reveals that players naturally organize into distinct groups with characteristic market value ranges, suggesting that data-driven player categorization could be a valuable tool for football analytics and decision-making. 
