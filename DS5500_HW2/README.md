# Imformation Visualization [DS 5500] - HW2

## Problem 1:

#### Group for the second project component :

1. Konanki Sai Charan 
2. Manvita Markala
3. Bishishta Mukherjee
4. Romil Rathi

## Problem 2:

Below I have discussed the visualization presented by Omair Shafi Ahmed for HW 1 Problem 2 (distribution of income across countries and continents over time).
Link to the original solution : https://github.com/Omairss/ds5500_hw1/blob/master/Homework1.ipynb

Visualization description: Omair has used a heat map and a stacked plot to show the distribution of income across countries over time.

Similarity to mines? It is similar to mines in the term that we both have used static plots but the choice of plots are very different. I have chosen line plots for the same.

Easy to interpret? Does it effectively visualize what is being asked? Why or why not?
I really liked the unique choice of heat map here. Given the huge number of countries in the dataset, line plot makes it quite clumsy to study the pattern of income change over the years for each of the individual country using a single plot but here the color coding makes it very easy to observe at a glance, the change in pattern or any unique behaviour for any particular country. However, searching for a particular country would have been easier if country abbreviations would have been replaced by the country name.
In my opinion, using stacked plot to visualize the changing income distributions across countries over time was not a wise choice since here the total number of countries are more than the maximum unique colors available in the plot’s color palette. Therefore, as can be seen from the legend of the stacked plot, multiple countries are represented by the same color which makes it difficult to study and interpret the plot distinguishably. It would have been a perfect choice to visualize the changing income distributions across ‘continents’ over time since there are just 4 or 6 continents.

## Problem 3:

Below I have discussed the visualization presented by Omair Shafi Ahmed for HW 1 Problem 3 (relationship between income, life expectancy, and child mortality over time).
Link to the original solution : https://github.com/Omairss/ds5500_hw1/blob/master/Homework1.ipynb

Visualization description: Omair has used Seaborn’s Pairgrid plot to show the relationship between income, life expectancy, and child mortality over time.

Similarity to mines? Again, it is similar to mines in the term that we both have used static plots but the choice of plots are very different. I have chosen line plots for the same.

Easy to interpret? Does it effectively visualize what is being asked? Why or why not?
Yet again, I really liked the unique choice of plot here and in my opinion, the plot very efficiently shows the distribution of each of the individual terms over time and the relationship amongst the three at the same time. The choice of interactive plots here makes it difficult for the users to retain and establish a clear relation between the three as well as distrubution over time for any of the three at a glance. Also, this plot very clearly conveys what proportion of the total countries in the world had the income, life expectancy or child mortality values in a particular range for a particular year. However, to study all of the above-mentioned things for a particular continent or making comparisons across continents, the points in the pairgrid can be colored based on continents. 

## Problem 4:

#### Baseline model -  Response variable : Y ->  Life Expectancy and Predictor variables : X1 -> Income, X2 -> Year
#### Final model -  Response variable : Y ->  Life Expectancy and Predictor variables : X1 -> log(Income), X2 -> Year

##### Comparing the linearity between the response variable and each of the predictor variables :

![Baseline : comparing the linearity between the response variable and each of the predictor variables []{label="fig:pairplot"}](solution_figures/q4_baseline_pair_plot.png)
###### Figure 1: pair-plot for baseline model

![Final : comparing the linearity between the response variable and each of the predictor varables []{label="fig:pairplot"}](solution_figures/q4_pair_plot.png)
###### Figure 2: pair-plot for final model

Existence of linear relationship between the response variable and each of the predictor variables is one of the core assumptions to fit a linear regression model. But as is evident from figure 1 that a linear relationship doe not exist between life expectancy and income [GDP per capita]. Hence, the assumption is violated by the baseline model, whereas it is clearly followed in the pair-plots for the final model, as can be seen in figure 2.

##### Comparing the R-squared value between the two models :

![comparing the R-squared value between the two models []{label="chart"}](solution_figures/q4_stats.png)
###### Figure 3: baseline and final model statistics

