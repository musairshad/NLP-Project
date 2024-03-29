# NLP-Project
#### Business Problem
In a world where there are many new technology companies starting up, how people feel about a brand can tell us a lot about whether they'll buy their products. This is important for companies like GoldenGroup that invest in technology. They've asked us to build them a predictive model that can read recent tweets about different technology products and figure out if people like them or not. They want this program to work for all kinds of brands, so they can use it to decide which ones to look into more closely for possible investment. GoldenGroup only cares about whether people feel good about the brand because they think people buy things they like. Here GoldenGroup's objective is determine what type of investments they can make with Apple and google positive tweets.
#### Data Understanding:
The dataset comes from CrowdFlower via data.world. Human raters rated the sentiment in over 8721 Tweets as positive, negative, or neither. The tweets included are sent out during the South by South West conference, mostly about Google and Apple products. The data was put together in 2011.

Tweets are usually short and packed with emotions. They can capture consumer's real time response to a brand very well. South by Southwest showcases all the newest technology and allows consumers to compare the products of major tech companies side by side, which can reduce their biases to some degree.

We engineered our target into two classes: tweets with positive sentiment and tweets with negative sentiment. We only care about whether the tweet is positive because positive emotion drives sales, which can translate into return on investment.

Data Source: https://data.world/crowdflower/brands-and-product-emotions
#### Objective :
- Our objective is to come up with predictive model which has high accuracy of determining positive sentiment tweets.
- Come up with investment options for GoldenGroup from the positive tweets so they can confidently invest in products and services accordingly. 
![Alt Text](https://github.com/musairshad/NLP-Project/blob/main/Images/tweets%20per%20sentiment.png)
#### NLP Analysis
Once the data was processed, we split the information for NLP analysis. Tokenization, removal of stopwords, and Lemmatization took place on the corpus from the dataframe.

Next, a function to identify context around words was used so we could add new items to the stopwords list if necessary. After that, I generated a set of word clouds to look at how sentiment compares between positive & negative tweets as a whole; and another set for either company.

Furthermore, I create more word clouds for the sentiment of tweets categorized by each company for further insight.

Once satisfied, we identified the target column & ran the data through various ML algorithms. Followed by SVC modeling to see if we can get even better results. I also configured each run to return a confusion matrix; classification reports with error scores and ROC curves are displayed on the Scikit-Learn models.
#### Percentage of Sentiment for Apple Related Tweets
![Alt Text](https://github.com/musairshad/NLP-Project/blob/main/Images/apple%20tweet%20sentiment%20by%20percentage.png)
#### Percentage of Sentiment for Google Related Tweets
![Alt Text](https://github.com/musairshad/NLP-Project/blob/main/Images/google%20sentiment%20percentage.png)
Apple and Google has similar Sentiments for for their tweets.
#### Apple Positive word cloud


![Alt Text](https://github.com/musairshad/NLP-Project/blob/main/Images/apple%20cloud%20without%20company.png)

![Alt Text](https://github.com/musairshad/NLP-Project/blob/main/Images/apple%20product%204.png)
We see much excitement for a popup store & its location downtown, which sells the latest products. Words mentioned the most for Apple are Ipad, Apple, Iphone and case.


#### Google Positive word cloud
![Alt Text](https://github.com/musairshad/NLP-Project/blob/main/Images/google%20cloud%20without%20company.png)

![Alt Text](https://github.com/musairshad/NLP-Project/blob/main/Images/google%20product%202.png)
There is much buzz for Google Circle (a social network) in this dataset and Google Maps. We also see much mention of Marissa Mayer, the PR manager for Google.


#### Binary Classification Models
To facilitate readability, I've showcased the top three models below. For additional results, kindly refer to the associated Jupyter notebook within this repository!



##### SVC Tuned Model


![Alt Text](https://github.com/musairshad/NLP-Project/blob/main/Images/tuned%20svc%20confusion.png)

![Alt Text](https://github.com/musairshad/NLP-Project/blob/main/Images/roc%20curve%20tuned%20svc.png)

##### Tuned LogReg model

![Alt Text](https://github.com/musairshad/NLP-Project/blob/main/Images/tuned%20log%20reg%20confusion%20matrix.png)

![Alt Text](https://github.com/musairshad/NLP-Project/blob/main/Images/tuned%20log%20reg%20roc%20curve.png)

##### Tuned RandomForest Classifier
[Alt Text](https://github.com/musairshad/NLP-Project/blob/main/Images/tuned%20random%20forest%20confusion.png)

![Alt Text](https://github.com/musairshad/NLP-Project/blob/main/Images/tuned%20random%20forest%20roc%20curve.png)

#### Recommendations
- We recommend Svc tuned model which has a Recall score of 1.0 for positive sentiment tweet and accuracy score and precision score of 85.6. 
- One of the most used words was 'New', 'Case' for Apple, 'phone' and 'tablet' for google so GoldenGroup can invest in Accessories company for Iphone, Ipad and google products.
- GoldenGroup also has an opportunity of investing in event planner companies for Apple and Google as they both have positive feedback from users about events






