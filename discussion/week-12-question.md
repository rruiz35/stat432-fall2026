---
id: w12-rirar-spectral-umap
title: "Spectral Clustering and UMAP"
author: "rirar"
---

You run ordinary k-means on a dataset and get compact clusters that don’t match what domain experts expect. You then try spectral clustering with a 10-nearest-neighbor graph and UMAP, and both give cleanly separated groups in a plot. However, when you rerun UMAP with `n_neighbors = 5` instead of 15, one of the groups breaks into several fragments. Why might spectral clustering succeed where k-means failed, and should you conclude from the UMAP plot that there are truly that many separate clusters with large gaps between them? Explain your reasoning.
