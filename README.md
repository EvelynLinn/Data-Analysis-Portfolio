# Data Analysis Portfolio
This is a portfolio of data analysis projects conducted during Udacity Data Analyst nanodegree.
## Installation
```
pip install pandas numpy matplotlib seaborn statsmodels scikit-learn
```
## Query Twitter Data
I used [Tweepy](https://www.tweepy.org/) to query Twitter's API for additional data beyond the data included in the WeRateDogs Twitter archive.
- First, if you do not already have one, you need to sign up for a [Twitter account](https://help.twitter.com/en/create-twitter-account).
- Next, to set up a developer account, follow the directions on [Twitter’s Developer Portal](https://developer.twitter.com/en/docs/basics/developer-portal/overview), in the “How to Apply” section.

## Project List
#### Project 1. Weather data investigation
A moving average visualisation model based on weather data.
#### Project 2. TMDB movie data analysis
Wrangling, exploratory analysis and visualisation of the data from over 10,000 movies.
#### Project 3. A/B test and practical statistics
Hypothesis testing and regression analysis on whether a new website page performs better than another.
#### Project 4. Data wrangling project description
Gathering data from web scraping, specifically Twitter API, cleaning up 10 quality and 2 tidiness issues, followed by a brief visualisation.
#### Project 5. Prosper Loan Data Exploration
##### Dataset
This data set contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others. The dataset can be found [here](https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv).
##### Summary of Findings 
I focused on the impact from borrowers' financial situations and loans' characteristics on interest rates, by looking into the impact of borrowers' personal situations on the existing correlations between rates and loan types and statuses. The indicators of financial status include: `IsBorrowerHomeowner`, `DebtToIncomeRatio`, `IncomeRange` or `StatedMonthlyIncome`, and `AvailableBankcardCredit`.

On the other hand, as ProsperScore seems to be the strongest indicator, due to the fact that it's not a direct indicator, I tried linking its underlying variables directly to interest rates, including `DebtToIncomeRatio` and `TotalInquiries`. 
##### Key Insights for Presentation 
- Within each income range group, the rate increases as amount of terms increases; overall, for the same amount of terms, people with higher income are able to be granted lower interest rate. 
- For each loan status, overall interest rates slightly decrease as income ranges increase. But once a loan is defaulted or charged off, the interest rates can expect to maintain a same level as past due, instead of keeping growing.
- The amount of available bankcard credits show a negative correlation to interest rates. In fact, low bank card creadit can be a barrier to have lowest interest rates. 
- Higher income doesn't necessarily mean lower interest rate, but in the range of below 0.10 of interest rate, most borrowers are with higher income.
