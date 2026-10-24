# Logistics Delivery Time Analysis — Dataset

This folder contains the dataset used for the **Logistics Delivery Time Analysis** project. The dataset is designed to analyze delivery performance, delivery delays, transportation costs, traffic conditions, weather conditions, and vehicle usage.

## 📊 Dataset Overview

The dataset contains **500 delivery records** collected over the period:

**1 January 2026 – 29 June 2026**

Each row represents one delivery order.

| Property | Details |
|---|---|
| Total Records | 500 |
| Total Features | 11 |
| Date Range | Jan 2026 – Jun 2026 |
| Average Distance | 255.90 km |
| Average Order Value | ₹7,265.20 |
| Average Promised Time | 419.99 minutes |
| Average Actual Time | 422.44 minutes |
| Average Delivery Cost | ₹475.19 |
| On-Time Deliveries | 47% |
| Delayed Deliveries | 53% |

## 📁 Files

```text
data/
├── logistics_delivery_data.csv
└── README.md
```

### `logistics_delivery_data.csv`

The main dataset used for exploratory data analysis, visualization, and delivery-time analysis.

## 🧾 Dataset Features

| Column | Description | Data Type |
|---|---|---|
| `order_id` | Unique identifier for each delivery order | String |
| `order_date` | Date on which the order was placed/delivered | Date |
| `distance_km` | Delivery distance in kilometers | Numeric |
| `traffic_level` | Traffic condition during delivery | Categorical |
| `weather` | Weather condition during delivery | Categorical |
| `vehicle_type` | Vehicle used for the delivery | Categorical |
| `order_value_inr` | Value of the order in Indian Rupees | Numeric |
| `promised_delivery_minutes` | Delivery time promised to the customer | Numeric |
| `actual_delivery_minutes` | Actual time taken for delivery | Numeric |
| `delivery_cost_inr` | Cost of completing the delivery in Indian Rupees | Numeric |
| `delivery_status` | Final delivery status | Categorical |

## 🚦 Traffic Levels

The dataset contains three traffic categories:

- **Low**
- **Medium**
- **High**

Distribution:

| Traffic Level | Records |
|---|---:|
| Low | 155 |
| Medium | 204 |
| High | 133 |

## 🌦️ Weather Conditions

The dataset includes different weather conditions that may affect delivery performance.

| Weather | Records |
|---|---:|
| Clear | 323 |
| Rain | 128 |
| Storm | 44 |

## 🚚 Vehicle Types

The dataset contains **3 different vehicle types**. Vehicle type can be analyzed to understand its relationship with:

- Delivery time
- Delivery cost
- Distance covered
- Delay frequency

## ⏱️ Delivery Performance

Delivery performance can be analyzed by comparing:

```text
Delay = Actual Delivery Time - Promised Delivery Time
```

A positive value indicates that the delivery took longer than promised.

The dataset contains:

- **47% On-Time deliveries**
- **53% Delayed deliveries**

This makes the dataset suitable for identifying factors contributing to delivery delays.

## 🔍 Possible Analysis

This dataset can be used for several analytical tasks:

### 1. Delivery Delay Analysis
Analyze the factors responsible for delayed deliveries.

### 2. Traffic Impact
Study how Low, Medium, and High traffic conditions affect delivery time.

### 3. Weather Impact
Compare delivery performance during Clear, Rain, and Storm conditions.

### 4. Distance vs Delivery Time
Analyze the relationship between delivery distance and actual delivery time.

### 5. Vehicle Performance
Compare different vehicle types based on:

- Average delivery time
- Average delivery cost
- Delay percentage
- Distance covered

### 6. Cost Analysis
Analyze the relationship between distance, vehicle type, and delivery cost.

### 7. Delivery Status Prediction
The dataset can also be used to develop a machine learning model for predicting whether a delivery will be **On Time** or **Delayed**.

## 📈 Suggested Visualizations

The following visualizations can be created using this dataset:

- Delivery Status Distribution
- Distance vs Actual Delivery Time
- Traffic Level vs Delivery Time
- Weather vs Delivery Delay
- Vehicle Type vs Delivery Cost
- Promised vs Actual Delivery Time
- Delivery Cost vs Distance
- Monthly Delivery Performance
- Average Delay by Traffic Level
- Average Delay by Weather Condition

## 🛠️ Technologies

The dataset can be analyzed using:

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook
- Scikit-learn

## 📌 Example Python Code

```python
import
