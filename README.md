# Network-Fault-Prediction-Using-Time-Series
Built a time series-based fault prediction model for telecom towers using signal strength, weather, and tower logs. Integrated ARIMA and anomaly detection to proactively identify outages, demonstrating a use case for telecom OSS systems like those managed by organizations.

# 📡 Network Fault Prediction Using Time Series
Predicting telecom tower outages using historical logs, weather data, and time series modeling.

# 📁 Project Overview
Telecom network outages cause service disruptions and revenue loss. This project uses time series forecasting and anomaly detection techniques to proactively predict telecom tower faults using synthetic and real-world data inputs. The goal is to support telecom OSS (Operations Support Systems) like those used by Amdocs.

# 🎯 Objectives
Forecast faults/outages at a tower level using historical data

Detect abnormal behavior in network KPIs like signal strength

Combine weather patterns, signal metrics, and geographic context

Visualize fault trends and real-time risk using dashboards

# 📊 Data Sources
Source	Description
tower_logs.csv	Historical fault logs with timestamps, tower IDs, error types
signal_data.csv	RSSI, SNR, and RSRP collected per tower
weather_data.csv	Weather parameters (rain, humidity, temperature) per location
tower_metadata.csv	Tower location, type, region classification
⚠️ Note: Synthetic datasets created for simulation. Real-world extensions possible with telecom APIs.

# 🛠️ Technologies Used
Python (Pandas, NumPy, Scikit-learn, Statsmodels, TensorFlow/Keras)

Time Series Models: ARIMA, SARIMA, Facebook Prophet, LSTM

Anomaly Detection: Isolation Forest, Autoencoders

Visualization: Matplotlib, Seaborn, Plotly, Power BI

Deployment: Streamlit (optional), Power BI dashboard

Tools: Jupyter, GitHub

# 🔍 Exploratory Data Analysis (EDA)
Daily/Hourly fault trends across regions

Signal vs. Fault correlation heatmaps

Weather overlay on fault frequency

Rolling window feature engineering (lag values, moving average)

# 🧠 Modeling Approach
📈 Time Series Forecasting
Built ARIMA/SARIMA models to forecast daily fault counts per tower

Used Facebook Prophet with weather & signal as regressors

Trained LSTM models for sequence-based forecasting

# 🚨 Anomaly Detection
Used Isolation Forest and autoencoders to detect sudden signal degradation or fault spikes

Combined outputs with forecasts to increase robustness

# 📐 Evaluation Metrics
Model	MAE	RMSE	Accuracy (Anomaly Detection)
ARIMA	X.XX	X.XX	-
Prophet	X.XX	X.XX	-
LSTM	X.XX	X.XX	-
Autoencoder	-	-	XX%
Note: Exact values depend on dataset and configuration

📊 Power BI / Streamlit Dashboard
Features:

Fault forecasts for each tower

Region-wise map of fault risk score

Historical signal strength trends

Anomaly flags on time series plots


# 📁 Project Structure
kotlin

Copy

Edit

network-fault-prediction/
│
├── data/
│   ├── tower_logs.csv
│   ├── signal_data.csv
│   ├── weather_data.csv
│   └── tower_metadata.csv
│
├── notebooks/
│   ├── eda.ipynb
│   ├── arima_model.ipynb
│   ├── lstm_model.ipynb
│   └── anomaly_detection.ipynb
│
├── dashboard/
│   └── fault_prediction_dashboard.pbix
│
├── requirements.txt
└── README.md
# ✅ Key Outcomes
Predictive modeling framework for proactive network fault handling

Scalable approach to integrate multiple towers and geographic zones

Amdocs-ready solution for OSS analytics and telecom diagnostics

# 🚀 Future Enhancements
Real-time data ingestion using Kafka or APIs

Geo-spatial modeling using satellite/tower coordinates

Model monitoring and alerting system with Grafana or Airflow

# 📬 Contact
Mayur Salunke
Data Scientist | https://www.linkedin.com/in/mayursalunke04/ 
For collaboration or deployment inquiries
