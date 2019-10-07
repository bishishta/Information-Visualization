# Imformation Visualization [DS 5500] - HW1 Visualization and Analysis

## Problem 1:

#### Gapminder test : 

Score received - 46%. 

Answer to a question that startled me the most - The answer being 9 years to the question : 30 years of men have spent 10 years in school on average, how many years have women of the same age spent in school. I thought there would be a huge gap in the two numbers since the issue of girl child being deprived of education is so common all over the world but the correct answer here being so close was surprising.

#### Original question : where does the majority of the world population live?
#### Question re-stated : Which income group does the majority of the world population belong to ?

![Pie chart for distribution of world population into income groups []{label="fig:piechart"}](solution_figures/prob1.png)

As can be seen from the pie chart, a very large portion of the world population(69.9%) belongs to middle income countries as compared to high income countries (17.1%) and low  income countries(13.1%).

[code under heading Problem1 in the ipython file - DS5500_HW1_code.ipynb]

## Problem 2:

#### Distribution of income (GDP / capita) across countries over time :

![Distribution of income (GDP / capita) across countries over time []{label="fig:linegraph"}](solution_figures/prob2_combined2.png)
![Distribution of income (GDP / capita) across countries over time []{label="fig:linegraph"}](solution_figures/prob2_combined_1.png)
![Distribution of income (GDP / capita) across countries over time []{label="fig:linegraph"}](solution_figures/prob2_combined3.png)

1. Majority of the countries have shown an overall rise in the GDP per capita over time with some exhibiting a downfall too.
2. The most interesting case being that of United Arab Emirates [1st row, 1st column plot]. During the late 1970s to late  1990s, when most countries had very less GDP per capita, it had an exceptionally high GDP per capita but decreased sharply over time while others increased.
3. In the present times Luxembourg[4th row, 2nd column plot] and Norway [5th row, 2nd column plot] has a very good and strong GDP per capita as compared to other countries while most of the African countries like Uganda, Zambia and Zimbabwe [last plot] has had very very low GDP since always.

#### Distribution of income (GDP / capita) across continents over time :

![Distribution of income (GDP / capita) across continents over time []{label="fig:linegraph"}](solution_figures/prob2_continents.png)

1. In all the four continents, GDP per capita has shown a rise over the time, the rates being different for each continent.
2. Africa has always had a very weak GDP per capita and a very weak rate of growth as well when compared to other continents since always and not changing much over time.
3. Europe has always had the highest GDP per capita and a very strong rate of growth than other continents and has overall increased tremendously from 1960 with short downfall in the early 1990’s.
4. Asia and America have closely followed each other in terms of GDP per capita, with Asia taking over from around 1975 to 1985 and then again since around 2015. 

[code under heading Problem2 in the ipython file - DS5500_HW1_code.ipynb]

## Problem 3:

#### Investigating the overall relationship between income (GDP / capita), life expectancy, and child mortality overall and within each continent over time :

![Investigating the overall relationship between income (GDP / capita), life expectancy, and child mortality []{label="fig:linegraph"}](solution_figures/prob3_overall.png)
![Investigating the overall relationship between income (GDP / capita), life expectancy, and child mortality []{label="fig:linegraph"}](solution_figures/prob3_overall_continents.png)

As can be seen in the graphs above, overall as well as within all the continents, life expectancy and GDP per capita grow in the same direction while the child mortality rate grow in the opposite direction that the two. The first two phenomenon have shown a rise, while the latter decreased over the time.
To investigate the phenomenon further, let’s look at the following visualizations :

#### Change in income (GDP / capita) over time within each continent :

![Change in income (GDP / capita) over time within each continent []{label="fig:linegraph"}](solution_figures/prob3_gdp_continents.png)

1. Africa always had a very week gap per capita as compared to other continents since always and not changing much over time.
2. Europe has always had the highest GDP per capita than other continents and has overall increased from 1960 with short downfall in the early 1990’s.
3. Asia and America have closely followed each other in terms of GDP per capita, with Asia taking over from around 1975 to 1985 and then again since around 2015. 

#### Change in life expectancy over time within each continent :

![Change in life expectancy over time within each continent []{label="fig:linegraph"}](solution_figures/prob3_life_expectancy_continents.png)

