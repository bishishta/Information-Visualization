# Imformation Visualization [DS 5500] - HW4

## Problem 1:

#### Proportion of each district’s total funding that will be lost:

![Proportion of each district’s total funding that will be lost []{label="histogram"}](solution_figures/prob1.png)
###### Figure 1: Histogram showing distribution of school district's according to total revenue cut range

![Proportion of each district’s total funding that will be lost []{label="histogram"}](solution_figures/prob1_boxplot.png)
###### Figure 2: Distribution of proportion of total funding to be cut for school districts with budget cut

According to the budget ctriteria adopted in HW3 - Problem 4, only 1352 school districts out of 16539 schools (obtained after pre-processing of fiscal data) will suffer from budget cut, that is, 15187 school districts will recieve total revenue as before suffering from no budget cuts. Therefore, we can see a huge number of school districts falling under the first bar in figure 1. To better visualize the distribution of proportion of total funding to be cut for districts suffering from budget cut, a boxplot is also drawn (figure 2). From figure 2, we see that 75% of the school districts suffering budget cut, endure a deduction of less than 3% of the total revenue, which is pretty low.

#### Top 10 districts that will be affected by the budget cuts the most:

![Top 10 districts that will be affected by the budget cuts the most []{label="table"}](solution_figures/prob1_table.png)
###### Figure 3: Districts that will be affected by the budget cuts the most

[code under heading Problem 1 in the ipython file - DS5500_HW4_code.ipynb]

## Problem 2:

![distribution of proportion of enrolled students by race for all school districts []{label="boxplot"}](solution_figures/prob2.png)
###### Figure 4: Distribution of proportion of enrolled students by race for all school districts

![distribution of proportion of enrolled students by race for school districts with budget cut []{label="boxplot"}](solution_figures/prob2_budget_cut.png)
###### Figure 5: Distribution of proportion of enrolled students by race for school districts with budget cut

![distribution of proportion of enrolled students by race for school districts with no budget cut []{label="boxplot"}](solution_figures/prob2_no__budget_cut.png)
###### Figure 6: Distribution of proportion of enrolled students by race for school districts with no budget cut

As seen for figure 4, races: Black, Hispanic and Asian are amongst the minority races when compared to White who predominantly constitue the majority proportion of enrolled children in all schol districts. Furthermore, a careful look at figure 5 and figure 6, reveals that the criteria adopted for budget cut, generated an almost similar distribution to that of figure 4. However, the selection method demonstrates a partial hidden bias and thus, the school districts for whom the budget was deducted contained a higher proportion of children from the minority races: Black, Hispanic and Asian and a lesser proportion of White when compared to school districts for whom the budget was not deducted.

[code under heading Problem 2 in the ipython file - DS5500_HW4_code.ipynb]

## Problem 3:

![distribution of proportion of enrolled students by disability for all school districts []{label="boxplot"}](solution_figures/prob3.png)
###### Figure 7: Distribution of proportion of enrolled students by disability for all school districts

![distribution of proportion of enrolled students by disability for school districts with budget cut []{label="boxplot"}](solution_figures/prob3_budget_cut.png)
###### Figure 8: Distribution of proportion of enrolled students by disability for school districts with budget cut

![distribution of proportion of enrolled students by disability for school districts with no budget cut []{label="boxplot"}](solution_figures/prob3_no__budget_cut.png)
###### Figure 9: Distribution of proportion of enrolled students by disability for school districts with no budget cut

Figure 8 and figure 9 have a similar distribution as that of figure 7, that is the same as original data. However, a careful look at figure 8 shows that the criteria adopted for budget cut included a partial hidden bias towards disabled children and thus, the school districts for whom the budget was deducted contained lesser proportion of disabled children when compared to school districts for whom the budget was not deducted. Although, the mentioned difference can only be seen in the outliers.

[code under heading Problem 3 in the ipython file - DS5500_HW4_code.ipynb]

## Problem 4:



## Problem 5:

