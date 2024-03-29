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