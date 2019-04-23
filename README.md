# ML_Project4

## Part 1 - Business Case

Can a stock's value be predicted with an acceptable error from past stock exchange data if enough data is provided?

This is obviously a very interesting topic for the world in general, and not only for people who like working with data. Having a working version of this algorithm in the real world would mean infinite financial gain, which everyone would immediately be interested in. Moving past that, this provides us, as a team, with getting closer to the subject of stocks, in general, and how trading works. We hope that by analyzing this data we might gain a better insight in how stock functions holistically.

This dataset provides is applying everything that we have learned in class in how to approach a problem of this type. How to think about designing the algorithm, applying normalization and curation techniquest on the dataset, ways of splitting the dataset in training our model, and then how we go about evaluating our results. Besides just going over what we have done in class again, we think this is a good opportunity to try our hand at something a bit more complex and maybe out of curriculum, but definitely very interesting, namely a LSTM (Long Short Term Memory) model. We will probably be building something basic in that regard, but it will serve the purpose of teaching us how it works underneath.

## Part 2 - Data

Link: https://www.kaggle.com/borismarjanovic/price-volume-data-for-all-us-stocks-etfs#Data.zip

Our dataset may not describe too many features, but they are very descriptive, and a lot of times we end up dropping features that are not correlated anyway, so this may be to our advantage. The features are as follows: Date, Open, High, Low, Close, Volume, OpenInt.

On the side of how many rows we have, the CSV is quite huge, and that will definitely help us.

## Part 3 - Data content and format
