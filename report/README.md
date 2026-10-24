# 📊 Logistics Delivery Performance Analysis and Delay Investigation

## Week 1 Internship Project Report

This report presents the **Week 1 strategic planning and exploratory data analysis** for a Logistics Data Science project focused on understanding delivery delays, delivery reliability, and operating costs.

The project uses **Python and a simulated dataset of 500 delivery records** covering January–June 2026. The analysis investigates delivery performance across traffic levels, weather conditions, vehicle types, months, and distance categories.

---

## 👨‍💻 Project Information

| Details | Information |
|---|---|
| **Intern** | Rohan Sandip Nikam |
| **Role** | Logistics Data Analyst Intern |
| **Organization** | YuvaIntern |
| **Internship Period** | 22 October 2026 – 19 November 2026 |
| **Project** | Logistics Delivery Performance Analysis and Delay Investigation |
| **Report** | Week 1 – Strategic Planning and Data Exploration |
| **Dataset** | 500 simulated delivery records |
| **Period Covered** | January – June 2026 |

The report was prepared as a Python Data Science project using Python, Pandas, NumPy, Matplotlib, Seaborn, Google Colab, and GitHub.

---

## 🎯 Project Objective

The primary objective is to explore delivery and contextual data to:

- Measure delivery reliability.
- Identify patterns associated with delivery delays.
- Analyze important logistics KPIs.
- Compare delivery performance across operational conditions.
- Define a roadmap for future delay prediction.
- Support future delivery-planning and optimization decisions.

The Week 1 scope focuses on **strategic planning, data exploration, descriptive analysis, and methodology planning**. Predictive modeling and deployment are planned for future phases.

---

## 📁 Project Structure

```text
Logistics-Delivery-Time-Analysis/
│
├── data/
│   ├── logistics_delivery_data.csv
│   └── README.md
│
├── notebooks/
│   ├── logistics_delivery_analysis.ipynb
│   └── README.md
│
├── report/
│   ├── Week1_Logistics_Strategic_Planning_Report.docx
│   └── README.md
│
└── README.md
```

---

## 📊 Dataset

The working dataset contains:

- **500 rows**
- **11 columns**
- Delivery records from **January to June 2026**
- One row represents one delivery order.

The dataset is **simulated and intended for educational purposes**.

### Dataset Features

| Feature | Description |
|---|---|
| `order_id` | Unique delivery order identifier |
| `order_date` | Date the order was recorded |
| `distance_km` | Delivery distance |
| `traffic_level` | Low, Medium, or High |
| `weather` | Clear, Rain, or Storm |
| `vehicle_type` | Bike, Van, or Truck |
| `order_value_inr` | Order value in INR |
| `promised_delivery_minutes` | Promised delivery duration |
| `actual_delivery_minutes` | Actual delivery duration |
| `delivery_cost_inr` | Delivery operating cost |
| `delivery_status` | On Time or Delayed |



---

# 📈 Key Results

## Overall Delivery Performance

| KPI | Result |
|---|---:|
| Total Deliveries | **500** |
| On-Time Deliveries | **235 (47.00%)** |
| Delayed Deliveries | **265 (53.00%)** |
| Average Actual Delivery Time | **422.44 minutes** |
| Average Delivery Cost | **INR 475.11** |
| Average Delay | **2.45 minutes** |

These KPIs establish the initial performance baseline for future analysis and improvement.

---

## 🚦 Traffic Analysis

Traffic showed one of the strongest associations with delivery delays.

| Traffic Level | Delayed | On Time | Avg. Delay |
|---|---:|---:|---:|
| High | **87.22%** | 12.78% | **25.12 min** |
| Medium | 59.31% | 40.69% | 3.22 min |
| Low | 14.19% | **85.81%** | **-18.52 min** |
| Unknown | 75.00% | 25.00% | 12.62 min |

High-traffic deliveries had the highest delay rate and average delay, while low-traffic deliveries were early on average.

---

## 🌧️ Weather Analysis

| Weather | Average Delay |
|---|---:|
| Storm | **28.59 min** |
| Unknown | 18.00 min |
| Rain | 10.38 min |
| Clear | **-4.49 min** |

Storm conditions had the highest average delay, while clear-weather deliveries were early on average. These are **descriptive associations rather than proof of causation**.

---

## 🚚 Vehicle Analysis

| Vehicle | Delayed | On Time |
|---|---:|---:|
| Bike | **50.81%** | 49.19% |
| Van | 52.92% | 47.08% |
| Truck | **55.15%** | 44.85% |

Truck deliveries had the highest delay rate, while bikes had the lowest. However, the differences are relatively modest, so vehicle type alone should not be considered the cause of delays.

---

## 📅 Monthly Analysis

| Month | Delayed | On Time |
|---|---:|---:|
| January 2026 | 46.15% | 53.85% |
| February 2026 | **61.33%** | 38.67% |
| March 2026 | **45.56%** | 54.44% |
| April 2026 | 54.55% | 45.45% |
| May 2026 | 57.45% | 42.55% |
| June 2026 | 54.79% | 45.21% |

February recorded the highest delay rate, while March recorded the lowest. Because the dataset covers only six months and is simulated, this should not be interpreted as a recurring seasonal pattern.

---

## 📍 Distance Analysis

