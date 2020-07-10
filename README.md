# Advanced Customer Segmentation

Patrick Hennessey

## Outline

### Part 0: Data cleaning and rough feature selection

#### Data cleaning:

 * Fix columns that spring errors
 * Remove columns with >20% missing values (found empirically with a histogram)
 * LabelEncoder for ABDC labels
 * Once features are selected (rough), find threshhold to remove rows with high missing value proportion

#### Feature selection:

 * Take all consumption oriented features, as well as socioeconomic feaures of both the person and the neighborhood
 * Identify and remove multicollinearities in the feature set

### Part 1: Unsupervised Customer Segmentation

#### Without feature extraction

 * Run k-Means clustering
 * Try hierarchical clustering, if it doesn't take too long.

#### With feature extraction

 * Add PCA here and see how that effects the clustering analysis

### Part 2: Supervised Machine Learning

 * Use voting method to pick features for training

 * Run another analysis using PCA

 * Ultimately, use XGBoost on the output of the feature selection and extraction.

* Might also be interesting to build a PyTorch model for this as well.