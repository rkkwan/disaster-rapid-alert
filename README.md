# Utilizing Twitter for Disaster Detection  

The goal of this project was to use social media, specifically Twitter, to identify natural disasters as they occur. In this repo you will find the following:    

01 - Code for scraping Twitter  
02 - Code for Doc2Vec feature engineering and Logistic Regression modeling  
03 - Code for making predictions on past and recent tweets  
04 - Visual exploration of Time-series analysis  
05 - Presentation  

This project was developed by:  

Tofer Kim,  
Ritchie Kwan, and  
Will Stecher,  
with special thanks to Li Zhong.  


## Problem Statement  
Traditional methods for alerting on disaster-related events like earthquakes and tsunamis rely on information derived from official sources (e.g. USGS). Twitter can be a valuable resource for sharing information regarding disaster-related events. We will attempt to identify "relevant" tweets in order to investigate Twitter trends that can be used to detect natural disasters as they occur. These methods, along with geolocation and population data, can be implemented to serve as an alert to first-responders (e.g. FEMA) and potentially help save lives.  


## Executive Summary  
Using a provided dataset of over 10,000 disaster-related tweets marked as either "relevant" or "not relevant", we trained a model using NLP to classify tweets as such. Narrowing the scope of our project to detect a specific natural disaster--wildfires--we used the keywords "wildfire" and "forest fire" to collect tweets from two distinct date-ranges: the beginning of the 2018 California wildfires and a more recent period after these fires had subsided.  


## Conclusion & Recommendations  
After running our logistic regression model to classify tweets from the specified time-ranges above, we analyzed the frequency of "relevant" tweets. Our findings show that at beginning of the 2018 California wildfire disaster, there were consistently over 180 "relevant" tweets within a window of 300 seconds (5 minutes). More recent tweets did not exceed this threshold of 180 "relevant" tweets. This distinction can be used to detect future wildfire disasters in as short of a delay as 5 minutes.   

## Next Steps  
We can implement our methods with new keywords and date-ranges in order to observe and detect different types of natural disasters, as well as further train our Doc2Vec model to classify these events. With access to Twitter geolocation and population data, we can further improve our functionality and potentially estimate local areas and number of people affected by future disasters.  



## References  

Training data: [https://www.figure-eight.com/data-for-everyone/](https://www.figure-eight.com/data-for-everyone/)  
Using Twitter for Disaster Response: [https://phys.org/news/2018-07-disaster-response-twitter.html](https://phys.org/news/2018-07-disaster-response-twitter.html)  
Doc2Vec classification methods: [https://towardsdatascience.com/multi-class-text-classification-with-doc2vec-logistic-regression-9da9947b43f4](https://towardsdatascience.com/multi-class-text-classification-with-doc2vec-logistic-regression-9da9947b43f4)  
Twitter scraping: [https://github.com/Jefferson-Henrique/GetOldTweets-python](https://github.com/Jefferson-Henrique/GetOldTweets-python)   
Doc2Vec summarization: [https://medium.com/scaleabout/a-gentle-introduction-to-doc2vec-db3e8c0cce5e](https://medium.com/scaleabout/a-gentle-introduction-to-doc2vec-db3e8c0cce5e)  
