# Georgia Climate Trend Dashboard (1900 - Present)
An independent data science and analytics project designed to clean, process, and visually map long-term localized climate variations across major regional centers in Georgia.

## 🔗 Live Interactive Dashboard
👉 **View the Live App:** [Click Here to Open the Interactive Graph](https://github.io)

---

## 🛠️ Tech Stack & Methodology
* **Language:** Python 3.x
* **Data Engineering:** `pandas` (with safe processing chunk loops to manage heavy row parsing without system memory failure)
* **Statistical Modeling:** Calculated rolling **5-Year Moving Averages** to filter seasonal noise and isolate macro-level temperature anomalies.
* **Interactive Frontend:** Deployed using custom `Plotly Express` line chart layering with optimized CDN script delivery for fast cross-browser performance.

---

## 📊 Dataset & Pipeline Overview
This project targets the **Berkeley Earth Surface Temperature Dataset**, which compiles over 1.6 billion global temperature registries. 

To overcome system limitations and regional file truncation bugs common in large data lakes, this pipeline directly queries the comprehensive `GlobalLandTemperaturesByCity.csv` registry. The backend loop isolates and aggregates historical coordinates across major urban hubs—including **Atlanta, Savannah, Augusta, and Columbus**—translating Celsius metrics into an intuitive regional Fahrenheit index from 1900 through the modern era.

---

## ⚙️ How to Run Locally
1. Clone this repository to your local system.
2. Ensure you have the required dependencies installed:
   ```bash
   pip install pandas plotly
   ```
3. Place the `GlobalLandTemperaturesByCity.csv` dataset into your root folder.
4. Execute the analysis pipeline script:
   ```bash
   python climate_tracker.py
   ```
