# Uttar Pradesh Climate Change Authority (UPCCCE)

# **UP Climate Change Authority Dashboard**

## **📌 Overview**
**Shiny dashboard** built in **R** that provides **real-time and historical air quality data** for **Uttar Pradesh, India**. It integrates **geospatial mapping, data visualization, and interactive components** to offer a comprehensive **Air Quality Index (AQI) monitoring system**.

---

## **🎯 Project Objectives**
- **Visualize real-time and historical AQI** data across different cities and stations in Uttar Pradesh.
- **Track pollution trends** over time and compare **air quality across different locations**.
- **Help policymakers, researchers, and the public** access pollution data in an interactive manner.

---

## **📌 Features & Functionalities**

### **1️⃣ Live AQI Monitoring (Real-Time Analysis)**
- **Interactive Map using Leaflet**:
  - Displays AQI levels at different locations.
  - Users can hover over or click on a station to see detailed air quality data.
- **City and Station Rankings**:
  - Ranks **cities and stations based on AQI** levels.
  - Identifies the most and least polluted locations.
- **Pollutant Breakdown**:
  - Identifies predominant pollutants (PM2.5, PM10, NO2, SO2, CO, Ozone, etc.).
  - Displays percentage contribution of each pollutant.
- **Time-Series Data**:
  - Displays AQI trends for the past **48 hours** using Highcharts.
- **Filtering Options**:
  - **City Selection**
  - **Station Selection**
  - **Pollutant Type Selection**

### **2️⃣ Historical AQI Analysis**
- **Long-term AQI trends analysis**.
- **Filters Available**:
  - **City, Station, Year, and Month Selection**.
- **Time-Series Analysis**:
  - **Line charts for AQI trends** over time.
  - Allows users to select specific pollutants.
- **AQI by Area Type**:
  - Compares AQI in different types of areas (urban, rural, industrial).
- **Comparison of AQI Levels**:
  - Displays how different cities and stations compare over time.

---

## **🔧 Technical Implementation**

### **📂 Data Sources & Processing**
1. **Shapefiles for Mapping Uttar Pradesh Blocks**:
   - Uses **GIS data (`UP_Blocks.shp`)** to overlay AQI data on a map.
   - Processes spatial data using `rgdal`, `sf`, `rmapshaper`.

2. **Real-Time AQI Data (`df_2days5`)**:
   - Stored in **Parquet format**.
   - Contains AQI data for the past **48 hours**.
   - Integrated with **station latitude-longitude** data.

3. **Historical AQI Data (`aqi_historical.csv`)**:
   - Stores long-term AQI trends for **multiple years**.

4. **Data Cleaning & Transformation**:
   - Uses `dplyr`, `tidyr`, `stringr` for processing.
   - **Pivoting data (`pivot_longer()`, `pivot_wider()`)** for better visualization.
   - **Filtering & Ranking**:
     - Cities and stations ranked based on pollutant concentration.
     - Identifies the most polluted areas.

---

## **🖥️ User Interface**

![UPCCCE-project](UPCCCE GIS(Drill Down ).png)
### **📌 UI Components**
1. **Navbar Layout (`navbarPage()`)**
   - **Tabs:** "Live AQI" and "Historical AQI".
   - **Title:** "UP Climate Change Authority Dashboard".
   - Includes a **favicon (small logo)**.

2. **Interactive Map (Leaflet)**
   - Displays **real-time AQI data**.
   - Uses **color-coded markers**:
     - **Green** → Good AQI
     - **Yellow** → Moderate AQI
     - **Red** → Poor AQI

3. **Dynamic Filtering Options**
   - **City Selection (`pickerInput()`)**
   - **Station Selection**
   - **Pollutant Selection**
   - **Year & Month Selection** (for historical analysis)

4. **Data Tables (`Reactable`)**
   - Displays **AQI rankings** for cities and stations.
   - Can be sorted and searched dynamically.

5. **Charts (`Highcharter`)**
   - **Time-series graphs for AQI** trends.
   - **Pie charts for pollutant distribution**.
   - **Comparison of AQI levels in different areas**.

---

## **📜 Key Libraries Used**

### **📊 Data Processing**
- `dplyr` → Data manipulation.
- `tidyr` → Data transformation.
- `data.table` → Fast data processing.
- `jsonlite` → Handling JSON files.
- `arrow` → Reading and writing Parquet files.

### **🗺️ Spatial & Mapping**
- `Leaflet` → For interactive maps.
- `sf & rgdal` → Handling geospatial data.
- `rmapshaper` → Simplifying shapefiles.

### **📈 Visualization**
- `Highcharter` → Interactive charts.
- `Reactable` → Tables with sorting and filtering.
- `DT` → DataTables for structured views.

### **🎨 UI Components**
- `ShinyWidgets` → Enhanced UI controls.
- `ShinyJS` → JavaScript integration.
- `Shinydashboard` → Dashboard layout.
- `FontAwesome` → Icons for UI elements.
---

## **🎯 Conclusion**
This **Shiny dashboard** is a powerful **air quality monitoring tool** for **Uttar Pradesh**. It provides **real-time insights, historical analysis, and interactive visualizations** to help researchers, policymakers, and the general public **understand and track pollution trends**.

🚀 **This is a well-structured, data-driven project that makes environmental data accessible and actionable!**
![UPCCCE_GIS_DrillDown](https://github.com/user-attachments/assets/f9b0feb9-0a0e-40dd-aeb8-d0c444d6a4ad)
![UPCCCE_Air_Quality](https://github.com/user-attachments/assets/97cc383e-70e7-4e90-90e9-11785b0968ea)
![Wind_Speed](https://github.com/user-attachments/assets/d183e45c-eb3e-4581-bf85-dc46a66e6c1a)



