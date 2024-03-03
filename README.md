# Shapley2

SHAPLEY2: Stata module to compute additive decomposition of estimation statistics by regressors or groups of regressors

Shapley2 is a post-estimation command to compute the Shorrocks-Shapley decomposition of any statistic of the model (normally the R squared). Shapley2 can be used for most estimation commands, e.g. ols, probit, logit, oprobit. Compared to the user written command shapley, shapley2 is faster and enables you to compute the Shapley value by groups of variables. The results are stored as e()-matrices, allowing the user to use them afterwards, for instance to export them to LaTeX.

The original package was developed by Florian Wendelspiess Chavez Juarez.
Starting with version 1.6, maintenance of the package is done by Sultan Orazbayev.
Additional contributions are welcome, please raise an issue or submit a pull
request here: https://github.com/SultanOrazbayev/shapley2.

Citation:

for versions 1.6+, use:

Florian Chavez Juarez and Sultan Orazbayev, 2023. "SHAPLEY2: Stata module to compute additive decomposition of estimation statistics by regressors or groups of regressors".

for the original code (up to and including version 1.5), use:

Florian Chavez Juarez, 2012. "SHAPLEY2: Stata module to compute additive decomposition of estimation statistics by regressors or groups of regressors," Statistical Software Components S457543, Boston College Department of Economics, revised 17 Jun 2015.


# Installation

Installing from SSC directly (currently only for version 1.5):

```stata
ssc install shapley2
```

Installing from GitHub directly (to get the latest version):

```stata
cap ado uninstall shapley2
net install shapley2, from("https://raw.githubusercontent.com/sultanorazbayev/shapley2/main/src/")
```


# Changelog

- Version 1.7: Adding special handling for the reghdfe command with the 'absorb' option.
- Version 1.6: Incorporated explicit parsing of the 'if' condition in the provided command.
- Version 1.5: It is now possible to use f. and l. factor variables as dependent variables
- Version 1.4: Small bugfix: sometimes the program did not execute in protected working directories. Change does not affect result.
- Version 1.3: Small bugfix: shapley2 did not work with oprobit. The fix does not affect the results. 
- Version 1.2: Change in the computation, now closer to similar routines. Bugfix: now accepts very long group-statements
- Version 1.1: Bugfix to ensure no changes are made to the current database. 
- Version 1.0: First release on 06nov2012
