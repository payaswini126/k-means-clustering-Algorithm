Customer Segmentation Using K-Means Clustering
This repository contains a Python implementation of customer segmentation using the K-Means Clustering algorithm. The purpose of this project is to group customers of a retail store based on their annual income and spending score, providing valuable insights for targeted marketing strategies.

Dataset
The dataset used for this project is Mall_Customers.csv, which contains information about 200 customers. 

The key features of the dataset are:
CustomerID: Unique ID for each customer.
Gender: Gender of the customer.
Age: Age of the customer.
Annual Income : Annual income of the customer in thousands of dollars.
Spending Score (1-100): A score assigned based on customer spending behavior.

Steps to Run the Project:
1. Prerequisites
Ensure you have the following libraries installed in your Python environment:
1.numpy
2.pandas
3.matplotlib
4.seaborn
5.scikit-learn

You can install these libraries using pip:
pip install numpy pandas matplotlib seaborn scikit-learn

2. Clone the Repository
Clone this repository to your local machine:
git clone https://github.com/your_username/customer-segmentation-kmeans.git
cd customer-segmentation-kmeans

3. Run the Script
Run the Python script (customer_segmentation.py) using the following command:
python customer_segmentation.py

METHODOLOGY:
1. Loading and Exploring the Dataset
The dataset is loaded into a Pandas DataFrame. The Annual Income and Spending Score columns are selected for clustering.

2. Elbow Method
The Elbow Method is used to determine the optimal number of clusters by calculating the Within-Cluster Sum of Squares (WCSS) for different values of 
K (number of clusters). A plot of WCSS versus 𝐾 helps identify the "elbow point."

3. Applying K-Means
The K-Means clustering algorithm is applied with the optimal number of clusters determined from the Elbow Method. The fit_predict method assigns each data point to a cluster.

4. Visualization
The clusters and their centroids are visualized using a scatter plot. Each cluster is represented with a unique color, and centroids are marked in cyan.

Output:
Elbow Point Graph
The Elbow Point graph helps determine the optimal number of clusters:


Customer Groups:
The scatter plot shows customer clusters based on Annual Income and Spending Score. Each cluster represents a group of customers with similar purchasing behavior:


Results:
The customers are segmented into 5 distinct clusters based on their purchasing behavior:

Cluster 1: Low income, low spending.
Cluster 2: High income, high spending.
Cluster 3: Medium income, medium spending.
Cluster 4: Low income, high spending.
Cluster 5: High income, low spending.
These insights can be used for personalized marketing strategies and improving customer engagement.

License:
This project is licensed under the MIT License. See the LICENSE file for details.

Contributing:
Contributions are welcome! If you have suggestions for improvements or find issues, please open an issue or create a pull request.

Acknowledgments:
Special thanks to the creators of the dataset and the open-source community for the tools used in this project.
