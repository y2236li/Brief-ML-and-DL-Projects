<a name="backtotop"></a>
# Project List
- [Build NN from strach - Computer Vision](#buildNNfromstrach)<br>
- [Marketing Funnel Analysis By Olist](#MarketFunnel)<br>
- [Using News to Predict Stock Market](#NewsStockMarket)<br>


___

## Build NN from strach - Computer Vision<a name="buildNNfromstrach"></a>
[back to top](#backtotop)

The program is building a simple Neural Network without any deep learning package


> 1. Include a dummuy variable value of which is one throughout all sample points so that we can get intercept value
> 2. Assign random weight to each of the variables and make prediction using dot product of the random weight and variable values
> 3. Using a cost function (cross entropy for example) to compute the loss of the target observations.
> 4. Calculate the derivatives of the cost function with respect to the weight and the bias
> 5. Update the weight and bias by mutiplying the weight and bias derivatives with learning rate
> 6. Iterate step 4 and 5 until the change in weights is insignificant 

Tutorial Link: https://towardsdatascience.com/step-by-step-guide-to-building-your-own-neural-network-from-scratch-df64b1c5ab6e
<br>

**Conclusion:**<br>

> The model achieved 99% accuracy on training data and 70% on testing data

___

## Marketing Funnel Analysis<a name="MarketFunnel"></a>
[back to top](#backtotop)

Notice: The Following text are refered from https://www.kaggle.com/olistbr/marketing-funnel-olist/home

The dataset has information of 8k Marketing Qualified Leads (MQLs) that requested contact between Jun. 1st 2017 and Jun 1st 2018. They were randomly sampled from the total of MQLs.

Its features allows viewing a sales process from multiple dimensions: lead category, catalog size, behaviour profile, etc.

This is real data, it has been anonymized and sampled from the original dataset.

___

## Using News to Predict Stock Market<a name="NewsStockMarket"></a>
[back to top](#backtotop)

The project aims to predict daily rising/dropping trending of Dow Jones Industrial Average(AJIA) by news headlines. In other words, this is a binary classification NLP project

**News data** is crawled from Reddit WorldNews Channel 

**DJIA data** is downloaded from Yahoo Finance 


**The following models are applied and their accuracy:**
> 1. 61% -- Logistic Regression<br>
> 2. 55% -- Multinomial Naive Bayes<br>
> 3. 52% -- Random Forest<br>
> 4. 54% -- Gradient Boosting Machines<br>
> 5. 52% -- Naive Bayes SVM<br>
> 6. 56% -- Multilayer Perceptron Neural Network(MLP)<br>
> 7. 55% -- LSTM Neural Network<br>
> 8. 55% -- Bidirectional LSTM Neural Network<br>
> 9. 54% -- Convolutional Neural Network<br>
___
## Lunar Lander Deep Q Learning
[back to top](#backtotop)

The project aims to train a lander to land on a pad by deep q learning

The lander at the beginning:
<a href="https://imgflip.com/gif/3gnzww"><img src="https://i.imgflip.com/3gnzww.gif" title="made at imgflip.com"/></a>

After Training:
<a href="https://imgflip.com/gif/3go36o"><img src="https://i.imgflip.com/3go36o.gif" title="made at imgflip.com"/></a>

Tutorial Link: https://github.com/philtabor
