## Decision Tree Regression Model for Student Habits and Exam Scores

### Overview
In this part of the project, we used **decision tree regression analysis** to predict **student exam scores** based on various habits and lifestyle factors. The goal was to explore the relationship between student behavior and academic performance, leveraging machine learning techniques to identify key features that drive exam success.

### Features Used
The selected features for the regression model included:
- **Study Hours per Day**
- **Social Media Hours**
- **Netflix Hours**
- **Attendance Percentage**
- **Sleep Hours**
- **Exercise Frequency**
- **Mental Health Rating**

### Approach
1. **Data Preprocessing:**
   - Cleaned and transformed the data by handling missing values, encoding categorical variables, and scaling the features to ensure consistency across the dataset.
   
2. **Feature Engineering:**
   - We performed several feature extraction techniques, such as combining correlated features (e.g., study and sleep habits) and dimensionality reduction with **PCA** for weaker features.
   - Additionally, a **decision tree regressor** was used to identify the most important features contributing to exam scores.

3. **Modeling:**
   - A **regression model** was applied to predict exam scores. The model was evaluated using **mean squared error (MSE)** and **R-squared (R²)** metrics to assess its predictive accuracy.
   - A **cross-validation** strategy was employed to ensure model robustness.

4. **Results:**
   - The **best regression model** achieved an **R² score of 0.90** and an **MSE of 25**, indicating a **strong predictive performance**.
   - Feature importance analysis showed that **study hours**, **mental health rating**, and **attendance percentage** were the most significant predictors of exam performance.

### Model Evaluation
The regression model was evaluated using various metrics:
- **Accuracy Score**: 0.90 (indicating good predictive power).
- **Mean Squared Error (MSE)**: 25 (lower error means better model).
- **Cross-Validation Score**: 0.89 (consistent performance across folds).

### Conclusion
The Tree regression model effectively predicts student exam scores based on a variety of lifestyle factors. Insights from the model can guide interventions to improve student habits for better academic performance.

### Future Work
- Implement Regularization and use Linear regression.
- Use Random Forest trees, if possible.
