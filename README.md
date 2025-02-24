# Uttar Pradesh Climate Change Authority (UPCCCE)

## **📌 Overview**  
The **UP Climate Change Authority Dashboard** is a **web-based analytical tool** designed to provide **real-time and historical air quality insights** for **Uttar Pradesh**.  

Built using **R Shiny**, it integrates **GIS-based visualizations** and **live CPCB API data** to help policymakers and researchers monitor **air pollution trends** and make data-driven decisions.  

### **🌍 Dashboard Sections:**  
1️⃣ **Air Quality Overview** – GIS-based station mapping with live AQI updates.  
2️⃣ **Air Quality Live** – Dynamic charts displaying real-time air quality trends.  
3️⃣ **Air Quality Historical** – Long-term air quality trend analysis with interactive visuals.  

---

## **📊 Key Features & Functionalities**  

### **1️⃣ Air Quality Overview**  
- **GIS-based map** showing air quality monitoring stations.  
- **Color-coded AQI levels** for quick pollution severity assessment.  
- **Hourly AQI updates** sourced directly from CPCB APIs.  

### **2️⃣ Air Quality Live**  
- **Interactive charts** displaying **24-hour average AQI trends**.  
- **Pollutant concentration trends** analyzed at the **city and station level**.  
- **Real-time data streaming** from CPCB APIs.  

### **3️⃣ Air Quality Historical**  
- **Multi-year historical AQI trends** for long-term analysis.  
- **Interactive visualizations**, including:  
  - 📊 **Monthly AQI trends**  
  - 🌍 **Wind speed & direction charts**  
  - 📈 **Annual pollutant concentration trends**  
  - 🔍 **Yearly AQI averages**  

### **4️⃣ Data Processing & Real-Time API Integration**  
- **Live data retrieval** from CPCB-authorized APIs.  
- **Historical data aggregation & transformation** for trend analysis.  
- **Caching mechanisms** for optimized performance.  

---

## **📌 Air Quality Parameters Monitored**  
✔ **Observation Time** (Real-time timestamp)  
✔ **Air Quality Index (AQI)** (24-hour rolling average)  
✔ **Uptime of the station** (PM2.5-based metric)  
✔ **Pollutant Concentrations** – PM2.5, PM10, NO2, SO2, O3, CO  
✔ **Meteorological Conditions** – Temperature, Humidity, Wind Speed  

---

## **🛠️ Technical Implementation**  

### **1️⃣ Data Processing Pipeline**  
✅ **Real-time data fetching** from CPCB APIs.  
✅ **Optimized data storage** using **Feather & Parquet files**.  
✅ **High-speed processing** with **Apache Spark & Arrow**.  

### **2️⃣ Data Quality & Preprocessing**  
- **Automated data profiling** to detect inconsistencies.  
- **Geospatial data cleaning & interpolation** to fill missing sensor data.  
- **Time-series smoothing techniques** for enhanced accuracy.  

### **3️⃣ Interactive Dashboard & GIS Integration**  
- 🌍 **Leaflet-based GIS visualizations** for **spatial pollution analysis**.  
- 📊 **Highcharter** for advanced time-series & comparative analysis.  
- 🔢 **Reactable** for interactive tabular data visualization.  

### **4️⃣ Modular & Scalable Dashboard Architecture**  
- **Encapsulated features within R Shiny modules** for reusability.  
- **Reactive expressions** enable **dynamic updates**.  
- **Robust error handling & caching** ensure smooth functionality.  

### **5️⃣ Deployment & Performance Optimization**  
- 🚀 **Deployed on Shinyapps.io** with security measures.  
- 🌐 **Load balancing & caching** for improved scalability.  
- ⚡ **Optimized API requests** using `httr` for high-performance data retrieval.  
---
# Key Libraries Used  

The project is built using multiple R packages:  

## 📊 Data Processing  
- **dplyr** → Data manipulation.  
- **tidyr** → Data transformation.  
- **data.table** → Fast data processing.  
- **jsonlite** → Handling JSON files.  
- **arrow** → Reading and writing Parquet files.  

## 🗺️ Spatial & Mapping  
- **Leaflet** → For interactive maps.  
- **sf** & **rgdal** → For handling geospatial data.  
- **rmapshaper** → For simplifying shapefiles.  

## 📈 Visualization  
- **Highcharter** → Interactive charts.  
- **Reactable** → Tables with sorting and filtering.  
- **DT** → DataTables for structured views.  

## 🎨 UI Components  
- **ShinyWidgets** → Enhanced UI controls.  
- **ShinyJS** → JavaScript integration for interactivity.  
- **Shinydashboard** → Dashboard layout.  
- **FontAwesome** → Icons for UI elements.  

## **🎯 Conclusion**
This **Shiny dashboard** is a powerful **air quality monitoring tool** for **Uttar Pradesh**. It provides **real-time insights, historical analysis, and interactive visualizations** to help researchers, policymakers, and the general public **understand and track pollution trends**.

🚀 **This is a well-structured, data-driven project that makes environmental data accessible and actionable!**
![UPCCCE_GIS_DrillDown](https://github.com/user-attachments/assets/e9141856-154e-4ac6-b3f7-4b1a43860f60)
![UPCCCE_Air_Quality](https://github.com/user-attachments/assets/6bc208df-5901-4008-959f-dc9887a3aec4)
![Wind_Speed](https://github.com/user-attachments/assets/75b64bb6-5165-449e-adda-c256cb38c4b9)





