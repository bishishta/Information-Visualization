# Information Visualization [DS 5500] - HW4

## Problem 1:

#### Proportion of each district’s total funding that will be lost:

![Proportion of each district’s total funding that will be lost []{label="histogram"}](solution_figures/prob1.png)
###### Figure 1: Histogram showing distribution of school district according to proportion of total revenue cut range

![Proportion of each district’s total funding that will be lost []{label="histogram"}](solution_figures/prob1_boxplot.png)
###### Figure 2: Distribution of proportion of total funding to be cut for school districts with budget cut

According to the budget criteria adopted in HW3 - Problem 4, only 1352 school districts out of 16539 schools (obtained after pre-processing of fiscal data) will suffer from budget cut, that is, 15187 school districts will receive total revenue as before suffering from no budget cuts. Therefore, we can see a huge number of school districts falling under the first bar in figure 1. To better visualize the distribution of proportion of total funding to be cut for districts suffering from budget cut, a boxplot is also drawn (figure 2). From figure 2, we see that 75% of the school districts suffering budget cut, endure a deduction of less than 3% of the total revenue, which is pretty low.

#### Top 10 districts that will be affected by the budget cuts the most:

![Top 10 districts that will be affected by the budget cuts the most []{label="table"}](solution_figures/prob1_table.png)
###### Figure 3: Districts that will be affected by the budget cuts the most

[code under heading Problem 1 in the ipython file - DS5500_HW4_code.ipynb]

## Problem 2:

![distribution of proportion of enrolled students by race for all school districts []{label="boxplot"}](solution_figures/prob2.png)
###### Figure 4: Distribution of proportion of enrolled students by race for all school districts

![distribution of proportion of enrolled students by race for school districts with budget cut []{label="boxplot"}](solution_figures/prob2_budget_cut.png)
###### Figure 5: Distribution of proportion of enrolled students by race for school districts with budget cut

![distribution of proportion of enrolled students by race for school districts with no budget cut []{label="boxplot"}](solution_figures/prob2_no_budget_cut.png)
###### Figure 6: Distribution of proportion of enrolled students by race for school districts with no budget cut

As seen for figure 4, races: Black, Hispanic and Asian are amongst the minority races when compared to White which predominantly constitutes the majority proportion of enrolled children in all school districts. Furthermore, a careful look at figure 5 and figure 6, reveals that the criteria adopted for budget cut, generated an almost similar distribution to that of figure 4. However, the selection method demonstrates a partial hidden bias and thus, the school districts for whom the budget was deducted contained a higher proportion of children from the minority races: Black, Hispanic and Asian and a lesser proportion of White when compared to school districts for whom the budget was not deducted.

[code under heading Problem 2 in the ipython file - DS5500_HW4_code.ipynb]

## Problem 3:

![distribution of proportion of enrolled students by disability for all school districts []{label="boxplot"}](solution_figures/prob3.png)
###### Figure 7: Distribution of proportion of enrolled students by disability for all school districts

![distribution of proportion of enrolled students by disability for school districts with budget cut []{label="boxplot"}](solution_figures/prob3_budget_cut.png)
###### Figure 8: Distribution of proportion of enrolled students by disability for school districts with budget cut

![distribution of proportion of enrolled students by disability for school districts with no budget cut []{label="boxplot"}](solution_figures/prob3_no_budget_cut.png)
###### Figure 9: Distribution of proportion of enrolled students by disability for school districts with no budget cut

Figure 8 and figure 9 have a similar distribution as that of figure 7, that is the same as original data. However, a careful look at figure 8 shows that the criteria adopted for budget cut included a partial hidden bias towards disabled children and thus, the school districts for whom the budget was deducted contained lesser proportion of disabled children when compared to school districts for whom the budget was not deducted. Although, the mentioned difference can only be seen in the outliers.

[code under heading Problem 3 in the ipython file - DS5500_HW4_code.ipynb]

## Problem 4:

##### Link to choice of fellow classmates’ selection of schools for budget cuts in HW 3 Problem 4 and Problem 5 - https://github.com/Omairss/ds5500-hw3

##### The approach and justification of selection: 
Approach adopted was first sorting the school districts by their respective per capita spending and then deducting 20% from the top n, till the total federal budget to be cut was achieved. Justification provided was that this method saves 15,000 districts from budget cuts.

##### Advantages of the approach: 
As mentioned in the justification provided, the very first advantage is that this method saves majority of the school districts from budget cut. Secondly, it does not deduct the budget of any school district based on the performance of students, which according to me would have been unjustified because the capabilities of students does not serve as a fair ground for budget allocation in any case and if still considered as one, might hamper the learning and performance of students in a negative way irrespective of the previous performance status, which is not good for any school district.

##### Disadvantages of the approach:
This method deducts 20% budget from the school districts with most per capita spending which could be a huge deduction for the considered school districts since they already have the highest per capita spendings. Also, this method does not take into account if the considered school districts have enough funding coming in from other sources like state and local or how much debt does the considered school districts have to pay. 

## Problem 5:

#### Summarization of the learnings from the lecture on Visualization by Steven Braun

As a data science student, I found this lecture to be most interesting and informative. Visualization is an utmost important task in every step of any data science task whether be it finding patterns, hidden biases, distribution, outliers, etc. in the data exploration and pre-processing step or presenting the findings obtained after applying any model or be it comparing the performance of various models for the same task. Steven covered various important aspects of visualization and demonstrated that how the amount of information conceived by an audience from a visualization is deeply impacted by very subjective topics like the choice of proper kind of plot/graph/table, choosing appropriate color palette, hue, saturation and luminance, proper scaling and providing proper label, legend, title at proper positions. Moreover, he taught how to incorporate contextual clues with shapes and designs. He also explained the difference between dynamic and static visualizations. The most important piece of information provided by him was that although dynamic visualizations appear more advantageous and appealing in theory but in professional world, more knowledge is leveraged to a non-technical user or customer from a static visualization. Overall, the golden rule is that graphs need not be complicated but minimal, readable and interpretable and should empower the concerned audience type by addressing their needs and conveying them all the information they want to know.
