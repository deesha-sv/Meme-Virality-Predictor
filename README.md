# Meme Virality Predictor

Machine Learning model (R² = 0.27) predicting meme shares from caption length, emoji count, image type & platform. Analyzed 50 memes synthesized from real Reddit/Instagram patterns.

![EDA Plots](images/eda_plots.png)
![Feature Importance](images/feature_importance.png)

## Business Insights
- Image type dominates virality (35% importance) - reaction images lead
- Color brightness (25%) - high contrast memes perform best
- Emoji density matters - optimal 3-5 emojis per caption
- Platform effect - Reddit > Instagram > Twitter for shares

## Model Performance
| Metric       | Value |
|--------------|-------|
| R² Score     | 0.27  |
| Dataset      | 50 memes |
| Algorithm    | Random Forest |
| Test Size    | 20%   |

## Technical Implementation

End-to-end ML pipeline:
1. Data: 50 memes (synthesized from real patterns)
2. Features: 7 engineered vars (emoji_per_word, encodings)
3. Model: RandomForestRegressor (n_estimators=100)
4. Evaluation: Train/test split, R² metric
5. Visualization: Seaborn/Matplotlib

## Dataset Methodology
50 memes synthesized using real social media benchmarks:
- Sources: Reddit r/memes, Instagram meme accounts, Twitter trends (Dec 2025)
- Features: caption_length, emoji_count, image_type (reaction=40%), shares
- Validation: Realistic engagement ratios (shares = 0.6-1.2x likes)

## Business Applications
Social Media Managers:
- Prioritize reaction images + high contrast + 3 emojis
- Post on Reddit for maximum reach
- Target 15-25 char captions (sweet spot)

## Tech Stack
Python 3.9 • Pandas • Scikit-learn • Seaborn • Matplotlib
Jupyter Notebook • Random Forest Regression

## Skills Demonstrated
- Feature Engineering (categorical encoding, derived metrics)
- Exploratory Data Analysis (EDA with statistical visualizations)
- Machine Learning (Random Forest, model evaluation)
- Data Storytelling (business insights from model output)
- End-to-End Pipeline (data → model → insights)
