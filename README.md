Strategic Engagement Analysis: Decoding Marketplace Virality
Project OverviewThis project identifies the structural drivers of engagement within a Facebook Marketplace dataset of 7,000+ retail records. Moving beyond basic descriptive statistics, this analysis utilizes a multi-model unsupervised learning framework to segment content behavior and quantify the "viral lift" of different media formats.The core discovery identifies a "Vertical Scaling" effect in Video content, which achieves engagement multipliers up to 20x higher than the marketplace baseline, compared to a stagnant "Growth Plateau" found in static Photos.

Key Technical Features:
1.Multi-Model Clustering: Parallel implementation of K-Means, Agglomerative (Hierarchical) Clustering, and DBSCAN to triangulate user behavior patterns.
2.Density-Based Outlier Detection: Utilized DBSCAN to isolate the 29 most viral posts in the dataset, identifying them as distinct "Viral Engines" rather than statistical noise.
3.Advanced Statistical Validation:  Achieved a Silhouette Score of 0.9184, indicating exceptionally high cluster density and separation.Optimized model selection using Bayesian Information Criterion (BIC) with a score of -224,898.2, verifying the 2-cluster probabilistic fit.
4.Relative Performance Matrix: Engineered a custom "Base Condition" logic to calculate performance multipliers across nine different engagement metrics (Reactions, Shares, Loves, etc.

Strategic Insights:
1.The Video "Viral Engine"Analysis shows that Video is the only format capable of breaking the engagement ceiling. While present in both standard and elite clusters, Videos in the top segment demonstrated:
    15x - 20x Multiplier in high-effort actions (Shares and Loves).
    Superior "Conversion-to-Share" rates compared to all other media types.
2.The Photo "Growth Plateau"Despite being the most frequent content type, Photos exhibit a localized performance limit:
    Initial entry-level engagement shows a ~84% spike.
    However, growth remains flat (1x - 2x) in viral metrics, failing to achieve the exponential scaling seen in Video content.
3. Structural TieringThe marketplace is not evenly distributed. It follows a "Heavy-Tail" distribution where ~95% of content resides in a standard baseline, while a tiny "Elite" segment drives the majority of organic reach.

Implementation Workflow:
1.Preprocessing: One-Hot Encoding of categorical media types and feature scaling.
2.Dimensionality Reduction: Utilized PCA to project high-dimensional behavioral data for visualization and cluster analysis.
3.Clustering & Optimization: Iterative testing of k-values using Elbow Method, Silhouette Analysis, and BIC.
4.Multiplier Analysis: Comparative benchmarking of clusters against a calculated "Base Condition" for each model.
