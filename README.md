# **Player Performance Prediction & Market Value Analysis Using FIFA21 Data**  

🚀 **Predicting FIFA21 player market values using Machine Learning models (Linear Regression & SVM) on AWS SageMaker & EC2**  

## **Overview**  
This project aims to predict the market value of FIFA21 players based on attributes like **overall rating, potential, and skill moves**. Using **Machine Learning techniques (Linear Regression & Support Vector Machines - SVM)**, we analyze key player factors that influence valuation and provide insights for **football clubs’ scouting & investment decisions**.  

## **Project Workflow**  
### 🔹 **Data Collection & Processing**  
- Processed **18,000+ player records** with **100+ attributes** (market value, overall rating, wage, etc.).  
- Cleaned missing data using **KNN Imputer (15 nearest neighbors)**.  
- Encoded categorical variables with **Label Encoding & One-Hot Encoding**.  

### 🔹 **Model Development & Training**  
- Built and trained models using:  
  - **Linear Regression** (Baseline predictive model).  
  - **Support Vector Regression (SVR)** (For capturing complex patterns).  
- **Hyperparameter tuning with GridSearchCV** to optimize **C, epsilon, and kernel**.  

### 🔹 **Deployment & AWS Integration**  
- **Amazon SageMaker & EC2** used for scalable model training & inference.  
- Feature scaling with **StandardScaler** to normalize input data.  

### 🔹 **Evaluation & Results**  
| Metric | Linear Regression | SVM |  
|--------|------------------|-----|  
| **R² Score** | **96.95%** | **96.86%** |  
| **Mean Absolute Error (MAE)** | 0.3548 | 0.3070 |  
| **Root Mean Squared Error (RMSE)** | 0.8300 | 0.8425 |  

### 🔹 **Insights & Visualization**  
- Identified **top 10 most valuable players & clubs** based on market value.  
- **Heatmaps & correlation analysis** show key player attributes affecting market value.  

## **Technologies Used**  
✅ **Machine Learning**: Scikit-Learn, NumPy, Pandas  
✅ **Cloud & Deployment**: Amazon SageMaker, EC2  
✅ **Data Processing**: KNN Imputation, Label Encoding, One-Hot Encoding  
✅ **Hyperparameter Tuning**: GridSearchCV  
✅ **Visualization**: Matplotlib, Seaborn  
✅ **Model Evaluation Metrics**: R², MAE, MSE, RMSE  

## **How to Run the Project**  
1️⃣ Clone the repository:  
   ```bash
   git clone https://github.com/yourusername/fifa21-ml-prediction.git
   cd fifa21-ml-prediction
