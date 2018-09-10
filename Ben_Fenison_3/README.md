Webscraping, APIs, and Natural Language Processing - Project 





I performed a web scrape from two subreddits:
1) Stock Market ~subreddit
2) CryptoCurrency Market ~ subreddit

Problem Statement: Are people who talk about CryptoCurrenies also talk about the Stock Market, & Visa Versa?


Hypothesis: I thought I would find that both groups talk and compare about investment opportunities in each market.


Proccessing:

After scrapping I removed all the html and json formatting

I gathered around 1,000 posts from both subreddits and from these posts I extracted the words from the 'Title' & 'Sefltext'

Created a DataFrame for my Title, Selftext, and Subreddit 



Models:

I formed a Logistic Regression model w/ ( Cross validation & Penalty: L2/Ridge ) that had a 93% accurate classification rate

I also conducted a pipeline with Random Forest & TFIDF that produced a 86% accurate model , which when compared to my Logistic Regression model was worst. 



Conclusion:

Suprisingly, The top words that both subreddits had in common were neither about stock market of cryptocurrencies, So I cannot fully come to a conclusion but from what I saw, I can assume that People who invest in Stock Market do not have a high probabiity of talking about investment opportunities in CryptoCurrency Markets, & Visa Versa.
