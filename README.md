# 🚗⚡ Tesla EV Growth Strategy · Washington EV Hub
### Explore how supercharger expansion unlocks EV adoption across Washington State.

Welcome to the **Washington EV Hub**, a simulation platform that lets you explore how different levels of Tesla supercharger expansion influence **EV growth**, **adoption behavior**, and **policy readiness** across all 39 Washington counties.

These tools combine population density, existing infrastructure, and adoption forecasting to reveal where chargers can create the **biggest jump in EV registrations**—and where they are failing to keep up.

### 🌐 Access the EV Forecast Tools  
👉 **Home Page — Choose Statewide or County-Level Tool**  
https://home-page-ev.onrender.com/  

Here you can:
- Model *statewide* EV adoption under different supercharger build-out scenarios  
- Explore *county-level* infrastructure gaps  
- See which counties benefit most from each new charger  
- Understand how supercharger expansion drives EV adoption all the way to 2050  

---

## 🔍 Why This Project Is Useful — EV Growth Starts With Charging

EV adoption does not grow in a vacuum—it grows where charging access exists. This project helps uncover exactly where Washington’s infrastructure is holding EV adoption back, and how strategic supercharger expansion can unlock the state's climate goals.

### The platform highlights critical insights such as:

### **Infrastructure Gaps**
- Dense counties where charging availability is clearly insufficient  
- Areas where **high population + low charger count** create high charging anxiety  
- Counties underserved due to **corridor-first planning**, not population-first planning  

### **Forecasting EV Growth from Charging Expansion**
- How EV registrations increase with every additional supercharger  
- How adoption rates shift upward as access improves  
- Whether counties are *on track* or falling behind 2030–2050 climate mandates  

### **Planning, Budgeting & ROI**
- Allocate charger budgets based on population demand  
- Prioritize counties where chargers yield the **largest adoption boosts**  
- Compare ROI for charger deployments between counties  
- Determine how many chargers are needed statewide to meet policy targets  

This transforms complex demographic + behavioral modeling into a tool that planners, utilities, and strategists can use to make **real-world decisions**.

---

## 🧠 How the Model Was Developed

This forecasting engine combines demographic analysis, infrastructure mapping, and probabilistic modeling.

### **1️⃣ Establishing the Baseline**
We analyzed:
- County-level population density  
- 2024 EV registration counts  
- Existing Tesla supercharger locations  
- Washington climate mandates (2030, 2040, 2050)

### **2️⃣ Creating County Prototypes**
Using population density and adoption behavior, four “prototype” county types were identified:
- High density  
- Medium density  
- Low density  
- Sparse  

Each of the 39 Washington counties was assigned to a prototype based on population cutoffs.

### **3️⃣ Monte Carlo + Time-Series Modeling**
For each prototype:
- Ran Monte Carlo simulations  
- Extended forecasts from **2024 → 2050**  
- Modeled behavioral response to charging access  

### **4️⃣ Pre-Generated Forecast Formulas**
From the modeling outputs:
- Built cubic curves for **EV Registrations vs Superchargers**  
- Built logistic curves for **Adoption Rate vs Superchargers**  
- Exported formulas into Excel for fast evaluation in the deployed app  

These formulas power the interactive forecasting tools—no heavy computation required at runtime.

---

## 🧭 Explore the Code (3 Repositories)

### 🏠 **Home Hub — Main Landing Page**  
- Repo: https://github.com/judyc4986/ev_home_hub  

### 🌎 **Statewide Forecast Tool**  
- Repo: https://github.com/judyc4986/ev_render_app  

### 🗺️ **County-Level Forecast Tool**  
- Repo: https://github.com/judyc4986/ev_forecast_app  

---

### 🧩 Site Flow & Architecture Overview

The diagram below shows how a user moves from the **Home Hub** to either the **Statewide** or **County-Level** tools, and then into the forecast results.

                             +----------------------+
                             |       Home Hub       |
                             +----------+-----------+
                                        |
                +-----------------------+-----------------------+
                |                                               |
  +----------------------------+             +-----------------------------+
  |   Statewide Forecast Tool  |             |  County-Level Forecast Tool |
  |       (ev_render_app)      |             |      (ev_forecast_app)      |
  +-------------+--------------+             +--------------+--------------+
                |                                             |
                +--------------------------+------------------+
                                           |
                                 +---------+---------+
                                 |     Forecast      |
                                 |      Results      |
                                 | (EV Registrations |
                                 |    & Adoption)    |
                                 +-------------------+









