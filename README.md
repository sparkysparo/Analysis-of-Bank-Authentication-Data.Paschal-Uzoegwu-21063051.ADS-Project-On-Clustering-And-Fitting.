# Analysis-of-Bank-Authentication-Data.Paschal-Uzoegwu-21063051.ADS-Project-On-Clustering-And-Fitting.
This project delves into the analysis of bank authentication data to identify patterns and relationships among various features. The dataset comprises four features: variance, skewness, curtosis, and entropy, along with the class label indicating authentic or fraudulent transactions.
## Analysis Process.
### Dataset Exploration
The initial step involved exploring the dataset to understand its structure and contents. The dataset contains 5 columns, with the first four columns representing numerical features and the last column representing the class label.

### Data Cleaning and Preparation
Before analysis, the dataset underwent preprocessing to handle missing values, descriptive statistics, outliers, and data type conversions. Standardization was applied to ensure uniform scaling of features.

## Clustering and Fitting Techniques;
Two primary techniques were employed:

K-Means Clustering: Utilized to group similar data points into clusters based on feature similarity.
Polynomial Fitting: Applied to fit a polynomial curve to the relationship between variance and skewness features.
## Visualization:
Visualizations such as scatter plots, line graphs, distribution plots,pair plots and heatmap. were generated to explore the data's characteristics and relationships.
The dispersed scatter plot, show a non-linear relationship between variance and skewness in a scatter plot suggests that there is no simple or direct correlation between the variables in the dataset.The distributions of statistical metrics  for a dataset are shown by the histograms: Right-skewed variance, multimodal skewness, right-skewed kurtosis with a long tail, and essentially normal entropy with a small right skew are all present.

The heatmap shows strong negative correlation between variance and class (-0.72), which suggests that less variance is characteristic of one class, and the strong negative correlation between skewness and curtosis (-0.79), which suggests that data with higher skewness tend to have less heavy tails. The heatmap displays correlations between various statistical features and a class label. There are other correlations that exhibit weaker linear relationships.
##Clustering Analysis.
Clustering Visualization: The scatter plots displayed clustered data points with distinct cluster centers.The two-cluster solution from the clustering analysis using features like variance, skewness, entropy, and curtosis is visually summarised in the graphs. On each graph, observations with generally lower feature values are grouped in Cluster 1, shown in blue, and observations with higher feature values are grouped in Cluster 2, shown in orange. The calculated cluster centres, or the central points around which the observations in each cluster are grouped, are represented by the red stars. Given how clearly the separation is along the variance axis, it appears to be a powerful characteristic for separating the two clusters. However, some clusters are intermingled along the axes of curtosis, entropy, and skewness, suggesting that these characteristics influence the clustering but are not significant.

### Silhouette method and elbow method:
The elbow determines the optimal number of clusters based on the elbow point in the distortion plot,while the silhouette method evaluate 
cluster cohesion and separation, helping assess clustering quality. The highest silhouette score at that point in the silhouette method graph suggests strong cohesion within clusters and good separation between them, indicating that the dataset is best divided into two clusters. 
The within-cluster sum of squares decreases sharply up to that point and then levels off, indicating diminishing returns for additional clusters beyond three. In the meantime, the elbow method graph suggests that three clusters might be optimal.

## Fitting Analysis.
#### Polynomial Fitting:
This graph shows how the relationship between variance and skewness can be fitted using a second-degree polynomial. The polynomial fit, which makes an effort to simulate the underlying trend among the data points, is represented by the dark line.The 95% confidence interval is shown by the shaded region surrounding the polynomial line; this range gives us a 95% confidence level regarding the existence of the true regression line.

Blue dots are used to symbolise the actual data points. In addition, the graph has multiple vertical blue lines that, based on their likely representation as residuals for specific predicted points, show how far the actual data points are from the values that correspond to them on the fitted curve. When we move along the variance axis, the residuals' dispersion varies, giving the impression that they are heteroscedastic; they are not equally dispersed throughout the variance range.
The spread and pattern of the residuals show that, overall, although the polynomial fit explains some of the trends in the data, there is a significant amount of variability that this model is unable to account for. This implies that there may be other factors influencing the relationship that are not taken into account by the model, or that the relationship between variance and skewness is not perfectly quadratic.

## Insights
#### Cluster Patterns: 
Distinct clusters were found in the data, indicating differences in the feature distributions between real and fake transactions.
#### Relationships: 
An investigation into the connections between variance, skewness, and class labels revealed potential for discriminating against fraudulent transactions.
#### Recommendations:
To increase clustering accuracy, more research should be done on outlier detection and management.investigation of alternative fitting methods to improve the capture of non-linear relationships application of cutting-edge machine learning algorithms to fraud detection and predictive modelling.
