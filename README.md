# Credit Score Portfolio

A portfolio of credit scoring projects on real public data: German Credit Risk (UCI, via Kaggle) and LendingClub accepted loans (2007 to 2018 Q4, via Kaggle). Each project is its own GitHub repository with a documented baseline, tests, and a README. Results that did not hold up, such as calibration gaps and drift, are reported as they are.

## Projects

| # | Name | Dataset | Main method | Repository |
|---|------|---------|-------------|-------------|
| CR01 | WOE Logistic Scorecard | German Credit | WOE binning, logistic regression, points table | [scorecard-woe-logistic](https://github.com/Patotricks15/scorecard-woe-logistic) |
| CR02 | Monotone Gradient Boosting Challenger | LendingClub | LightGBM with monotone constraints, compared with the scorecard, out-of-time validation | [gbm-monotone-challenger](https://github.com/Patotricks15/gbm-monotone-challenger) |
| CR03 | Calibration and Fairness | German Credit | Platt and isotonic calibration, group approval and error audit | [calibration-and-fairness](https://github.com/Patotricks15/calibration-and-fairness) |
| CR04 | Reason Codes and Explainability | German Credit (scorecard), LendingClub (challenger) | Scorecard point contributions and tree SHAP | [reason-codes-explainability](https://github.com/Patotricks15/reason-codes-explainability) |
| CR05 | Score Drift Monitoring | LendingClub | PSI, KS and monthly Gini | [score-drift-monitoring](https://github.com/Patotricks15/score-drift-monitoring) |
| CR06 | Cutoff Economics | LendingClub | Expected loss and profit curve over PD cutoffs | [cutoff-expected-loss](https://github.com/Patotricks15/cutoff-expected-loss) |

Shared code lives in [credit-scoring-core](https://github.com/Patotricks15/credit-scoring-core) (WOE, scorecard, metrics, economics).

## Scope

Each repository is self-contained and can be cloned, tested, and run independently. Raw data is not committed. German Credit is small and old, so use it to check the method, not to draw conclusions about current credit markets. LendingClub is US consumer lending data.
