# L05 — Further Reading & Glossary

## Further reading

### Videos (free)

- **StatQuest — PCA, Step-By-Step**
  [https://www.youtube.com/watch?v=FgakZw6K1QQ](https://www.youtube.com/watch?v=FgakZw6K1QQ)

- **StatQuest — K-Means Clustering**
  [https://www.youtube.com/watch?v=4b5d3muPQmA](https://www.youtube.com/watch?v=4b5d3muPQmA)

- **StatQuest — t-SNE**
  [https://www.youtube.com/watch?v=NEaUSP4YerM](https://www.youtube.com/watch?v=NEaUSP4YerM)

- **StatQuest — DBSCAN**
  [https://www.youtube.com/watch?v=RDZUdRSDOok](https://www.youtube.com/watch?v=RDZUdRSDOok)

### Interactive / official docs

- **scikit-learn — Clustering**
  [https://scikit-learn.org/stable/modules/clustering.html](https://scikit-learn.org/stable/modules/clustering.html)
  Includes the famous "Comparing different clustering algorithms" gallery — bookmark it.

- **scikit-learn — Outlier detection**
  [https://scikit-learn.org/stable/modules/outlier_detection.html](https://scikit-learn.org/stable/modules/outlier_detection.html)
  Side-by-side comparison of Isolation Forest, One-Class SVM, and Local Outlier Factor.

- **UMAP documentation**
  [https://umap-learn.readthedocs.io/](https://umap-learn.readthedocs.io/)

### Books

- **Hands-On Machine Learning** by Aurélien Géron — chapter 8 (dimensionality reduction) and chapter 9 (unsupervised).
- **Pattern Recognition and Machine Learning** by Bishop — chapter 9 covers EM, K-Means, and Gaussian mixtures.

---

## Glossary (20 key terms)

- **Anomaly / Outlier** — A data point that differs significantly from the rest of the dataset. The distinction: "outlier" usually implies measurement error or noise; "anomaly" implies something genuinely interesting (fraud, malfunction).

- **Centroid** — In K-Means, the mean of all points assigned to a cluster. The cluster's "centre."

- **Contamination** — In Isolation Forest, the expected fraction of anomalies in the data. Affects the threshold used to label points as anomalous; doesn't affect the underlying anomaly score.

- **DBSCAN** — Density-Based Spatial Clustering of Applications with Noise. Finds clusters of varying shape; flags low-density points as noise. Doesn't need K specified.

- **Dimensionality reduction** — Squeezing high-dimensional data into fewer dimensions while preserving as much signal as possible. PCA, t-SNE, and UMAP are the three most common methods.

- **Eigenvector / Eigenvalue** — In PCA, the eigenvectors of the covariance matrix are the principal components. The eigenvalues are their corresponding variances.

- **Elbow method** — A heuristic for choosing K in K-Means. Plot inertia (within-cluster sum of squares) vs K; look for the bend where the curve flattens.

- **`explained_variance_ratio_`** — The fraction of total variance captured by each principal component. Components are ordered: PC1 captures the most.

- **Hierarchical clustering** — A clustering family that builds a tree of nested groupings (dendrogram). Doesn't require K up-front but is O(n²) — slow on large datasets.

- **Inertia** — In K-Means, the sum of squared distances from each point to its assigned centroid. Lower = tighter clusters. Always decreases as K grows.

- **Isolation Forest** — An anomaly detection algorithm. Builds random trees; anomalies tend to be isolated (reach leaves) in few splits.

- **K-Means** — Partitions data into K spherical clusters by minimising within-cluster variance. The default first try for segmentation.

- **Principal Component** — In PCA, a new axis (a linear combination of the original features) along which data is most spread out. PCs are ordered by variance and are mutually orthogonal.

- **PCA** — Principal Component Analysis. Standard linear dimensionality reduction. Always scale features first.

- **Scree plot** — Plot of `explained_variance_ratio_` vs PC index. Look for the elbow.

- **Silhouette score** — A clustering quality metric per point: how close it is to its own cluster vs the nearest other cluster. Mean silhouette across all points gives an overall cluster quality from -1 to +1.

- **t-SNE** — t-Distributed Stochastic Neighbour Embedding. Non-linear dimensionality reduction, mainly for visualisation. Preserves local structure but distorts global structure. Slow; expensive on large datasets.

- **UMAP** — Uniform Manifold Approximation and Projection. The modern alternative to t-SNE; faster, often preserves more structure. Default choice for non-linear viz today.

- **Unsupervised learning** — ML without labels. Finds structure in the data: clusters, principal components, anomalies. Contrast with supervised learning (L03/L04), which uses labels to predict targets.

- **Variance explained** — How much of the original data's spread a reduced representation captures. PCA explicitly maximises this; t-SNE and UMAP do not.
