# Student-Grade-prediction
Predicts students’ final grade (G3) from demographic, social and school features using scikit-learn.

Data: UCI Student Performance dataset , math course, 395 rows. The notebook downloads it directly from UCI.

What I did: Started with exploring the data, split 80/20, set a mean-prediction baseline, and trained Linear Regression and Random Forest, with and without the earlier-period grades G1 and G2.

Baseline(mean): MAE (3.65), R2 (n/a)

With G1, G2 [Linear Regression]: MAE (1.65), R2 (0.72)

With G1, G2 [Random Forest]:	MAE (1.16), R2 (0.81)

Without G1, G2 [Linear Regression]:	MAE (3.40), R2 (0.14)

Without G1, G2	[Random Forest]: MAE(3.15), R2	(0.24)


Takeaway: prior grades account for nearly all the predictive power; other features barely beat the baseline.

Limitations: small dataset and no tuning.
