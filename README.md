# **Weather Data Analysis using Python**

### **Exploratory Data Analysis (EDA) | Feature Engineering | Time-Series Trends | Visual Insights**

This project analyzes historical hourly weather data to uncover **seasonal patterns**, **temperature behavior**, **visibility changes**, and **frequencies of major weather events** such as fog, rain, snow, and storms.
It demonstrates end-to-end data analyst skills including **data cleaning**, **preprocessing**, **feature engineering**, **visualization**, and **insight generation**.

---

## 📌 **Project Objectives**

* Clean and preprocess raw weather data
* Handle missing values and detect outliers
* Perform EDA using Python
* Engineer new features such as:

  * Year, Month, Day, Hour
  * Weekday
  * Temperature in Fahrenheit
  * Weather Category
* Analyze seasonal temperature patterns
* Visualize distribution and frequency of weather events
* Generate insights useful for forecasting or reporting

---

## 🧰 **Technologies Used**

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **Jupyter Notebook**
* **Power BI (Optional)**

---

## 📂 **Project Structure**

```
Weather-Data-Analysis/
│── 1. Weather Data.csv                   # Raw dataset
│── weather_data_analysis.ipynb           # Main analysis notebook (with summary)
│── Weather_Data_Analysis_Dashboard.pbix  # Power BI dashboard
│── README.md                             # Project documentation
│── venv/                                 # Virtual environment (ignored in repo)
```

---

## 🔧 **Data Cleaning & Preprocessing**

Steps performed:

* Converted **Date/Time** into Pandas datetime format
* Checked missing values and applied **forward fill (ffill)**
* Handled outliers using **Z-Score**
* Created new useful columns:

  * `Year`, `Month`, `Day`, `Hour`
  * `Weekday`
  * `Temp_F` (°C → °F)
  * `Weather_Category` (Fog, Rain, Snow, Cloudy, Clear, etc.)

---

## 📊 **Key Visualizations**

* Temperature distributions
* Boxplots for detecting outliers
* Weather Category Frequency Heatmap
* Monthly Temperature Trend line chart
* Correlation heatmap of all numerical variables

---

## 🧠 **Insights Generated**

* **Temperature peaks** around **July–August** and reaches the lowest around **January**.
* **Visibility drops sharply** during foggy months (especially winter).
* **Snowfall frequency** is highest between **December–February**.
* **Clear weather** dominates summer months, while **fog** dominates winter.
* Rain and snow show strong **seasonal patterns**, supporting predictive forecasting.

---

## 📝 **How to Run the Project**

### **1) Clone the repository**

```bash
git clone https://github.com/JithendraTechie/Weather-Data-Analysis.git
```

### **2) Install dependencies**

```bash
pip install pandas numpy matplotlib seaborn scipy jupyter
```

### **3) Run Jupyter Notebook**

```bash
jupyter notebook
```

Open:
`weather_data_analysis.ipynb`

---

## 📈 **Power BI Dashboard (Optional)**

Data Transformation in Power BI

After loading clean_weather_data.csv into Power BI:

1️⃣ Promoted Headers

Convert first row to headers.

2️⃣ Corrected Data Types

Date/Time → datetime

All numeric columns → decimal number

Weather → text

3️⃣ Added DAX Columns
Month Name
MonthName = FORMAT(WeatherData[Date_Time], "MMMM")

Month Number
MonthNumber = MONTH(WeatherData[Date_Time])

Sort MonthName by MonthNumber

Power BI → Column tools → Sort by Column → MonthNumber

📈 Step 3 – Power BI Dashboard
✔ Dashboard Components
🔹 KPI Cards

Average Temperature (°C)

Average Relative Humidity (%)

Average Visibility (km)

Total Records

🔹 Line Charts

Average Temperature by Month

Average Humidity by Month

Average Visibility by Month

Average Pressure by Month

🔹 Donut Chart

Distribution of Weather Types

🔹 Slicers

Month Name

Weather Type

📌 Step 4 – Insights & Interpretation
🌡 Temperature

Average temperature: 8.8°C

Warmest months: July & August

Coldest months: January & February

💧 Humidity

Peaks during June–August

Drops sharply in October

👁 Visibility

Lowest in winter months (fog)

Highest in summer

🌬 Pressure

Highest in December

Lowest during mid-year

🌦 Weather Types

Mostly Mainly Clear, Mostly Cloudy, and Cloudy

Fog accounts for ~4% → impacts visibility in January

Open Power BI File
Weather_Data_Analysis_Dashboard.pbix

Interact with Dashboard

Use slicers to filter by:

Month

Weather

---

## 🚀 **What This Project Demonstrates (Resume Points)**

* Performed **end-to-end EDA on 8,700+ hourly weather records**
* Engineered multiple time-series features using Python
* Identified patterns in **temperature, humidity, pressure, and visibility**
* Created visual insights for **seasonal forecasting**
* Built a **Power BI dashboard** for business-ready presentation

---

## 📬 **Contact**

If you'd like to collaborate or have feedback, connect with me on GitHub.

https://github.com/JithendraTechie

---
