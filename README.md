# SQL Data Analysis: Order Acceptance, Customer Support Trends, and User Behavior  

## Overview  
This project demonstrates SQL-based data analysis techniques to extract insights from a dataset related to order fulfillment, customer support interactions, and user device trends. The queries explore key business questions, focusing on improving operational efficiency, understanding customer behaviors, and optimizing the user experience.  

---

## ⚠️ Disclaimer  
- **This dataset is private and not included in this repository.** The queries are written based on a real-world dataset, but the actual data cannot be shared.  
- **All data references have been fully randomized.** Any specific insights, names, categories, or numerical patterns do not reflect the real dataset. This project is designed purely to showcase SQL querying skills and analytical techniques.  

---

## 📌 Questions Addressed  

1. **Order Acceptance Trends** – What types of orders are accepted the most by couriers during peak hours? How can we maximize the number of accepted orders?  
2. **Customer Support Trends** – Is there a correlation between batched orders and customer support interactions? How can we minimize potential challenges?  
3. **Device Usage Trends** – What devices do the majority of customers use? How can we leverage this insight to optimize the user experience?  

---

## 📂 Repository Structure  

/sql-projects/ ├── Queries/ # Folder containing SQL queries │ ├── acceptance_trends.sql │ ├── customer_trends.sql │ ├── platform_usage.sql ├── Visualizations/ # Folder containing generated visualizations │ ├── Acceptance Rate vs. Meal Time.png │ ├── Orders by Device Type (%).png │ ├── Top 5 Contact Reasons.png ├── README.md # Project documentation

---

## 🛠️ Querying Approach and Visualizations  

### **1️⃣ Order Acceptance Trends**  
📌 *Goal:* Identify the most accepted order types by couriers during peak times and explore ways to improve overall acceptance rates.  

#### **Query Breakdown**  
- **Retrieve order data** to analyze different meal time categories.  
- **Identify peak order times** by counting total orders per category.  
- **Determine product category trends** by analyzing accepted vs. non-accepted orders.  
- **Calculate courier acceptance rates** for each meal time.  

📊 **Visualization:**  
![Acceptance Rate vs. Meal Time](Visualizations/Acceptance%20Rate%20vs.%20Meal%20Time.png)  

🔍 **Query File:** [`acceptance_trends.sql`](Queries/acceptance_trends.sql)  

---

### **2️⃣ Customer Support Trends**  
📌 *Goal:* Examine the relationship between batched orders and customer support inquiries to identify operational challenges.  

#### **Query Breakdown**  
- **Join orders with support contacts** to analyze customer complaints.  
- **Filter for fulfilled batched orders** to focus on completed deliveries.  
- **Group by contact reason** to determine common reasons for support cases.  

📊 **Visualization:**  
![Top 5 Contact Reasons](Visualizations/Top%205%20Contact%20Reasons.png)  

🔍 **Query File:** [`customer_trends.sql`](Queries/customer_trends.sql)  

---

### **3️⃣ Device Usage Trends**  
📌 *Goal:* Identify customer device usage patterns to optimize user experience and marketing efforts.  

#### **Query Breakdown**  
- **Retrieve session data** to analyze device types.  
- **Count sessions per device type** to determine user distribution.  
- **Calculate percentages** to understand overall platform trends.  

📊 **Visualization:**  
![Orders by Device Type (%)](Visualizations/Orders%20by%20Device%20Type%20(%25).png)  

🔍 **Query File:** [`platform_usage.sql`](Queries/platform_usage.sql)  

---

## 🔥 Key Takeaways  
- **Operational Efficiency:** Identifying acceptance rate patterns can inform strategies to improve order fulfillment.  
- **Customer Experience:** Support interactions can highlight underlying inefficiencies in order processing.  
- **Platform Optimization:** Device trends guide product enhancements and targeted marketing approaches.  

---

## 🚀 Future Enhancements  
- Conduct **time-series analysis** to track trends in order acceptance over different periods.  
- Use **machine learning models** to predict support contact likelihood based on order characteristics.  
- Perform **A/B testing** to evaluate the impact of different interventions on order acceptance rates.  

---

## 🔗 Contact  
For any questions or discussions about this project, feel free to reach out!
