# K-Nearest Neighbors (KNN) Project

## Project Overview
This project demonstrates the use of the **K-Nearest Neighbors (KNN)** algorithm for both classification and regression.  
It explains the theory behind KNN, different algorithm variants, and applies it to synthetic datasets.  
Model performance is evaluated with appropriate metrics, and hyperparameter tuning is performed for classification.  

---

# 1. Theory

## KNN Classifier
- A **lazy learning algorithm** that does not build an explicit model.  
- Classifies a data point based on the **majority class** of its K nearest neighbors.  
- Distance measures commonly used: Euclidean, Manhattan, Minkowski.  

## KNN Regressor
- Predicts the value of a data point based on the **average (or weighted average)** of the K nearest neighbors.  
- Suitable for continuous output variables.  

---

## Variants of KNN (for Classification)
1. **Brute Force**:  
   - Computes distance of a query point to all training samples.  
   - Simple but computationally expensive.  

2. **Ball Tree**:  
   - Partitions data into nested hyperspheres.  
   - Efficient for high-dimensional datasets.  

3. **KD Tree**:  
   - Partitions data into k-dimensional space.  
   - Works best with low-dimensional data.  

---

# 2. Implementation

## Classification
- Dataset: Generated using `make_classification`.  
- Built a **KNN Classifier** with different values of K.  
- Performed **Hyperparameter Tuning** using GridSearchCV and RandomizedSearchCV to find the optimal K and distance metric.  

## Regression
- Dataset: Generated using `make_regression`.  
- Built a **KNN Regressor** to predict continuous values.  

---

# 3. Model Evaluation

## For Classification
- **Accuracy Score**  
- **Confusion Matrix**  
- **Classification Report** (Precision, Recall, F1-Score)  

## For Regression
- **Mean Squared Error (MSE)**  
- **Mean Absolute Error (MAE)**  
- **R² Score (Coefficient of Determination)**  

---

# 4. Conclusion
- KNN is a simple yet powerful algorithm for both classification and regression.  
- Performance depends heavily on the choice of **K** and the **distance metric**.  
- **Brute Force** is simple but slower, while **Ball Tree** and **KD Tree** improve efficiency.  
- Hyperparameter tuning significantly improves classification accuracy.  
- Regression performance is evaluated with error metrics, showing how KNN adapts to continuous predictions.  
