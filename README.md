# Exploratory Data Analysis (EDA) Summary ✈ Flight Delay Prediction 
This EDA bridges technical data patterns with practical airline operations strategy — paving the way for a robust, business-impacting flight delay prediction system.
# 📌 Objective
The goal of this project is to analyze flight operation, weather, and scheduling data to identify patterns and drivers of departure delays (≥15 minutes).
These insights guide predictive modeling and business decision-making for airlines and airports.
Machine Learning model to predict flight delays using real 2019 airline data, with potential application in passenger insurance schemes.

# 🗂 Dataset Overview
Size: ~6.5M flight records

Features: 26 variables covering:

Time & Schedule: Month, Day of Week, Time Block, Segment Number

Operations: Concurrent Flights, Seats, Airport/Airline Monthly Volumes

Aircraft: Carrier, Plane Age, Capacity

Location: Departing Airport, Previous Airport, Coordinates

Weather: Temperature, Wind, Precipitation, Snow

Target: DEP_DEL15 — 1 if delayed ≥15 mins, else 0

# Data Quality:
✅ 100% complete — no missing values detected.
📊 Both categorical and numerical features available for modeling.

# 🔍 Key EDA Insights
## 1. Traffic & Schedule Patterns
Seasonality: Summer (26.4%) and Spring (25.3%) see the highest flight volumes — peak planning needed.

Monthly Trends: Slight dips in Jan–Feb; peaks in Jul–Oct for demand and operations.

Day-wise Distribution: Flights evenly spread across days; no extreme weekday/weekend skew.

Time of Day: Morning & midday blocks dominate departures; lowest traffic late at night.

Operational Takeaway: Congestion risk is time-driven, not day-driven — staffing should follow daily peaks.


## 2. Weather Impact
Delays are more frequent with:

Higher wind speeds

Greater precipitation

More snow & snow depth

Temperature alone has little impact.

Season Link: Winter delays correlate strongly with snow amount; summer snow impact = 0.

Business Move: Prioritize weather-response operations (de-icing crews, weather monitoring) in winter and during high-wind/rain events.


## 3. Operational Congestion Risk
Delayed flights average:

Higher concurrent flights

Busier airports (monthly flight volume)

Higher passenger throughput

Delay likelihood increases with later flight segments, especially for short-haul routes (delay propagation effect).

Business Move: Improve turnaround efficiency and scheduling buffers for aircraft later in their daily cycle.


## 4. Carrier & Airport Insights
Top Airlines by Flight Share: Southwest (20%), American (14%), Delta (14%), United (9%), SkyWest (9%).

High-volume carriers contribute most to overall system delays — improvement here has maximum business impact.

Busiest airports (e.g., ATL, SLC) require priority congestion mitigation.


## 5. Delay Pattern Hotspots
Heatmap Findings: Delay rates spike in afternoon/evening time blocks across all days.

On-Time Reliability: Highest in early morning; premium/business flights could be strategically scheduled here.

## 6. Feature Relationships
Strong relationships:

Airport flights ↔ Concurrent flights

Passenger volumes ↔ Airline/Airport scale

Weak correlations indicate features bring unique predictive value (useful for ML without redundancy).

# 📈 Business Takeaways
Congestion & weather are the biggest drivers; day of week plays a small role.

Proactive delay management should focus on:

Afternoon/evening peak hours

High-traffic airports and carriers

Winter weather disruptions

Flights later in aircraft’s operational day

Data supports a predictive model that blends operational load, schedule position, and weather context.













