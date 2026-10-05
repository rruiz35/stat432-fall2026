---
title: "Week 06 Discussion Question"
author: "rirar"
week: "06"
---

In a classification tree, why do we first grow a large tree and then prune it back instead of stopping as soon as a split gives only a small decrease in Gini impurity? Why can’t we use the training loss to choose the final tree size? The main issue is that a split with a small local improvement can still help a lot later because the tree is built greedily, and many small gains add up across the full structure. Training loss is also not a valid way to choose the final tree because it always decreases as the tree gets deeper, so a fully grown tree will almost always fit the training data perfectly even when it is overfitting. Pruning uses a separate validation or cross-validation criterion to pick the size that balances fit and complexity, which is why the final tree is selected after growing a larger model rather than stopping early.
