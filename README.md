# Regression Discontinuity: Bandwidths, Manipulation and Close Elections

## Objective

I used simulations and close-election data to examine how bandwidth choices and the credibility of the cutoff comparison affect an RD estimate.

## Methodology

- I compared a global quadratic regression with local linear estimates of a grant’s effect.
- I repeated the simulation 300 times and compared bias, variation, and RMSE across bandwidths.
- I tested the running variable’s density for sorting and checked whether a pre-treatment covariate jumped at the cutoff.
- I estimated the difference in congressional voting when a Democrat barely won a House election.
- I fitted local linear RD with triangular weights using weighted least squares and checked the estimate against rdrobust.

## Key Findings

The grant’s true effect was 8 percentage points. The global quadratic estimated +0.0357, while local linear RD estimated +0.0789 at a selected bandwidth of 16.1. Across the repeated simulations, the lowest RMSE on the grid occurred at a bandwidth of 20.

The density test detected manipulation in the data where units moved across the cutoff, with a p-value of 0.0022. The covariate test also detected the jump I planted.

In the House-election data, barely electing a Democrat increased the representative’s adjusted ADA score by 46.491 points. This measures a change in how liberally the district was represented near the election threshold.
