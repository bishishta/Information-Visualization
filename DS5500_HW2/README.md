# Imformation Visualization [DS 5500] - HW2

## Problem 1:

#### Group for the second project component :

1. Konanki Sai Charan 
2. Manvita Markala
3. Bishishta Mukherjee
4. Romil Rathi

## Problem 2:

## Problem 3:

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

[code under heading Problem5 in the ipython file - DS5500_HW2_code.ipynb]