1. For each of the continent, the life expectancy has increased tremendously from 1800’s to the present.
2. Life expectancy was around 30-35 years in all the continents in the early 1800’s, remained almost constant until the late1910’s and in the early 1920’s saw an unusually sharp decrease  followed by an equally sharp increase [ this could possibly be an outlier in the data ]. After that not has tremendously increased over the time with around 65-80 years of life expectancy currently.
3. Europe always had the highest life expectancy, closely followed by America, with America taking over only for a short period from around 11940 to 1945.
4. Till around 1925, Asia had the lowest life expectancy, after that Africa has the lowest life expectancy.

#### Change in child mortality over time within each continent :

![Change in child mortality over time within each continent []{label="fig:linegraph"}](solution_figures/prob3_child_mortality_continents.png)

1. For each of the continent, the child mortality rate has decreased tremendously from 1800’s to the present (almost by 100%).
2. Asia had the highest child mortality in the early 1800’s, closely followed by Africa but run current times Africa has taken over Asia in terms of child mortality rate.
3. Europe has constantly maintain its status of being the continent with the lowest child mortality rate
4. The decrease in child mortality rate in all the continents were not so sharp till the late 1800’s. From around the early 1900’s the fall is very steep.
5. If the same trend continues, soon there will be close to 0 child mortality rate in all continents.

Overall, Europe is a strong continent in terms of income (GDP / capita), life expectancy, and child mortality and Africa is the weakest continent in terms ofincome (GDP / capita), life expectancy, and child mortality over time

[code under heading Problem3 in the ipython file - DS5500_HW1_code.ipynb]


## Problem 4:

Variables chosen :
      1) access to basic sanitation
      2) maternal death 

#### Investigating the overall relationship between access to basic sanitation and maternal death over time :

![Investigating the overall relationship between access to basic sanitation and maternal death  over time []{label="fig:linegraph"}](solution_figures/prob4_overall.png)

1. As can be seen from the plot, access to basic sanitation is inversely proportional to the number of maternal deaths occurring. As the access to basic sanitation increases, the number of maternal deaths fell sharply. Hence, access to basic sanitation is an utmost important factor in controlling the number of maternal deaths from increasing.
2. Over the years, access to basic sanitation has increased by almost 7.5% overall.
3. Over the years, the number of maternal deaths has decreased by almost 35% overall.

#### Investigating the overall relationship between access to basic sanitation and maternal death  over time within each continent :

![Investigating the overall relationship between access to basic sanitation and maternal death  over time []{label="fig:linegraph"}](solution_figures/prob4_continents_combined.png)

1. In the continents of Africa and Asia, there is a decrease in the number of maternal deaths (by almost 22% and 40% respectively) as their access to basic sanitation increased over the years. These continents had a huge number of maternal deaths and poor access to basic sanitation in the early 2000’s. Their situation improved drastically over the years both in  terms of increased access to basic sanitation and decreased  number of maternal deaths.
2. In the continents of America and Europe, the number of maternal deaths were almost 0 and an excellent and well built access to basic sanitation since the early 2000’s itself. They have successfully been able to maintain the same over the years.
3. Hence, a good percentage of access to basic sanitation always ensures the lower number of maternal deaths across the globe.

[code under heading Problem4 in the ipython file - DS5500_HW1_code.ipynb]

## Problem 5:

I used static plots to answer the previous questions.

#### Static visualization :

1. advantages -
      a. This can be used as infographics which can be posted on the web or can be printed as handouts.
      b. More readable and easy to understand when less number of data points to plot or less categories to compare.
      c. Does not require big budget when produced on large scale.

2. disadvantages -
      a. Change in status of a variable cannot easily be reflected dynamically.
      b. Does not give users the leverage to play around with different variables and explore them.
      c. CanNOT represent different relationships and distributions in one plot.
      
#### Dynamic visualization :

1. advantages -
      a. This can be used only over the web as applications.
      b. More readable and easy to understand when huge number of data points or huge number of categories to compare.
      c. Change in status of a variable can easily be reflected dynamically.
      d. Interactive with the user. Does not give users the leverage to play around with different variables and explore them.
      e. Is multilayered, can represent different relationships and distributions in one plot.
      

2. disadvantages -
      a. Requires big budget to be produced on a large scale.
      b. Cannot be printed as handouts.













