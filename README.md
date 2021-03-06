<a name="backtotop"></a>
# Project List
- [Build NN from strach - Computer Vision](#buildNNfromstrach)<br>
- [Marketing Funnel Analysis By Olist](#MarketFunnel)<br>
- [Using News to Predict Stock Market](#NewsStockMarket)<br>
- [Lunar Lander Deep Q Learning](#LunarLander)<br>
- [Path Finding by Q Learning](#SimpleQLearning)<br>


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
## Path Finding by Q Learning<a name ="SimpleQLearning></a>
[back to top](#backtotop)

This project aims to find an optimal path from a given node to another <br>
Path Visualization: <br>
![PathVisualization](https://github.com/y2236li/Brief-ML-and-DL-Projects/blob/master/Path%20Finding%20by%20Q%20Learning/Path%20Finding%20Visualization.png) <br>

Goal:<br>
**Find the closest route from node 1 to node 7** <br>

Agent State:
> Current Node

Agent Actions:
> Move to transitable adjacent nodes

Agent Reward:
> 100: transition end with the destination node (e.g. R[2, 7] = R[4, 7] = 100)
> 0: If there is a transition between two nodes (e.g. R[0, 1] = R[1, 2] = 0)
> -1: if there is no transition between two nodes (e.g. R[0, 3] = R[6, 4] = -1)

Use **dynamic programming** to random sample and update Q values by <br>
> Q = reward + gamma*max(rewards from the next state) <br>

Output: <1, 2, 7>

___
## Lunar Lander Deep Q Learning<a name="LunarLander"></a>
[back to top](#backtotop)

Goal: <br>
**The project aims to train a lander to land on a pad by deep Q learning** <br>

Agent State:
> Postion of lander: represented by pixel postion and info

Agent Actions:
> 0: Do nothing
> 1: Fire left engine
> 2: Fire down engine
> 3. Fire right engine

Agent Reward:
> 100 - 140 point: Moving from the top of the screen to landing pad and zero speed
> -100 point: Crashes
> 100 point: Comes to rest
> 10 point: Landing on each leg
> -0.3 point: Firing main engine per frame
> 200 point: solved

Agent randomly samples N transition from memory. According to the transition and the rewards in the memory, Agent calculates the corresponding Q values and feeds into a **Two-Layer MLP Neural Network**. The Neural Network will ouput the action by the agent's current state. <br>

Q Formula: <br>
> Q = reward + gamma*max(rewards from the next state) <br>

The lander at the beginning:<br>
<a href="https://imgflip.com/gif/3gnzww"><img src="https://i.imgflip.com/3gnzww.gif" title="made at imgflip.com"/></a> <br>

After Training:<br>
<a href="https://imgflip.com/gif/3go36o"><img src="https://i.imgflip.com/3go36o.gif" title="made at imgflip.com"/></a> <br>

Tutorial Link: https://github.com/philtabor
