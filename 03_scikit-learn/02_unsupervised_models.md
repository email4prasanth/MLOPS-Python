# UNSUPERVISED LEARNING MODELS

Unsupervised learning models work with unlabeled data (only `X`, no `y`).

---

## CLUSTERING MODELS

| Module | Model Name | Import Statement |
|--------|-----------|------------------|
| `cluster` | `KMeans` | `from sklearn.cluster import KMeans` |
| `cluster` | `MiniBatchKMeans` | `from sklearn.cluster import MiniBatchKMeans` |
| `cluster` | `DBSCAN` | `from sklearn.cluster import DBSCAN` |
| `cluster` | `OPTICS` | `from sklearn.cluster import OPTICS` |
| `cluster` | `AgglomerativeClustering` | `from sklearn.cluster import AgglomerativeClustering` |
| `cluster` | `MeanShift` | `from sklearn.cluster import MeanShift` |
| `cluster` | `SpectralClustering` | `from sklearn.cluster import SpectralClustering` |
| `cluster` | `Birch` | `from sklearn.cluster import Birch` |
| `cluster` | `AffinityPropagation` | `from sklearn.cluster import AffinityPropagation` |
| `mixture` | `GaussianMixture` | `from sklearn.mixture import GaussianMixture` |
| `mixture` | `BayesianGaussianMixture` | `from sklearn.mixture import BayesianGaussianMixture` |

---

## DIMENSIONALITY REDUCTION MODELS

| Module | Model Name | Import Statement |
|--------|-----------|------------------|
| `decomposition` | `PCA` | `from sklearn.decomposition import PCA` |
| `decomposition` | `IncrementalPCA` | `from sklearn.decomposition import IncrementalPCA` |
| `decomposition` | `KernelPCA` | `from sklearn.decomposition import KernelPCA` |
| `decomposition` | `SparsePCA` | `from sklearn.decomposition import SparsePCA` |
| `decomposition` | `TruncatedSVD` | `from sklearn.decomposition import TruncatedSVD` |
| `decomposition` | `NMF` | `from sklearn.decomposition import NMF` |
| `decomposition` | `FastICA` | `from sklearn.decomposition import FastICA` |
| `manifold` | `TSNE` | `from sklearn.manifold import TSNE` |
| `manifold` | `Isomap` | `from sklearn.manifold import Isomap` |
| `manifold` | `LocallyLinearEmbedding` | `from sklearn.manifold import LocallyLinearEmbedding` |
| `manifold` | `MDS` | `from sklearn.manifold import MDS` |
| `manifold` | `SpectralEmbedding` | `from sklearn.manifold import SpectralEmbedding` |
| `discriminant_analysis` | `LinearDiscriminantAnalysis` | `from sklearn.discriminant_analysis import LinearDiscriminantAnalysis` |

---

## ANOMALY / OUTLIER DETECTION MODELS

| Module | Model Name | Import Statement |
|--------|-----------|------------------|
| `ensemble` | `IsolationForest` | `from sklearn.ensemble import IsolationForest` |
| `neighbors` | `LocalOutlierFactor` | `from sklearn.neighbors import LocalOutlierFactor` |
| `svm` | `OneClassSVM` | `from sklearn.svm import OneClassSVM` |
| `covariance` | `EllipticEnvelope` | `from sklearn.covariance import EllipticEnvelope` |

---

## ASSOCIATION RULE MINING

| Module | Model Name | Import Statement |
|--------|-----------|------------------|
| `apriori` | `apriori` | `from sklearn.apriori import apriori` *(deprecated - use `mlxtend` instead)* |

> **Note:** sklearn doesn't have built-in association rule mining (Apriori, FP-Growth). Use `mlxtend` library instead.

---

## PREPROCESSING (Feature Scaling, Encoding, etc.)

These are transformers, not models, but commonly used in unsupervised context:

| Module | Model Name | Import Statement |
|--------|-----------|------------------|
| `preprocessing` | `StandardScaler` | `from sklearn.preprocessing import StandardScaler` |
| `preprocessing` | `MinMaxScaler` | `from sklearn.preprocessing import MinMaxScaler` |
| `preprocessing` | `LabelEncoder` | `from sklearn.preprocessing import LabelEncoder` |
| `preprocessing` | `OneHotEncoder` | `from sklearn.preprocessing import OneHotEncoder` |
| `preprocessing` | `Normalizer` | `from sklearn.preprocessing import Normalizer` |
| `preprocessing` | `RobustScaler` | `from sklearn.preprocessing import RobustScaler` |

---

## QUICK REFERENCE BY USE CASE

| Use Case | Common Models |
|----------|---------------|
| **Customer Segmentation** | `KMeans`, `DBSCAN`, `AgglomerativeClustering` |
| **Image Compression** | `PCA`, `NMF`, `KMeans` |
| **Data Visualization** | `TSNE`, `PCA`, `Isomap`, `MDS` |
| **Anomaly Detection** | `IsolationForest`, `OneClassSVM`, `LocalOutlierFactor` |
| **Feature Reduction** | `PCA`, `TruncatedSVD`, `FastICA` |
| **Noise Reduction** | `PCA`, `KernelPCA` |

---

## EXAMPLE USAGE

```python
# Clustering example
from sklearn.cluster import KMeans
kmeans = KMeans(n_clusters=3)
kmeans.fit(X)
labels = kmeans.predict(X)
clusters = kmeans.labels_
centroids = kmeans.cluster_centers_

# Dimensionality reduction example
from sklearn.decomposition import PCA
pca = PCA(n_components=2)
X_reduced = pca.fit_transform(X)

# Anomaly detection example
from sklearn.ensemble import IsolationForest
iso_forest = IsolationForest(contamination=0.1)
outliers = iso_forest.fit_predict(X)