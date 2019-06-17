# Prosper Loan Data Exploration
## by Jeffrey Van Anderson


## Dataset

The original dataset used for this explorations consists of 113,937 loan observations from Prosper.  Although the original data set has 81 variable columns, only 11 were used for this analysis.

## Summary of Findings

Through this exploration, I was surprised to find that the five quantitative variables of interest did not have any strong relationship with each other.  I suspect that this is due to an excess of other lurking variables that are of stronger influence.  At the time, this analysis appeared to be a dead end.  As I was particularly interested in Borrower APR, this variable was explored in more detail against qualitative variables during bivariate and multivariate visualization.  I found that there was a quite unusual distribution of borrower APR and compared other variables against this distribution.  

Clearly, there is more to the relationships between variables in this data than I will use in the explanatory presentation.  One I found and did not elaborate on was a difference in each employment status category and borrower APR.  There were clearly differences in these distributions.  Another univariate feature of interest was the original loan amount.  This distribution was concentrated on five specific values.  Perhaps if elaborated on in bivariate analysis, more insights could be drawn.

## Key Insights for Presentation

For the explanatory presentation, the key thread of interest is the relationship between four of the qualitative variables and Borrower APR.  The APR distribution seamed to have a mode value of 0.358.  Through bivariate violin plots, density around this value was identified for the `Term` and `IncomeRange` categories.  When `ListingCategory` and `IsBorrowerHomeowner` were compared  against the other two variables, there was yet another filter.  For those with 12 month loans, it is more likely that one will have a 35.8% interest rate if they are not a homeowner or their loan is for debt consolidation.  Additionally, there does seam to be a negative correlation between Income Range and borrower APR.

In summary, the four qualitative variables described above appear to have an influence on borrower APR.  When the data is viewed as measurements of center, there appears to be an effect on APR distribution.  More people have higher APRs (especially at a 35.8% rate) depending on their income range, reason for a loan, term length and homeowner status.

## Resources used for code reference:

* Python Standard Library: https://docs.python.org/3/library/
* Pandas Library: https://pandas.pydata.org/pandas-docs/stable/
* Matplotlib Library: https://matplotlib.org/api/_as_gen/matplotlib.pyplot.html
* Seaborn Library: https://seaborn.pydata.org/
