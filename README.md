# AIRLINE MARKET INSIGHTS AND PRICING ANALYSIS

# ✈️ AIRLINE MARKET INSIGHTS AND PRICING ANALYSIS

**Overview**  
Analyzed 300,000+ Indian airline records using Python and SQL to uncover pricing trends, route demand, and travel patterns, with complete data cleaning, feature engineering, EDA, and visualizations to support data-driven airline optimization.

---

## 📂 Dataset (used in this project)

- **Filename:** `airlines_flights_data.csv`  
- **Total Records:** ~300,000+ (as used during analysis)  
- **Core Features:** `Airline`, `Source` / `Origin`, `Destination`, `Date_of_Journey`, `Dep_Time`, `Arrival_Time`, `Duration`, `Total_Stops`, `Price`, `Route`, `Class` (if present)



---

## 🔄 Project Workflow

1. **Data Loading**
   - Loaded the uploaded CSV into pandas (Colab path: `/content/airlines_flights_data.csv` or from Google Drive).
2. **Data Cleaning**
   - Handled missing/null values
   - Standardized `Date_of_Journey`, `Dep_Time`, `Arrival_Time`
   - Cleaned and converted `Duration` to numeric minutes
   - Removed duplicates and invalid rows
3. **Feature Engineering**
   - Extracted `day`, `month`, `year`, `weekday`
   - Derived `time_of_day` buckets (Morning/Afternoon/Evening/Night)
   - Created `route_code` and `is_weekend` flags
   - Season and holiday indicators (where applicable)
4. **Exploratory Data Analysis (EDA)**
   - Price distributions, airline-wise averages, class-wise comparisons
   - Route popularity and frequency
   - Stops vs price, duration vs price
   - Time-based trends (month/day/hour)
5. **Visualization**
   - Bar charts, boxplots, histograms, heatmaps
   - Interactive charts with Plotly (optional)
   - Bar charts were used for category comparisons, boxplots for price variability and outliers, histograms for price distribution, heatmaps for correlation analysis, and Plotly was used to create interactive visualizations for better insight exploration.
6. **Insights & Reporting**
   - Peak/off-peak travel windows
   - Popular and least popular routes
   - Pricing anomalies and seasonality
   - Recommendations for scheduling and pricing strategy

---

## 📌 Key Findings (from the uploaded data)

- **Direct (non-stop) flights** generally command higher prices but save significant time.  
- **Weekend and holiday periods** show clear price spikes.  
- **Business-class** fares have wider variability than economy.  
- Certain **metro-to-metro routes** show the highest frequency and demand.  
- Number of stops and duration are strong predictors of price differences.

*(These findings reflect the patterns observed in `airlines_flights_data.csv` used for analysis.)*

---

## 🛠 Tools & Libraries

- **Environment:** Google Colab / Jupyter Notebook  
- **Languages & Libraries:** Python, pandas, numpy, matplotlib, seaborn, plotly (optional), pandasql (optional)  
- **Files in repo:** `airlines_flights_data.csv`, `AIRLINE_MARKET_INSIGHTS_AND_PRICING_ANALYSIS.ipynb`, `README.md`, `/visuals` (optional)

---

## 📁 Project Structure (recommended)

├── data/
│ └── airlines_flights_data.csv
├── notebooks/
│ └── AIRLINE_MARKET_INSIGHTS_AND_PRICING_ANALYSIS.ipynb
├── visuals/
│ └── figures_and_charts.png
├── requirements.txt
└── README.md


---

## ▶️ How to run (Google Colab)

1. Open `AIRLINE_MARKET_INSIGHTS_AND_PRICING_ANALYSIS.ipynb` in Google Colab.  
2. Upload `airlines_flights_data.csv` to Colab (or mount Google Drive and update path). Example to mount Drive:
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   df = pd.read_csv('/content/drive/MyDrive/path/to/airlines_flights_data.csv')

#Install any missing libraries:

!pip install pandas plotly pandasql

#Run all cells (Data cleaning → Feature engineering → EDA → Visualizations).

-->Conclusion

This project analyzes flight data to understand pricing trends, demand patterns, and route popularity.
Using Python, the data was cleaned, explored, and visualized to uncover meaningful insights.
The findings reveal peak travel times, popular routes, and key factors affecting ticket prices.
Overall, the analysis helps airlines and stakeholders make better, data-driven decisions.





