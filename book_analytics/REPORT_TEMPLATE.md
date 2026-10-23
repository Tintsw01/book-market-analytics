# Book Market Analytics: Books to Scrape
*Consulting report | Data Science 500 | [Your name, ITS number]*

(Front matter required by the brief: cover page, signed declaration of originality, Table of Contents.)

## 1. Introduction
Purpose of the analysis, the client (publishing analytics team), the question (what influences book price and rating?), and a one-line description of the data source and the model built.

## 2. Methodology
### 2.1 Data acquisition
Site, tool (requests + BeautifulSoup), 50 listing pages + 1,000 detail pages, fields collected, rate limiting and ethics (sandbox site made for scraping). State the final number of books: `n_books` in `results/summary.json`.
### 2.2 Data cleaning
Duplicates by UPC, price converted from text to numeric GBP, rating words mapped to 1-5, stock quantity parsed from the availability text, missing descriptions handled (flag + empty text), text cleaned, outliers checked (IQR) and kept. Justify each decision.
### 2.3 Exploration and visualisation
Which charts were produced (`figures/01-06`) and why.
### 2.4 Modelling
Linear Regression, target = price, the features used and why, one-hot genre with rare genres grouped, 80/20 split, 5-fold cross-validation, baseline = predict the mean.

## 3. Key insights
Use the figures and `summary.json`. Cover: price level and spread, relationship between star rating and price, genre differences (with counts), correlations with price. Insert the figures with captions and one or two sentences of interpretation each.

## 4. Modelling outcomes
Table of MAE, RMSE, R² (train, test, baseline) and cross-validated R². Explain in plain language what the numbers mean (for example, "on average predictions are off by £X"). Discuss the strongest coefficients and whether they make business sense. Include `figures/07` and `figures/08`.

## 5. Limitations
Sandbox data (prices are not real market prices), few available features (no author, publisher, pages, format), linear assumptions, small genres, any pattern seen in the residuals.

## 6. Practical implications and recommendations
Separate short recommendations for (a) retailers, (b) publishers, (c) data-driven book buyers. Each must follow from a finding above, and be honest if the data show that price is hard to predict from catalogue information alone.

## 7. Conclusion
Three or four sentences summarising findings and next steps (richer features, non-linear models, real market data).

## References
Harvard style. Include at least: the Books to Scrape site (accessed date), the BeautifulSoup, pandas, scikit-learn and seaborn documentation, and any textbook or article you cite.
