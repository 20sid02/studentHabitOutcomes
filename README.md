## Clustering Model for Student Habits

### Overview
In this section of the project, we applied **unsupervised machine learning** techniques to cluster students based on their habits, behaviors, and lifestyle factors. The goal was to segment students into meaningful groups that share similar characteristics, helping to understand how their behaviors relate to their academic performance.

### Approach
We used the **K-Means clustering algorithm** to group students into clusters based on various features like **study hours**, **sleep hours**, **exercise frequency**, **mental health rating**, and other lifestyle factors. The dataset used in this part contains information on students' habits and their respective academic performances.

#### Steps Taken:
1. **Data Preprocessing:**
   - The dataset was cleaned by handling missing values and converting categorical features into numerical labels for clustering.
   - Features like **study hours**, **attendance percentage**, **mental health rating**, and **sleep hours** were selected to perform clustering.

2. **Feature Engineering and Scaling:**
   - **Standard scaling** was applied to the features to ensure that they were on the same scale and the clustering algorithm wouldn’t be biased toward higher magnitude features.
   - **PCA (Principal Component Analysis)** was also applied to reduce dimensionality and help visualize the clusters in 2D or 3D plots, especially when dealing with high-dimensional data.

3. **Clustering with K-Means:**
   - The **K-Means** algorithm was used to create **4 clusters** (based on the visualization and analysis). K-Means groups students into clusters such that the variance within each group is minimized.
   - The optimal number of clusters was determined using techniques like **elbow method** or visualizations like **pairplots** and **PCA scatter plots**.

4. **Model Evaluation:**
   - **Silhouette score** was used to evaluate the quality of the clusters, measuring how similar an object is to its own cluster compared to other clusters.
   - The clusters were visually inspected through **pair plots** and **PCA plots** to see how distinct and well-separated the groups were.
   
5. **Cluster Analysis:**
   - After clustering, the mean of the features within each cluster was calculated to understand the characteristics of each group.
   - The clusters were then labeled based on the student habits:
     - **Balanced but Inactive**
     - **Distracted Media Users**
     - **High Achievers**
     - **Working Students**
   - Each group showed distinct patterns in terms of academic performance, attendance, study habits, and lifestyle.

### Results
- The K-Means clustering algorithm successfully grouped students into meaningful clusters based on their habits.
- The **PCA scatter plots** showed clear distinctions between clusters, confirming the effectiveness of the clustering process.
- Cluster analysis revealed that **High Achievers** had better attendance and study habits, while **Distracted Media Users** spent more time on social media and Netflix.

### Conclusion
This clustering analysis provides valuable insights into student behavior patterns. By identifying clusters of students with similar habits, this analysis can help educators tailor their strategies to improve academic performance for different groups. It also shows how unsupervised learning can uncover hidden patterns and groupings in complex datasets.

### Key Insights:
- The four identified clusters had significant differences in terms of study habits, media consumption, and academic performance.
- The clustering analysis can help in understanding how lifestyle choices like media consumption and exercise affect student performance.

### Future Work:
- Further refinement can be done by trying different clustering algorithms such as **DBSCAN** or **Hierarchical Clustering**.
- Adding more features (e.g., parental education or socioeconomic status) could lead to more detailed clusters.
