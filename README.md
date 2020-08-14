
#  Measuring Customer Satisfaction in Delivery Companies Using Sentiment Analysis


#### Group members: 
- Khwla Alsafri
- Wafa Alshehri 
- Hessah Alkhattabi 
- Doaa Alsenani
----


## Table of Contents
* [Introduction](#Introduction)
* [Problem Statement](#Problem-Statement)
* [Data Collection](#Data-Collection)
* [Data Dictionary](#Data-Dictionary)
* [Methodology](#Methodology)
* [Algorithms](#Algorithms)
* [Challenges of Sentiment Analysis](#Challenges-of-Sentiment-Analysis)
* [Modeling](#Modeling)
* [Time Frame](#Time-Frame)
* [Conclusion](#Conclusion)
* [Future Work](#Future-Work)
* [Reference](#Reference)



### Introduction <a name="Introduction"></a>

During these days, our current situation witnesses many precautions due to the outbreak of the Coronavirus (COVID-19) and the home quarantine and curfew, which led to reducing direct customer contact and increasing pressure on the delivery companies in Saudi Arabia.In this project, we seek to measure the extent of customer satisfaction with delivery companies by applying sentiment analysis on customers' tweets before and after this pandemic from the 1st of September 2019 to April 2020. After research, we found that the two delivery companies most talked about on Twitter were Marsol and Hungerstation, so we worked on them.

## Problem Statement <a name="Problem-Statement"></a>
A customer satisfaction rating is often a leading indicator of the success or failure of a company. This project helps in highlighting the customer satisfaction ratio of the delivery companies before and after the COVID-19, by analyzing customer tweets with a sentiment analysis model. Thus, we can know how the companies faced the problems caused by this virus and provided a service to satisfies the customer. This analysis assists companies to make decisions and search for solutions to problems and improve the company's services more by knowing the satisfaction rate.

- What is the customer's satisfaction ratio before and after the COVID-19 for Marsol and Hungerstation delivery companies in Saudi Arabia?

##### Objective
Measure the customer's satisfaction ratio on the Marsol and Hungerstation delivery companies in Saudi Arabia, before and after the COVID-19 by analyzing customers tweets with a sentiment analyses model.


## Data Collection <a name="Data-Collection"></a>
In order to extract relevant information, text mining is the application of natural language processing techniques and analytical methods to the text data. Owing to an exponential rise in digital text data from web pages like Twitter, text mining is getting a lot of attention these last years. Twitter data is a rich source, which can be used to collect information about any imaginable subject. These data may be used in various ways, and we will use it to assess customer sentiment analysis about Marsol and Hungerstation delivery companies in Saudi Arabia from September 2019 to April 2020.

- ### The tools that we used to get data from Twitter:-

- ScrapeHero to collect data from Twitter, it is one of the best 3 data scraping companies in the world that providing custom data collecting. 

- Twitter Advanced Search tool to help us filter the result we are looking for. For example, we use the filter to select the mention of delivery companies, language, the period of time, and words that we do not want to find in our data to avoid spams like coupons and offers from companies.

After obtaining the result, we combine the data to be in two separate datasets one before COVID-19 and the other after COVID-19.

||Before COVID-19|After COVID-19|
|---|---|---|
|Time Period|From September 2019 to February 2020|March and April 2020|
|Rows|22397|8353|
|Features|13|13|
|Important Features|Text and Date |Text and Date|

## Data Dictionary <a name="Data-Dictionary"></a>

|Feature|Type|Dataset|Description|
|---|---|---|---|
|text|object|Before, After COVID-19|The content of the tweet|
|replies|int64|Before, After COVID-19|The number of replies on the tweet|
|retweets|int64|Before, After COVID-19|The number of reposting the tweet|
|favorite|int64|Before, After COVID-19|The number of  likes of on the tweet|
|date|datetime64|Before, After COVID-19|The time the tweet was written|
|company|object|Before, After COVID-19|The company name|
|year|int64|Before, After COVID-19|The year the tweet was written|
|month|int64|Before, After COVID-19|The month the tweet was written|


## Methodology <a name="Methodology"></a>
We will build a sentiment analyses model, to measure the customer's satisfaction ratio for Marsol and Hungerstation delivery companies in Saudi Arabia before the COVID-19 and after, by applying:

1- Data collection by using Twitter Streaming API.
2- Text preparation by using multiple data cleaning techniques.  

- ##### The steps of tweets preparing and Cleaning:
    - Handle Emoticons and Emojis.
    - Removing Stop-word and words with 1 or 2 letters.
    - Removing numbers.
    - Removing Characters.
    - Removing punctuations.
    - Removing normalize Arabic.
    - Removing repeating char.
    - Tokenization.

3- EDA to analyze and visualize the dataset.
4- Presentation of the results by showing the customer's satisfaction ratio for Marsol and Hungerstation delivery companies in Saudi Arabia before the COVID-19 and after.


## Algorithms <a name="Algorithms"></a>

- Use Sentiment Analysis to identify the sentiment of a string of text, will it be neutral, negative or positive.
- Break up text into tokens using Tokenizer.
- Sequential Model.
- GaussianNB Model.
- Naive Bayes Classifier.
- Decision Tree Classifier.
- Random Forest Classifier.
- Extra Trees Classifier.
- KNeighbors Classifier.
- SVM Mode.
- Logistic Regression.
- AdaBoost Classifier.


## Challenges of Sentiment Analysis <a name="Challenges-of-Sentiment-Analysis"></a>

1- Tweets Preprocessing and Cleaning.

2- We need to identify the labels, will it be neutral negative or positive.

3- People express opinions in complex ways, there are multiple layers of meaning in any human-generated sentence which can mislead sentiment analysis.

4- We used manual classification, to avoid misleading and increase the accuracy, It was hard because our data was almost 30 thousand.


## Modeling <a name="Modeling"></a>

We applied multiple machine learning algorithms in order to get high accuracy in predicting the customer’s satisfaction on delivery companies. The algorithms we used were Sequential Model, GaussianNB Model, Naive Bayes Classifier,  Decision Tree Classifier, Random Forest Classifier, Extra Trees Classifier, KNeighbors Classifier, SVM Model, Logistic Regression, AdaBoost Classifier. The best score we achieved was by using the Sequential Model with Accuracy = 0.76%.


## Time Frame <a name="Time-Frame"></a>

The project took around 4 weeks of work and the deadline was on the 14th of May. The data collection time was from September 2019 to April 2020.


## Conclusion <a name="Conclusion"></a>

In conclusion, we used multiple data cleaning and EDA techniques to analyze and visualize our dataset. We seek to measure the customer’s satisfaction ratio before and after the COVID-19 for Marsol and Hungerstation delivery companies in Saudi Arabia. We came to, that before COVID-19, Marsol customer satisfaction was 49% and Hungerstation had 23%, so we can say that Marsol customer satisfaction was better. After COVID-19, Marsol shows 40% of customer satisfaction and on the other hand, Hungerstation had 21%, in that we can say that also after COVID-19 pandemic Marsol steel better. Finally, we applied multiple machine learning algorithms, the best score we achieved was by using a Sequential Model with Accuracy = 0.76%.


## Future Work <a name="Future-Work"></a>
- Completion of the project requires an increase in the time period after COVID-19.
- Improve the accuracy of our model.
- Include more companies, especially the new companies that appeared during COVID-19.


## Reference <a name="Reference"></a>
- https://www.aziz-blog.com/?p=10615
- https://github.com/sarah66679/US-gasoline
- https://www.youtube.com/watch?v=xYhDQFnlBko
- https://monkeylearn.com/text-classification/
- https://www.scrapehero.com/marketplace/apis/
- http://adilmoujahid.com/posts/2014/07/twitter-analytics/
- https://jovianlin.io/keras-models-sequential-vs-functional/
- https://www.kaggle.com/ragnisah/text-data-cleaning-tweets-analysis
- https://www.geeksforgeeks.org/twitter-sentiment-analysis-using-python/
- https://www.kaggle.com/gunesevitan/nlp-with-disaster-tweets-eda-cleaning-and-bert
- https://towardsdatascience.com/sentiment-analysis-for-text-with-deep-learning-2f0a0c6472b5
- https://ipullrank.com/step-step-twitter-sentiment-analysis-visualizing-united-airlines-pr-crisi
- https://machinelearningmastery.com/save-load-keras-deep-learning-models/
- https://www.kaggle.com/ragnisah/text-data-cleaning-tweets-analysis
- http://www.andrewtcrooks.com/2017/06/05/Data_Viz_DiagrammeR_and_wordcloud/
- https://www.earthdatascience.org/courses/use-data-open-source-python/intro-to-apis/calculate-tweet-word-frequencies-in-python/
- https://stackoverflow.com/questions/49384111/reflect-arabic-word-cloud
- https://www.kaggle.com/marcovasquez/basic-nlp-with-tensorflow-and-wordcloud
- https://www.aziz-blog.com/?p=10646
- https://towardsdatascience.com/an-introduction-to-tweettokenizer-for-processing-tweets-9879389f8fe7
- https://github.com/amueller/word_cloud/pull/315
- https://stackoverflow.com/questions/20510768/count-frequency-of-words-in-a-list-and-sort-by-frequency
- https://stackoverflow.com/questions/716477/join-list-of-lists-in-python
- https://stackoverflow.com/questions/22412258/get-the-first-element-of-each-tuple-in-a-list-in-python/22412308
- https://towardsdatascience.com/a-complete-exploratory-data-analysis-and-visualization-for-text-data-29fb1b96fb6a
- https://mode.com/blog/python-data-visualization-libraries/
- https://towardsdatascience.com/nlp-for-beginners-cleaning-preprocessing-text-data-ae8e306bef0f
- https://monkeylearn.com/blog/sentiment-analysis-of-twitter/
- https://www.kaggle.com/kashnitsky/topic-2-visual-data-analysis-in-python
- https://matplotlib.org/3.2.1/gallery/index.html
- https://davidhamann.de/2017/06/26/pandas-select-elements-by-string/
- https://theappsolutions.com/blog/development/sentiment-analysis/
- https://algorithmia.com/blog/introduction-sentiment-analysis
- https://algorithmia.com/blog/introduction-natural-language-processing-nlp
- https://www.analyticsvidhya.com/blog/2018/07/hands-on-sentiment-analysis-dataset-python/
