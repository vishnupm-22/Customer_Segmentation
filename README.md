
## **CUSTOMER SEGMENTATION**
**problem statement**:
* Implement KMeans clustering to develop a mall customer segmentation strategy based on customer behavior and demographic data to enhance marketing and optimize space 
 utilization.

**Steps** :
* Understanding the data
* EDA
* Handling Imbalanced dataset 
* Model Building and Evaluation

**Dataset link** : https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python
Data contains 5 features : CustomerID ,Gender, Age, Annual Income ,Spending Score of a customer.
Demographic data plays a crucial role in identifying patterns and preferences among different consumer groups. So Features like Age,Gender,Annual Income and Spending Score are important for grouping the data.

**Did exploratory data analysis to gain some insights on data**:
* **Univariate Analysis**:
  * from dist plot : Gender feature displays a normall distribution whereas distribution of Age and Annual Income (k$) is positively skewed.
  * from box plot ,there are no outliers in the data.
  * Gender distribution : plotting Bar,pie chart shows female customers just edge out the male customers.
* **Bivariate Analysis**:
  * Pair Plot : Scatter plot between Annual Income and Spending Score have some groupings in the data. These groupings  suggest the presence of clusters.
  * heat map : Annual Income and Spending Score are positively correlated.Age wrt to  Annual Income and Spending Score are negatively correlated.
 
**Feature Engineering**:
 * Applied MinMaxScaler technique to the features that does not display a normal distribution,
 * Applied PCA technique to reduce the dimension from 4d to 2d and to visualize the clusters in 2d

**Model Building and Evaluation**:
 * used elbow method to find the optimal no of clusters (k).
 * Implemented K-means and visualized these clusters with their centroids.
