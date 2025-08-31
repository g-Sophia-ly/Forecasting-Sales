本仓库包含两个基于机器学习的预测项目：  
This repository contains two machine learning prediction projects:  

1. **二手车价格预测 | Car Price Prediction**  
2. **销售预测（线性回归模型） | Sales Forecasting with Linear Regression**  

---

## 🚗二手车价格预测 | Car Price Prediction

### 项目概述 | Project Overview
本项目通过机器学习模型预测二手车价格，依据车辆品牌、型号、年份、行驶里程以及燃料类型等特征。  
This project builds a machine learning model to predict the price of used cars based on their attributes such as brand, model, year, mileage, and fuel type.  

整个流程包括数据清洗、探索性数据分析（EDA）、特征编码、模型训练与评估。  
The pipeline includes data cleaning, exploratory data analysis (EDA), feature encoding, model training, and evaluation.  

---

### 技术栈 | Tech Stack
- `Pandas, NumPy`：数据清洗与预处理 | Data cleaning and preprocessing  
- `Matplotlib, Seaborn`：数据可视化 | Visualization  
- `Scikit-learn`：OneHotEncoder, ColumnTransformer, Pipeline, Linear Regression  

---

### 关键步骤 | Key Steps
1. 数据清洗 → 处理缺失值、重复值与异常值  
   Data Cleaning → Removing missing values, duplicates, and outliers  

2. 探索性数据分析（EDA）→ 统计特征、分布与相关性  
   Exploratory Data Analysis (EDA) → Summary statistics, distributions, and correlations  

3. 特征工程 → 对 `name`、`company`、`fuel_type` 进行 OneHot 编码  
   Feature Engineering → Encoding categorical features (`name`, `company`, `fuel_type`) with OneHotEncoder  

4. 模型构建 → 使用 `Pipeline` 将预处理与线性回归结合  
   Model Building → Using `Pipeline` to combine preprocessing and Linear Regression  

5. 模型评估 → 在不同随机划分下计算 R² 分数，选择表现最优的模型  
   Model Evaluation → Calculating R² score across different random splits to select the best model  

6. 模型保存 → 使用 `pickle` 保存训练好的模型，方便后续调用  
   Model Saving → Exporting the trained model with `pickle` for future predictions  

---

### 结果 | Results
最优线性回归模型的 R² 分数达到 **0.86**，说明预测效果良好。  
The best Linear Regression model achieved an R² score of **0.92**, indicating strong predictive performance.  

---

## 📈销售预测项目（线性回归模型）  
## Sales Forecasting with Linear Regression

本项目旨在使用线性回归模型对历史销售数据进行时间序列建模与未来销售预测。  
This project uses a linear regression model to perform time-series forecasting on historical sales data.

---

### 项目目标 | Project Objectives

- 将原始日销售数据按月聚合处理  
  Aggregate daily sales data into monthly periods
- 利用 `LinearRegression` 建立预测模型  
  Build a prediction model using `LinearRegression` from scikit-learn
- 可视化对比实际值与预测值  
  Visualize and compare actual vs. predicted sales over time

---

### 3 技术栈 | Tech Stack

- `pandas`：数据处理 | Data manipulation  
- `numpy`：数值计算 | Numerical computing  
- `scikit-learn`：线性回归建模与数据归一化 | Modeling & scaling  
- `matplotlib`：可视化销售趋势 | Visualization of trends

---

### 示例输出 | Sample Output

- 显示 2017 年每月销售预测与实际值对比曲线  
  Shows monthly sales predictions vs actuals for 2017  
- 模型预测趋势与实际变化基本一致  
  Model captures the overall upward/downward sales trend

---

### 后续优化 | Future Improvements

- 引入 MAE / RMSE 评估指标 | Add MAE / RMSE evaluation metrics  
- 比较其他算法如 XGBoost 或 ARIMA | Compare with XGBoost or ARIMA  
- 多门店或多品类预测分析 | Multi-store or multi-item segmentation  
- 增加预测不确定性分析 | Add confidence interval or error bounds

---

