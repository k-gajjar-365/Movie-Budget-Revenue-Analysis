# 🎬 Movie Budget vs Box Office Revenue Analysis

Do higher film budgets lead to more box office revenue? This project explores the relationship between production budgets and financial performance using movie data scraped from [The Numbers](https://www.the-numbers.com/movie/budgets) on **May 1st, 2018**.

<img src="https://i.imgur.com/kq7hrEh.png" alt="Movie Budget vs Revenue" width="600"/>

---

## 📊 Project Overview

This notebook walks through a complete data analysis pipeline:

- Cleaning and preprocessing raw movie budget and revenue data
- Identifying unreleased and zero-revenue films
- Exploring profitability trends
- Visualizing budget vs revenue relationships
- Running linear regression to quantify correlations

---

## 🧰 Tools & Libraries Used

- **Python** (Pandas, NumPy, Matplotlib, Seaborn)
- **Scikit-learn** for regression modeling
- **Jupyter Notebook** for interactive analysis

---

## 📁 Dataset Details

- Source: [The Numbers](https://www.the-numbers.com/movie/budgets)
#### Columns:
 - `Rank`
 - `Release_Date`
 - `Movie_Title`
 - `USD_Production_Budget`
 - `USD_Worldwide_Gross`
 - `USD_Domestic_Gross`

---

## 🧼 Data Cleaning Steps

- Removed `$` and `,` from currency columns
- Converted budget and revenue columns to numeric types
- Converted `Release_Date` to datetime format
- Filtered out unreleased films (after May 1st, 2018)
- Removed duplicates and handled missing values

---

## 📈 Key Insights

- 💸 **Average Production Budget**: `~$31 million`
- 🌍 **Average Worldwide Gross**: `~$89 million`  
- ❌ **Films That Lost Money**: `~30%` of released films  
- 🎥 **Zero Revenue Films**: Identified both domestic and worldwide flops  
- 📅 **Decade-wise Trends**: Split into pre-1970 and post-1970 films for comparison

---

## 📉 Regression Analysis

Using Seaborn and Scikit-learn, we plotted and modeled the relationship between budget and revenue:

- Older films show weaker correlation.
- Newer films (post-1970) display a clearer linear trend.
- A `$150M` budget film is predicted to gross `~$500M` worldwide.

---

## ✅ Conclusion

This analysis reveals a clear trend: **higher production budgets generally correlate with higher worldwide box office revenue**, especially for films released after 1970. While not every big-budget film guarantees success, the data shows that:

- 📈 Most profitable films tend to have substantial budgets and wide international releases.
- ❌ Around **30% of films** still lose money, highlighting the risk inherent in film production.
- 🎬 Films like *Fantastic Four (2005)*, with a budget of ~$87.5M and a worldwide gross of ~$333M, demonstrate how blockbuster investments can yield strong returns.
- 🧨 On the flip side, niche or limited-release films like *Ten (2003)* grossed just ~$105K despite theatrical efforts.

Ultimately, while budget is a strong predictor of revenue, **factors like genre, marketing, release strategy, and audience appeal** play crucial roles in a film’s financial success.

---
## 📚 Future Improvements
- Include genre and rating data for deeper insights

- Explore ROI and profitability metrics

- Build predictive models for future releases
---


