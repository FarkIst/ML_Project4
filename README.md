# ML_Project4

## Part 1 - Business Case

Can a stock's value be predicted with an acceptable error from past stock exchange data if enough data is provided?

This is obviously a very interesting topic for the world in general, and not only for people who like working with data. Having a working version of this algorithm in the real world would mean infinite financial gain, which everyone would immediately be interested in. Moving past that, this provides us, as a team, with getting closer to the subject of stocks, in general, and how trading works. We hope that by analyzing this data we might gain a better insight in how stock functions holistically.

This dataset provides is applying everything that we have learned in class in how to approach a problem of this type. How to think about designing the algorithm, applying normalization and curation techniquest on the dataset, ways of splitting the dataset in training our model, and then how we go about evaluating our results. Besides just going over what we have done in class again, we think this is a good opportunity to try our hand at something a bit more complex and maybe out of curriculum, but definitely very interesting, namely a LSTM (Long Short Term Memory) model. We will probably be building something basic in that regard, but it will serve the purpose of teaching us how it works underneath.

## Part 2 - Data

Link: https://www.kaggle.com/borismarjanovic/price-volume-data-for-all-us-stocks-etfs#Data.zip

Our dataset may not describe too many features, but they are very descriptive, and a lot of times we end up dropping features that are not correlated anyway, so this may be to our advantage. The features are as follows: Date, Open, High, Low, Close, Volume, OpenInt.

On the side of how many rows we have, the CSV is quite huge, and that will definitely help us.
Not only that, but the dataset contains data for all US-based stocks and ETFs trading on the NYSE, NASDAQ, and NYSE MKT.
This means that the substance of the dataset is very high, and very relatable to us; based on what we would like to work and end up with in relation to our Business Case. 

## Part 3 - Data content and format

The data provides us with insight on the stock's values with dates. This can be very useful if we decide to get inspired by the Elliot Wave Theory, which in essence states that stocks are traded in repetitive patterns. However stock price or movement prediction is an extremely difficult task, and the currently available models still require supervision. 

For this case LSTM models are the most efficient.
Long Short Term Memory-Networks or LSTMs are a special kind of Recurrent Neural Networks, meaning that their behaviour is naturally persistent with storing past data and use that for future results. An example would be; to predict what kind of event is going to occur at every point in a movie. Traditional Neural Networks would have an unclear understanding on how to predict future events based on past events. RNNs or Recurrent Neural Networks which implies LSTM-models as well, adress this issue. This is because they function in loops to create this long-term persistance in data, since they work as a chain of repeating modules. 

There's a lot of cool and very interesting information of how these models work, but for this step we're going to keep it relatively simple and broad, thus when giving it a second thought it makes sense to use LSTM's for our features(listed below), that we're going to DataMine in the near future with the use of our models.  

List of features we're going to be working with, includes: Date, Low, High, Open, Close & Volume. 
* Date: The Data that we're going to be exploring is sorted by Date. This is due to that the order of which the data is presented is crucial in Time Series Modelling - That we will make use of. 

* Low & High: Essentially meaning the Lowest price of a certain stock within the day and respectively the highest stock price within the day. This feature is naturally going to be useful for our project to help training our models, to identify certain patterns or trends that might occur within the daily progress of certain stock/s. 

* Close: Meaning the final price in which either an equity or debt is being traded on a given trading day. The closing value represent an up-to-date estimation of a certain investment untill the next trading day commences. This will act as giving us certain "checkpoints" or markers for how the stock develops which will further improve the prediction of the stock. 

* Volume: Volume determines the amount of sales that has occured for a given stock or the market overall, in a period of time. This is a logical feature to include in our processes, since it determines a rise or decrease in trading activity for the market and specific stock/s, hence giving a prediction on which stocks may increase or decrese investor-interest. 
