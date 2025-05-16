# Project Machine Learning: KMEANS ALGORITHM - CUSTOMER SEGMENTATION 👥👥👥
This project aims to leverage company data to enable the development of uniquely appealing products and services, allowing them to outperform their competitors, all implemented using the Python programming language.

---

## 📋 Casetudy: 

You are owing a supermarket mall and through membership cards, you have some basic data about your customers like Customer ID, age, gender, annual income and spending score. You want to understand the customers like who are the target customers so that the sense can be given to marketing team and plan the strategy accordingly.

---
## 🎯 Objectieves:

Customer Segmentation is the subdivision of a market into discrete customer groups that share similar characteristics. Customer Segmentation can be a powerful means to identify unsatisfied customer needs. Using the above data companies can then **outperform the competition by developing uniquely appealing products and services**.

---

## 📂 Dataset: 

* <a href= "https://github.com/TrieuTuanVi/KMEANS_ALGORITHM/blob/main/data.csv">Dataset</a>

* **Data dictionary**:

| **Fields**        | **Data Type** | **Features**                                                                                                                    |
|-------------------|---------------|---------------------------------------------------------------------------------------------------------------------------------|
|**ID**             | numerical     | unique identifier of each customer                                                                                              |
|**Sex**            | categrical    | **0**: male, **1**: female                                                                                                      |
|**Marital status** | categorical   | **0**: single, **1**: non-single (divorced, separated, married, widowed)                                                        |
|**Age**            | numerical     | age in years                                                                                                                    |
|**Education**      | categorical   | **0**: other/unknown, **1**: high school, **2**: university, **3**: graduate school                                             |
|**Income**         | numerical     | annual income in USD/ Occupation                                                                                                |
|**Categorical**    | categorical   | **0**: unemployed/unskilled, **1**: skilled employee/official, **2**: management/self-employed/highly qualified employed/officer|
|**Settlement size**|categorical    | **0**: small city, **1**: mid-sized city, **2**: big city                                                                       | 

* The dataset consists of information about the purchasing behavior of 2,000 individuals from a given area when entering a physical ‘FMCG’ store. All data has been collected through the loyalty cards they use at checkout. The data has been preprocessed and there are no missing values. In addition, the volume of the dataset has been restricted and anonymised to protect the privacy of the customers.

---

## 📚 Introduction to DBSCAN

**DBSCAN** is a density-based clustering algorithm that allows detecting clusters of arbitrary shapes and identifying noise points.

How it works:
- **Core Point**: A point is considered a core point if there are at least minPts points within its radius ε.
- **Reachable Point**: From a core point, DBSCAN will expand to points within ε and continue to check whether those points are core points.
- **Border Point**: Points within the ε region of the core point but do not have enough neighbors to become core points.
- **Noise**: Points that do not belong to any cluster because they are not within ε of any core point.
- **Iterative process**: When the current cluster cannot be expanded further, the algorithm moves to the next unvisited point and starts the check again from the beginning.

Result:
- Clusters of densely connected points are created.
- Automatically detects noise points without specifying the number of clusters in advance.

---
## 🛠️ Technology used

- **Programming language**:  [![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)](https://www.python.org/) Python: – a powerful, flexible and popular language in the field of data science and machine learning.

- **Analysis & visualization tools**: [![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=jupyter&logoColor=white)](https://jupyter.org/) Jupyter Notebook:  – an interactive environment that allows writing code, displaying charts and annotating explanatory notes in the same interface, effectively supporting the process of exploring and presenting data.

---

## 🛠️ Steps to implement K-Means algorithm:

- Collect data from suitable sources (CSV, Excel, etc.).
- Preprocess data: handle missing values, standardize data (StandardScaler).

  ![image](https://github.com/user-attachments/assets/5a7618aa-1ef0-4630-82e5-5e50e1f89783)

- Select appropriate features for clustering.
- Determine the number of clusters k using Elbow/ Silhouette method.

![image](https://github.com/user-attachments/assets/2be5b1d0-0e2b-4ab6-8774-f4af94f49fc5)

- Train K-Means model with the selected number of clusters.
- Assign cluster labels to each data point.
- Visualize clustering results (using matplotlib or seaborn).
- Analyze clusters and draw insights from each group.

---
## ✅ Result

![image](https://github.com/user-attachments/assets/bbeeaca8-c7a6-4a86-b362-a13f92452df0)


The above graph illustrates the results of clustering data using the DBSCAN (Density-Based Spatial Clustering of Applications with Noise) algorithm. Each data point represents an individual, with the horizontal axis being age and the vertical axis being annual income. The colors of the points represent different clusters detected by DBSCAN.

- Number of clusters identified: 26
- Number of noise points: 177
- Noise points are labeled -1 and do not belong to any cluster, are often scattered and do not have a high enough density to form a cluster.
- DBSCAN is well suited to detecting clusters with complex shapes and removing noise without pre-specifying the number of clusters.

This graph helps visualize the natural cluster structure in customer data, supporting the development of appropriate segmentation strategies in business.

---
## 🏆 Conclusion

The application of the DBSCAN algorithm in the project has helped to effectively detect clusters of potential customers based on age and income, while eliminating inappropriate noise points, thereby helping businesses better understand market segments and optimize customer approach strategies.
