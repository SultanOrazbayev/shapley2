# Shapley2

SHAPLEY2: Stata module to compute additive decomposition of estimation statistics by regressors or groups of regressors

Shapley2 is a post-estimation command to compute the Shorrocks-Shapley decomposition of any statistic of the model (normally the R squared). Shapley2 can be used for most estimation commands, e.g. ols, probit, logit, oprobit. Compared to the user written command shapley, shapley2 is faster and enables you to compute the Shapley value by groups of variables. The results are stored as e()-matrices, allowing the user to use them afterwards, for instance to export them to LaTeX.

Citation:

Florian Chavez Juarez, 2012. "SHAPLEY2: Stata module to compute additive decomposition of estimation statistics by regressors or groups of regressors," Statistical Software Components S457543, Boston College Department of Economics, revised 17 Jun 2015.


# Installation

Installing from SSC directly:

```stata
ssc install shapley2
```

Installing from GitHub directly (to get the latest version):

```stata
cap ado uninstall shapley2
net install shapley2, from("https://raw.githubusercontent.com/sultanorazbayev/shapley2/main/src/")
```