Higher the R-squared value, better the model because it means that more variance is explained by the model. As can be seen in the figure 3, the baseline model has a R-squared value of 0.440 and the final model has a R-squared value of 0.703. Hence, the later is a better model.

##### Final model parameters :

As can be seen from the p-value of all the terms in figure 3, all the terms are significant. The intercept and co-efficient estimates obtained for the final model are:

![Final model parameters []{label="chart"}](solution_figures/q4_params.png)

Hence the model fitted is : Y1 = -350.49 + 4.759X1 + 0.189X2, 
where Y1 = Life Expectancy, X1 = log(Income), X2 = Year

##### Impact of autocorrelation of time series on analysis:

Autocorrelation of time series exists when there is a correlation of the time series with it’s own lagged version. It might be useful in some of the problems of technical analysis, such as, predicting if there is a momentum factor associated with a stock. However, an underlying assumptions of regression analysis is that data has no autocorrelation. If not so, autocorrelation increases the variance of the coefficient estimates and hence deflates the size of estimated standard error. The F-statistic, R2, and adjusted R2 may not be accurate either. Additionally,  when the autocorrelation comes from a missing independent variable, the coefficient estimates will be biased. This makes the results obtained by the model very unclear, misleading and in some cases meaningless. 

[code under heading Problem4 in the ipython file - DS5500_HW2_code.ipynb]

## Problem 5:

#### Baseline model -  Response variable : Y -> Child Mortality Rate and Predictor variables : X1 -> Income, X2 -> Year
#### Final model -  Response variable : Y -> log(Child Mortality Rate) and Predictor variables : X1 -> log(Income), X2 -> Year

##### Comparing the linearity between the response variable and each of the predictor variables :

![Baseline : comparing the linearity between the response variable and each of the predictor variables []{label="fig:pairplot"}](solution_figures/q5_baseline_pair_plot.png)
###### Figure 4: pair-plot for baseline model

![Final : comparing the linearity between the response variable and each of the predictor varables []{label="fig:pairplot"}](solution_figures/q5_pair_plot.png)
###### Figure 5: pair-plot for final model

Existence of linear relationship between the response variable and each of the predictor variables is one of the core assumptions to fit a linear regression model. But as is evident from figure 4 that a linear relationship doe not exist between child mortality rate and income [GDP per capita]. Hence, the assumption is violated by the baseline model, whereas it is clearly followed in the pair-plots for the final model, as can be seen in figure 5.

##### Comparing the R-squared value between the two models :

![comparing the R-squared value between the two models []{label="chart"}](solution_figures/q5_stats.png)
###### Figure 6: baseline and final model statistics

Higher the R-squared value, better the model because it means that more variance is explained by the model. As can be seen in the figure 6, the baseline model has a R-squared value of 0.378 and the final model has a R-squared value of 0.808. Hence, the later is a better model.

##### Final model parameters :

As can be seen from the p-value of all the terms in figure 6, all the terms are significant. The intercept and co-efficient estimates obtained for the final model are:

![Final model parameters []{label="chart"}](solution_figures/q5_params.png)

Hence the model fitted is : Y1 = 61.025 - 0.626X1 + 0.026X2, 
where Y1 = log(Child Mortality Rate), X1 = log(Income), X2 = Year

##### Impact of autocorrelation of time series on analysis:

Autocorrelation of time series exists when there is a correlation of the time series with it’s own lagged version. It might be useful in some of the problems of technical analysis, such as, predicting if there is a momentum factor associated with a stock. However, an underlying assumptions of regression analysis is that data has no autocorrelation. If not so, autocorrelation increases the variance of the coefficient estimates and hence deflates the size of estimated standard error. The F-statistic, R2, and adjusted R2 may not be accurate either. Additionally,  when the autocorrelation comes from a missing independent variable, the coefficient estimates will be biased. This makes the results obtained by the model very unclear, misleading and in some cases meaningless. 

[code under heading Problem5 in the ipython file - DS5500_HW2_code.ipynb]
