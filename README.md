<h2> Credit Card Customer Clustering/h2>
<h4> Project Description </h4>
<p> 
In this project we cluster different customers of a bank from a previously used <a href='https://www.kaggle.com/datasets/sakshigoyal7/credit-card-customers'>Kaggle.</a> dataset.
</p>
<h4> Step-by-Step Solution </h4>
<p>
The following steps are used to cluster the customers:<br>
<ol>
<li> <strong> Data Preprocessing: </strong> Since this is a <a href='https://github.com/AliAbbasiSh/Credit-Card-Customers'>previously used dataset</a> the preprocessing step is the same as the mentioned project(one-hot encoding, lable encoding and ordical encoding) </li>
<li> <strong> Principal Component Analysis: </strong> Since there are a lot of features in this data frame, principal component analysis is conducted to reduce the number of features </li>
<li> <strong> Model Selection and Training: </strong> A K-Means clustering model is trained for this dataset</li>
</ol>
</p>
<h4> Principal Component Analysis(PCA)</h4>
<p> 
Since this dataset has a lot of features (even after preprocessing) principal component analysis (PCA) is done to reduce the number of features. The number of components is chosen based on the explained variance. A 95% cut-off threshold is chosen and as a result the number of components resulting in a more than 95% explained variance is 14.
<br>
<img src='https://github.com/AliAbbasiSh/Customer-Clustering/blob/main/PCA.png' ><br>
<br>
Afterwards, the correlation between each component and dataset feature is illustrated using a heatmap.
<br>
<img src='https://github.com/AliAbbasiSh/Customer-Clustering/blob/main/PCA%20correlation.png' ><br>
<br>
</p>
<h4> Model Selection and Training</h4>
<p>
In order to identify the most optimum number of clusters,<a href='https://www.analyticsvidhya.com/blog/2021/05/k-mean-getting-the-optimal-number-of-clusters/'>silhouette score</a> is the main parameter which we try to optimize and as it can be seen in the next graph 8 clusters is an optimal number.<br>
<br>
<img src='https://github.com/AliAbbasiSh/Customer-Clustering/blob/main/Silhouette%20Score.png' ><br>
<br>
And finaly the clustering is conducted with 14 compenents and 8 clusters. The relationship between different components are shown in the next figure and the clusters are differentiated with different colors.
<br>
<img src='https://github.com/AliAbbasiSh/Customer-Clustering/blob/main/download%20(1).png'><br>
<br>
</p>
