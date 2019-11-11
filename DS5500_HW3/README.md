# Imformation Visualization [DS 5500] - HW2

## Problem 1:

#### Federal funding assigned to each state:

![federal funding assigned to each state []{label="bargraph"}](solution_figures/Q1_FFPS.png)
###### Figure 1: Federal Funding assigned to each state

As seen from figure 1, the state which takes in the most federal revenue is California, followed by Texas, New York, Florida and Illinois while Vermont gets the least federal funding amongst all the U.S states, followed by Wyoming, North Dakota, Delaware and New Hampshire.

#### Federal funding spent per student for each state:

![Federal funding spent per student for each state []{label="bargraph"}](solution_figures/Q1_FFPSPS.png)
###### Figure 2: Federal funding spent per student for each state

As seen from figure 2, the state which spends the most federal funding per student is District of Columbia, followed by Alaska, Louisiana, New Mexico and South Dakota.

[code under heading Problem 1 in the ipython file - DS5500_HW3_code.ipynb]

## Problem 2:

#### Relationship between school districts’ total revenue and total expenditures:

![relationship between school districts’ total revenue and expenditures []{label="correlationplot"}](solution_figures/Q2_correlation.png)
###### Figure 3: Correlation plot between school districts’ total revenue and total expenditures

As seen from figure 3, there exists a strong positive correlation between total revenue and total expenditures. To verify the relation obtained, the total expenditure for each school ditrict was plotted against the total revenue received [ school districts sorted according to the total revenue].

![total expenditure for each school ditrict against the total revenue received  []{label="lineplot"}](solution_figures/Q2_relationship.png)
###### Figure 4: Total expenditure for each school ditrict against the total revenue received 

As seen from figure 4, more the total revenue received by a school district, more the total expenditure.

#### Debt per student for each state:

![Debt per student for each state []{label="bargraph"}](solution_figures/Q2_DPSFS.png)
###### Figure 5:  Debt per student for each state

As seen from figure 5, South Carolina has the most debt per student, followed by Minnesota, Texas, Pennsylvania and Michigan while Hawaii has the least debt per student followed by Wyoming, West Virginia, Georgia and Vermont.

[code under heading Problem 2 in the ipython file - DS5500_HW3_code.ipynb]

## Problem 3:

#### explaination of the function built for processing a single column of “blurred” metrics into usable numeric values:

1) The column values presented as ranges were replaced by the mean of the range.
2) The column values with 'LT' followed by a number, were replaced by the mean of the range: 0 - number specified.
3) The column values with 'GT' followed by a number, were replaced by the mean of the range: number specified - 100.
4) The column values with 'LE' followed by a number, were replaced by the  75th percentile of the range: 0 - number specified.
4) The column values with 'GE' followed by a number, were replaced by the  25th percentile of the range: number specified - 100.
5) All other column value type (excluding the above-mentioned types and ones containing all digits), like, 'PS', NaN, '.', were replaced by the mean of 0 and 100, that is, 50.

At the end of processing, it was ensured that all the columns values were of type float.

#### Processsing and then visualizing the distribution of the performance metric - Percentage of students in the school that scored at or above proficient in Reading/Language Arts

The raw values of the column containg the info for above-mentioned metrics were processed using the function built and were mapped to the processed values. Unique raw values and unique processed values can be seen in figure 6.

![raw values and processed values of the metric chosen []{label="table"}](solution_figures/Q3_value_table.png)
###### Figure 6:  Table containing the unique raw values and unique processed values of the metric chosen

![Distributionvisualization []{label="histogram"}](solution_figures/Q3_distribution.png)
###### Figure 7:  Visualization of the distribution of the metric chosen.

As can be seen for figure 7, distribution for the percentage of students in the school that scored at or above proficient in Reading/Language Arts follows a gaussian distribution, with almost 3000 school districts having 50 - 60 % students scoring good and approx 10, 000 school districts have more that 50% student scoring at or above proficient while almost an equal number of school districts need to improve and produce good results: more than 50% student score at or above proficient in the future.

[code under heading Problem 3 in the ipython file - DS5500_HW3_code.ipynb]

## Problem 4:

##### Total federal budget allocated before deduction: $55602742000
##### Total federal budget to be deducted: $8340411300.0
##### Total federal budget allocated after deduction: $47262330700.0

##### Table of LEAIDs and the dollar amount by which their federal funding will be cut:

The total revenue assigned to each school district was calculated as the sum of state revenue, federal revenue and local revenue. The LEAIDs were sorted in descending order according to the total revenue . Starting from the schol district receiving the most total revenue, 25% of the federal amount assigned was deducted, till the total amount to be deducted from fedral budget was achieved.

![Revenue deduction []{label="table"}](solution_figures/Q4_revenue_table.png)
###### Figure 8:  Top 25 LEAIDs according to the amount deducted from the federal revenue assigned.

[code under heading Problem 4 in the ipython file - DS5500_HW3_code.ipynb]

## Problem 5:

#### statement for the supervisor justifying the decision on which school districts will lose funding:

The basis of the decision was fair to all the school districts since it makes sure that the ones loosing funding from the federal government are getting enough funds from the other sources (state and local) so that the functioning conitinues to be smooth as before, which would not be possible for the school districts who receive no or very less funds from the other sources. This way just 1351 school districts out of 16539 school districts loose out on funding. 
