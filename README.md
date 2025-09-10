# 🌦️ Overfit & Chill – Dual-Task ML Model  

Overfit & Chill is a dual-task machine learning project built for **IRIS Kaggle Clash #3 (Aug 2025)**.  
It predicts both **precipitation (regression)** and **electricity shutdown events (classification)** using time-series weather data.  

To balance performance across tasks, it introduces a **custom evaluation metric**:  

\[
\text{Score} = \text{RMSE} \times (1 - \text{F1})
\]  

This ensures accuracy in continuous rainfall predictions while maintaining fairness in outage classification.  

---

## 🚀 Features  
- 🌧️ **Regression** – Predicts precipitation in millimeters  
- ⚡ **Classification** – Forecasts whether a power outage occurs  
- 📊 **Custom Metric** – RMSE × (1 – F1) for dual-task evaluation  
- 📈 **Benchmarking** – Compared hand-tuned models vs. AutoML (Auto-sklearn)  
- ⚖️ **Imbalance Handling** – Applied threshold tuning for better F1-scores  
- 🗂️ **End-to-End ML Pipeline** – Preprocessing, feature engineering, modeling, evaluation  

---

## 🛠️ Tech Stack  
- **Python** – Core development  
- **Pandas / NumPy** – Data processing & feature engineering  
- **scikit-learn** – Model training and evaluation  
- **Matplotlib** – Data visualization  
- **Auto-sklearn** – Automated model benchmarking  

---

## 📌 Limitations  
- Dataset limited to weather and environmental indicators from the competition.  
- Electricity shutdown events were **class-imbalanced**, requiring extra tuning.  
- Model not yet deployed — results are for **experimental and educational purposes**.  

---

## 🔮 Future Improvements  
- Integrate **LSTMs or Transformers** for advanced time-series forecasting.  
- Experiment with **ensemble methods** to boost accuracy across both tasks.  
- Automate **hyperparameter optimization** beyond AutoML defaults.  
- Deploy as a **web app dashboard** for real-time weather–outage predictions.  

---

## 📬 Contact  
Made by **@vaetheneeb** for IRIS Kaggle Clash #3.  
Feel free to fork, explore, and suggest improvements! 🚀  
