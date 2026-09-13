---
title: "Week 03 Discussion Question"
author: "rirar"
week: "03"
---

Ridge regression is often introduced as a solution when ordinary least squares becomes unstable because predictors are nearly redundant. Imagine a standardized design with an unpenalized intercept, where two predictors carry almost the same information and the response is noisy. Why might the OLS coefficient estimates for those predictors have large sampling variability, especially for a contrast such as $\widehat{\beta}_1-\widehat{\beta}_2$? How does ridge regression shrink those directions through the penalty term, and why can this shrinkage reduce variance while introducing only a modest increase in squared bias? Explain the tradeoff in plain language and connect it to the idea of effective degrees of freedom from Week 2. If the predictors were orthogonal instead, how would the same ridge penalty behave differently?
