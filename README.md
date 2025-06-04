
# 📊 NYC Taxi Data Dashboard

This project is a **Streamlit dashboard** for analyzing and visualizing **NYC Yellow Taxi trip data** (January–June 2023). It features dynamic insights on trip frequency, fare composition, taxi zones, and pickup-dropoff patterns.

---

## 🚀 Features

- **Monthly Overview**: Total trips, distance, and fare analysis.
- **Trip Distribution**: Day-wise and time-of-day patterns.
- **Zones Dashboard**: Zone-wise pickup/dropoff details, maps, passenger stats.
- **Fare Breakdown**: Components like fare, tip, surcharge, MTA tax, etc.
- **Trip Planner**: Top 5 recommended drop-off zones per selected pickup location.

---

## 🌐 Data Source

All trip data is publicly available via the **NYC Taxi & Limousine Commission (TLC)**:

🔗 [NYC TLC Trip Record Data](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page)

> 📥 Download monthly Yellow Taxi data for **2023** in CSV format (e.g., `yellow_tripdata_2023-01.csv`, `yellow_tripdata_2023-02.csv`, etc.).

---

## 📁 Project Structure

```
project/
├── devlab.py                   # Streamlit dashboard script
├── /taxi/                      # Folder with downloaded monthly CSVs
├── /taxinyc/                   # Contains taxi_zones.shp (shapefile)
├── frequency_table.csv         # Used for trip planner feature
└── README.md                   # This file
```

---

## 🛠️ Installation & Usage

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/nyc-taxi-dashboard.git
   cd nyc-taxi-dashboard
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Ensure the following files and folders exist:**
   - `/taxi/`: Contains Yellow Taxi monthly data for 2023
   - `/taxinyc/taxi_zones.shp`: NYC Taxi Zones shapefile
   - `frequency_table.csv`: Dropoff frequency matrix

4. **Run the dashboard**
   ```bash
   streamlit run devlab.py
   ```

---

## 📋 Requirements

Create a `requirements.txt` with:

```txt
streamlit
pandas
plotly
matplotlib
seaborn
numpy
geopandas
streamlit-option-menu
pydeck
```
