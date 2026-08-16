# Decision Log
## Assignment 2: Dataset (2026-07-19)
- Dataset: Player Stats - EPL Serie A from Kaggle
- Main variable of interest: Goals + Assist per 90 because it best describes individual performance and correlates well with other variables such as minutes, team points, and cards.
- Key decision: Organized dataset to identify categorial variables from continuous variables easier.

## Assignment 3: Descriptive Stats (2026-07-26)
- Cleaning done: Removed unneeded or redudant variables such as Minutes %, 90 minutes played, Completed Matches, Goals For, Goals Against, and Net +/- per 90.
- Most surprising pattern: Many outliers due differing player times. We also found it surprising how the majority of the continuous variables are rightly skewed.

## Assignment 4: Probability (2026-07-26)
- Normal vs. empirical, and why: Our distribution assumption for Goals + Assist for 90 held. As for empirical, we had to use COUNTIF/COUNTIFS to calculate empirical probabilities directly from the actual data because our data was right-skewed.

## Assignment 5: Inference (2026-08-09)
- What we tested, alpha, conclusion:

Test 1 — Team Points Per Match: H0: μ ≤ 1.25 vs. Ha: μ > 1.25, α = 0.05. t = 2.05, p = 0.020 < α → reject H0; sample mean (1.29) is significantly greater than 1.25.

Test 2 — % of Squad Minutes Played: H0: μ ≤ 35.0 vs. Ha: μ > 35.0, α = 0.05. t = 2.48, p = 0.007 < α → reject H0; sample mean (37.16%) is significantly greater than 35%.

Confidence Interval — 95% CI for mean Team Points Per Match: (1.252, 1.325), consistent with Test 1's conclusion since 1.25 falls outside the interval.

## Assignment 6: Regression (2026-08-11)
- First predictor removed and why: Minutes removed because it had the highest p-value in
Model 1, p = 0.625, which is not significant at alpha = 0.05.
- Multicollinearity handling: We resolved multicollinearity by dropping the minutes variable as minutes and % of squad minutes were heavily correlated.
