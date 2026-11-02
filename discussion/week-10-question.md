---
id: w10-rirar-rf-oob-tuning
title: "Choosing Random Forest Settings with OOB Error"
author: "rirar"
---

With OOB MSEs spanning only about 0.03, I would treat these settings as practically tied unless the difference is large relative to the OOB estimate's uncertainty. Node size and `mtry` affect both tree strength and correlation, so neither should be chosen from a single rule. A smaller `mtry` can decorrelate trees and improve averaging, but here only three of 20 predictors carry signal; considering fewer predictors can also make it less likely that a useful predictor is available at a split, increasing bias. With `mtry = 20`, trees may be more correlated, but they can use the signal more consistently and reduce bias. I would compare stability across repeated fits and prefer a simpler or more stable setting among near-ties.

The smallest OOB MSE is a tuning criterion, not an unbiased expected test error: selecting the minimum among candidates can make it optimistic. The independent test MSE of 1.074 is the better final performance estimate for the selected model, assuming the test set was not used to choose settings. The correlation concern is relevant, but it does not prove that smaller `mtry` is better.