| Distance Category | Delayed | On Time |
|---|---:|---:|
| Short | 40.95% | **59.05%** |
| Medium | 56.15% | 43.85% |
| Long | 56.23% | 43.77% |

Medium- and long-distance deliveries showed higher delay rates than short-distance deliveries. However, medium and long categories were nearly identical, so delay does not increase steadily with distance.

---

# 🔎 Delayed vs On-Time Deliveries

| Status | Orders | Avg. Distance | Avg. Cost | Avg. Actual Time |
|---|---:|---:|---:|---:|
| Delayed | 265 | 266.26 km | INR 502.64 | 448.53 min |
| On Time | 235 | 244.21 km | INR 444.06 | 393.02 min |

Delayed orders had higher average distance, delivery cost, and actual delivery time compared with on-time orders. These comparisons identify areas for further investigation but **do not establish causation**.

---

# 🧠 Proposed Data Science Methodologies

The report proposes the following approaches for future project phases:

### 1. Exploratory Data Analysis
Analyze distributions and relationships between operational variables and delivery outcomes.

### 2. Classification
Predict whether a delivery will be **On Time** or **Delayed**.

Possible evaluation metrics:

- Precision
- Recall
- F1-score
- Confusion Matrix
- ROC-AUC

### 3. Regression
Predict:

- Actual delivery duration
- Delay duration

Evaluation metrics:

- MAE
- RMSE
- R²

### 4. Clustering
Identify groups of deliveries with similar operational characteristics.

### 5. Optimization
Explore route, departure-time, and vehicle-allocation decisions subject to operational constraints.

---

# 🗺️ Strategic Roadmap

The proposed project workflow consists of eight stages:

```text
Business Understanding
        ↓
Data Collection
        ↓
Data Understanding
        ↓
Data Preparation
        ↓
Exploratory Data Analysis
        ↓
Predictive Modeling
        ↓
Model Evaluation
        ↓
Operational Recommendations
```

The roadmap emphasizes understanding the business problem first, preparing reliable data, exploring patterns, building appropriate models, evaluating them against baselines, and finally translating validated results into operational recommendations.

---

# 🛠️ Technologies Used

- 🐍 Python
- 🐼 Pandas
- 🔢 NumPy
- 📊 Matplotlib
- 📈 Seaborn
- 🤖 Scikit-learn
- ☁️ Google Colab
- 🐙 GitHub
- 📓 Jupyter Notebook

---

# 🧹 Data Cleaning

The Week 1 analysis includes:

- Duplicate-row checking
- Missing-value analysis
- Missing traffic values → `Unknown`
- Missing weather values → `Unknown`
- Missing delivery costs → Median imputation
- Date conversion to datetime
- Creation of `delay_minutes`

The dataset contained **0 duplicate rows**, 8 missing traffic values, 5 missing weather values, and 4 missing delivery-cost values before cleaning.

---

# ⚠️ Important Modeling Consideration

`actual_delivery_minutes` should not be used as an input feature when predicting delivery delay **before the delivery is completed**, because it contains information from the outcome.

The report also notes that route optimization would require additional information such as:

- Origin/destination coordinates
- Road-network travel times
- Vehicle capacity
- Delivery time windows

These fields are not available in the current dataset.

---

# 💡 Preliminary Recommendations

Based on the Week 1 analysis:

1. Review high-traffic dispatch periods and validate appropriate time buffers.
2. Investigate whether storm conditions require additional delivery buffers.
3. Investigate medium- and long-distance routes.
4. Track on-time rate, delay rate, average delivery time, and delivery cost together.
5. Collect route-level timestamps and operational information before making major staffing or fleet-allocation decisions.

---

# ⚠️ Limitations

- The dataset is simulated.
- Associations do not prove causation.
- Only January–June 2026 is represented.
- Missing traffic/weather categories have limited observations.
- GPS coordinates are not available.
- Route sequences are not available.
- Driver and warehouse information is not available.
- No predictive model has been completed in Week 1.
- No route-optimization algorithm has been implemented yet.

---

# 🏁 Conclusion

The Week 1 project analyzed **500 simulated logistics delivery records** using Python-based data science techniques.

The initial analysis found:

- **47.0%** of deliveries were on time.
- **53.0%** were delayed.
- High traffic showed the strongest delay pattern.
- Storm conditions showed the highest average delay.
- Medium and long-distance deliveries had higher delay rates than short-distance deliveries.

These findings provide a starting point for future predictive modeling and logistics optimization. However, the results should first be validated using real operational data before being used for business decisions.

---

## 📄 Full Report

The complete Week 1 report is available in this folder:

```text
report/
└── Week1_Logistics_Strategic_Planning_Report.docx
```

For the supporting analysis, see:

```text
notebooks/
└── logistics_delivery_analysis.ipynb
```

For the dataset, see:

```text
data/
└── logistics_delivery_data.csv
```

---

## 📚 References

1. World Bank — *Logistics Performance Index 2023*
2. Rokoss et al. (2024) — *Case study on delivery time determination using a machine learning approach in small batch production companies*
3. Kaggle — *Package delivery time prediction*

The report explicitly notes that the numerical results come from the project's **simulated educational dataset**, while the external references support the background and methodology discussion.

---

## 👨‍💻 Author

**Rohan Sandip Nikam**

**Logistics Data Analyst Intern**

**YuvaIntern**

> *Strategic Planning and Data Exploration — Week 1*
