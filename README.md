# 🚗 Dynamic Pricing for Urban Parking Lots

A data-driven pricing engine for urban parking spaces, developed as part of the **Summer Analytics 2025** capstone project hosted by the **Consulting & Analytics Club × Pathway**.

## 📌 Project Objective

Urban parking lots often suffer from poor utilization due to static pricing. This project simulates a real-world dynamic pricing system using historical and real-time data to optimize pricing across 14 parking lots based on:

- Occupancy levels
- Queue length
- Traffic congestion
- Special days/events
- Vehicle type
- Competitor pricing (optional advanced model)

## 💡 Models Implemented

### ✅ Model 1: Baseline Linear Model
A simple model that adjusts price linearly based on current occupancy:
Price = Base Price + α × (Occupancy / Capacity)


### ✅ Model 2: Demand-Based Model
A more advanced model that factors in demand-affecting variables:
Demand = α × (Occupancy / Capacity) + β × Queue - γ × Traffic + δ × SpecialDay + ε × VehicleTypeWeight
Price = Base Price × (1 + λ × NormalizedDemand)

Prices are bounded between $5 and $20 to ensure stability.

### 🧪 Model 3 (Planned): Competitive Pricing Model
Adds location-based intelligence to adjust prices considering nearby lot prices and geographic distance. (To be implemented.)

## 📊 Visualizations

Interactive plots built using **Bokeh** to visualize pricing behavior across time for each lot:
- Compare Model 1 and Model 2 side by side
- Understand how price varies with demand and occupancy

## 🛠 Tech Stack

- Python
- Pandas, NumPy (model implementation)
- Bokeh (visualization)
- Google Colab (execution environment)
- [Pathway](https://pathway.com/) 





