 # UG Thesis 
This repository contains my undergraduate dissertation, which includes a Twitter scraping module adapted from https://github.com/israel-dryer/Twitter-Scraper/blob/main/twitter_scraper.py to accommodate my slow internet connection. The Delta TF-IDF module is based on https://kgptalkie.com/amazon-and-imdb-review-sentiment-classification-using-spacy/.

To run the code, you must download it and have a functional Python environment with all the necessary packages. You must also properly set up a Selenium webdriver on your computer. Follow this link for instructions: https://selenium-python.readthedocs.io/installation.html or watch this video: https://www.youtube.com/watch?v=9XAH_TvxwLg&t=29s. You also need a Twitter account and password, as specified in the Python script.

The "twitter" folder contains the scraped raw tweets, and the "df_res" folder contains the processed sentiment analysis results. The Twitter search keywords are "Comscore," "Rentrak," "Comscore Merger," and "Rentrak Merger." 

# Short-term Event Study Methodology

The "comscore.csv" and "rentrak.csv" files are the data collected from WRDS CRSP. Ensure that the R code and these files are located in the same root directory when you run the code. The "st_res" folder contains the data frame result of the event study intermediary process. To check other computational data such as CAR, Patell Z, and p-value, running R is required. In the final section of the R code, I have marked each table with a specific code you can run.

# Sentiment Analysis

For sentiment analysis, I first scraped Twitter within [-1, 85] days, and the scraped tweets are in the "twitter" folder. Then I trained the Delta TF-IDF model using the training dataset in the "datasets" folder. To obtain the table for prediction accuracy, you will need to run the actual Python code. I then used the trained algorithm to predict sentiments on actual tweets and aggregated them on a daily frequency, resulting in the "df_res" folder.

That concludes my explanation. If you have any questions or issues, please feel free to write an issue in GitHub.

