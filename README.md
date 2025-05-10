# KMEANS_ALGORITHM
Using the above data companies can then outperform the competition by developing uniquely appealing products and services

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
