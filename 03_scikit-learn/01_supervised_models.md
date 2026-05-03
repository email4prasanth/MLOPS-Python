# CLASSIFICATION MODELS

| Module | Model Name | Import Statement |
|--------|-----------|------------------|
| `neighbors` | `KNeighborsClassifier` | `from sklearn.neighbors import KNeighborsClassifier` |
| `neighbors` | `RadiusNeighborsClassifier` | `from sklearn.neighbors import RadiusNeighborsClassifier` |
| `linear_model` | `LogisticRegression` | `from sklearn.linear_model import LogisticRegression` |
| `linear_model` | `RidgeClassifier` | `from sklearn.linear_model import RidgeClassifier` |
| `linear_model` | `Perceptron` | `from sklearn.linear_model import Perceptron` |
| `svm` | `SVC` | `from sklearn.svm import SVC` |
| `svm` | `NuSVC` | `from sklearn.svm import NuSVC` |
| `svm` | `LinearSVC` | `from sklearn.svm import LinearSVC` |
| `tree` | `DecisionTreeClassifier` | `from sklearn.tree import DecisionTreeClassifier` |
| `ensemble` | `RandomForestClassifier` | `from sklearn.ensemble import RandomForestClassifier` |
| `ensemble` | `GradientBoostingClassifier` | `from sklearn.ensemble import GradientBoostingClassifier` |
| `ensemble` | `AdaBoostClassifier` | `from sklearn.ensemble import AdaBoostClassifier` |
| `ensemble` | `BaggingClassifier` | `from sklearn.ensemble import BaggingClassifier` |
| `ensemble` | `ExtraTreesClassifier` | `from sklearn.ensemble import ExtraTreesClassifier` |
| `naive_bayes` | `GaussianNB` | `from sklearn.naive_bayes import GaussianNB` |
| `naive_bayes` | `MultinomialNB` | `from sklearn.naive_bayes import MultinomialNB` |
| `naive_bayes` | `BernoulliNB` | `from sklearn.naive_bayes import BernoulliNB` |
| `discriminant_analysis` | `LinearDiscriminantAnalysis` | `from sklearn.discriminant_analysis import LinearDiscriminantAnalysis` |
| `discriminant_analysis` | `QuadraticDiscriminantAnalysis` | `from sklearn.discriminant_analysis import QuadraticDiscriminantAnalysis` |
| `gaussian_process` | `GaussianProcessClassifier` | `from sklearn.gaussian_process import GaussianProcessClassifier` |
| `neural_network` | `MLPClassifier` | `from sklearn.neural_network import MLPClassifier` |

---

# REGRESSION MODELS

| Module | Model Name | Import Statement |
|--------|-----------|------------------|
| `linear_model` | `LinearRegression` | `from sklearn.linear_model import LinearRegression` |
| `linear_model` | `Ridge` | `from sklearn.linear_model import Ridge` |
| `linear_model` | `Lasso` | `from sklearn.linear_model import Lasso` |
| `linear_model` | `ElasticNet` | `from sklearn.linear_model import ElasticNet` |
| `linear_model` | `SGDRegressor` | `from sklearn.linear_model import SGDRegressor` |
| `neighbors` | `KNeighborsRegressor` | `from sklearn.neighbors import KNeighborsRegressor` |
| `neighbors` | `RadiusNeighborsRegressor` | `from sklearn.neighbors import RadiusNeighborsRegressor` |
| `svm` | `SVR` | `from sklearn.svm import SVR` |
| `svm` | `NuSVR` | `from sklearn.svm import NuSVR` |
| `svm` | `LinearSVR` | `from sklearn.svm import LinearSVR` |
| `tree` | `DecisionTreeRegressor` | `from sklearn.tree import DecisionTreeRegressor` |
| `ensemble` | `RandomForestRegressor` | `from sklearn.ensemble import RandomForestRegressor` |
| `ensemble` | `GradientBoostingRegressor` | `from sklearn.ensemble import GradientBoostingRegressor` |
| `ensemble` | `AdaBoostRegressor` | `from sklearn.ensemble import AdaBoostRegressor` |
| `ensemble` | `BaggingRegressor` | `from sklearn.ensemble import BaggingRegressor` |
| `ensemble` | `ExtraTreesRegressor` | `from sklearn.ensemble import ExtraTreesRegressor` |
| `gaussian_process` | `GaussianProcessRegressor` | `from sklearn.gaussian_process import GaussianProcessRegressor` |
| `neural_network` | `MLPRegressor` | `from sklearn.neural_network import MLPRegressor` |

---

# QUICK REFERENCE BY MODULE

| Module | Classification Models | Regression Models |
|--------|---------------------|-------------------|
| `neighbors` | `KNeighborsClassifier`, `RadiusNeighborsClassifier` | `KNeighborsRegressor`, `RadiusNeighborsRegressor` |
| `linear_model` | `LogisticRegression`, `RidgeClassifier`, `Perceptron` | `LinearRegression`, `Ridge`, `Lasso`, `ElasticNet` |
| `svm` | `SVC`, `NuSVC`, `LinearSVC` | `SVR`, `NuSVR`, `LinearSVR` |
| `tree` | `DecisionTreeClassifier` | `DecisionTreeRegressor` |
| `ensemble` | `RandomForestClassifier`, `GradientBoostingClassifier`, `AdaBoostClassifier`, `BaggingClassifier`, `ExtraTreesClassifier` | `RandomForestRegressor`, `GradientBoostingRegressor`, `AdaBoostRegressor`, `BaggingRegressor`, `ExtraTreesRegressor` |
| `naive_bayes` | `GaussianNB`, `MultinomialNB`, `BernoulliNB` | *(none - classification only)* |
| `neural_network` | `MLPClassifier` | `MLPRegressor` |
| `discriminant_analysis` | `LinearDiscriminantAnalysis`, `QuadraticDiscriminantAnalysis` | `LinearDiscriminantAnalysis` |
| `gaussian_process` | `GaussianProcessClassifier` | `GaussianProcessRegressor` |

---

**Note:** All models follow the same import pattern:
```python
from sklearn.<module> import <ModelName>