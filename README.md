## 销售预测项目（线性回归模型）  
## Sales Forecasting with Linear Regression

本项目旨在使用线性回归模型对历史销售数据进行时间序列建模与未来销售预测。  
This project uses a linear regression model to perform time-series forecasting on historical sales data.

---

### 🎯 项目目标 | Project Objectives

- 将原始日销售数据按月聚合处理  
  Aggregate daily sales data into monthly periods
- 利用 `LinearRegression` 建立预测模型  
  Build a prediction model using `LinearRegression` from scikit-learn
- 可视化对比实际值与预测值  
  Visualize and compare actual vs. predicted sales over time

---

##3 🛠️ 技术栈 | Tech Stack

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

