# Unsupervised-Learning
This project explores the application of unsupervised learning techniques to identify patterns, groupings, and structures within unlabeled data. The focus is on discovering hidden patterns and relationships in data without predefined labels.

## Features
- This project consists of two datasets.
- Treating missing values and duplicate values with suitable approaches.
- Understanding significant insights in the data through exploratory data analysis (EDA).
- Segmenting data using K-Means clustering.
- Applying Principal Component Analysis (PCA) for dimensionality reduction.
- Using the elbow technique to determine the optimal value of k for clustering.
- Building supervised learning models to predict the outputs.
- Comparing accuracies and other scores to select the best model for deployment.
- Tuning hyperparameters to enhance model performance.

## Dataset

- auto-mpg dataset



 https://www.kaggle.com/code/datafan07/auto-mpg-eda-feature-engineering-and-regressions/input


- Vehicle dataset

 https://www.kaggle.com/code/krishnaheroor/k-means-unsupervised-learning-explained/input

## Tools and Techniques

- Python
- Numpy
- Pandas
- Matplotlib
- Seaborn
- PCA
- clustering
- KMenas Clustering
- GridSearchCV

## Analysis


### Auto-mpg clustering(Kmeans)
- Elbow chart
- From the elbow chart, the optimal value of k for clustering is 5.

![image](https://github.com/user-attachments/assets/af5d909e-6589-43d4-99cd-206503adeda4)


K (Clusters) = **5**

- Cluster **Inertia** is  916.23
![image](https://github.com/user-attachments/assets/f1ef7c26-ff17-41cc-b69a-da6f9448b253)


K (Clusters) = **4**

- Cluster **Inertia** is  968.32

![image](https://github.com/user-attachments/assets/021fec1f-ec22-49f2-9933-6437a80bc9ac)

#### Observations
**Minimum Clusters:** From the pairplot, the minimum number of clusters is 3.

**Optimal Value of k:** Based on the graphs above, the optimal value of k is 4.
### Vehicle Data analysis
#### Model scores on Testset  before applying PCA:

- **Accuracy:** =  0.9647058823529412
- **Precision:** =  0.9635322483423749
- **Recall:** =  0.9638888888888889
- **F1-Score:** =  0.9632231360467101
- 
#### PCA chart(90% variance)

![image](https://github.com/user-attachments/assets/6de8a064-d4e0-4837-8396-edd892459318)


#### Model scores on Testset  after applying PCA:

- **Accuracy:** =  0.7588235294117647
- **Precision:** =  0.751901604523666
- **Recall:**  =  0.7478632478632479
- **F1-Score:** =  0.744708259546146


#### Observations
**Model Scores:** The model scores are very high with the original data.

**Effect of PCA:** After applying PCA, the model scores decreased significantly, even with cross-validation techniques.





