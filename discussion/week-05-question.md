---
title: "Week 05 Discussion Question"
author: "rirar"
week: "05"
---

In high-dimensional data, why does KNN often become less reliable as the number of predictors increases, even when the data still follow a local pattern? As dimensionality rises, distances between observations become more similar, so a point’s nearest neighbors may no longer be especially close in a meaningful sense. This makes local neighborhoods less informative and increases variance in prediction. In practice, KNN can require much more data to maintain the same density of neighbors, so the method becomes less stable and less accurate in high dimensions.
