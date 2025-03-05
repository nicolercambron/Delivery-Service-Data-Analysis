# Delivery-Service-Data-Analysis

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

## 🛠️ Querying Approach

### **Q1: Order Acceptance Trends**
📌 *Goal:* Identify the most accepted order types by couriers during peak times and explore ways to improve overall acceptance rates.

#### **Query Breakdown**
1. **Understanding the Data Structure**  
   - Retrieved a sample of records to inspect available columns.
   - Identified relevant fields such as `meal_time_category`, `product_category`, and `accepted_time`.

2. **Identifying Peak Order Times**  
   - Queried the number of total orders by meal time category.
   - Sorted results in descending order to determine high-traffic periods.

3. **Analyzing Product Category Trends**  
   - Focused on orders during a selected meal time (`Meal Time A`).
   - Counted orders per product category to see what items are ordered the most.

4. **Calculating Courier Acceptance Rates**  
   - Joined `orders_table` and `assignments_table` to connect order details with acceptance status.
   - Computed the acceptance rate per meal time category.

#### **Analysis**
- The results highlight variations in order acceptance across different time periods.
- Understanding courier behavior allows for optimization strategies, such as adjusting incentives or modifying order batching techniques.
- While some meal times might have higher order volumes, they may also experience lower acceptance rates, requiring targeted interventions.

---

### **Q2: Customer Support Trends**
📌 *Goal:* Examine the relationship between batched orders and customer support inquiries to identify operational challenges.

#### **Query Breakdown**
1. **Exploring Customer Support Data**  
   - Joined the `orders_table` with `support_contacts` to link order fulfillment with customer interactions.
   - Retrieved a sample of records to review available support case details.

2. **Filtering for Relevant Orders**  
   - Focused only on **fulfilled** and **batched** orders to analyze their impact on customer support cases.

3. **Grouping by Contact Reasons**  
   - Counted the number of unique orders for each customer support contact reason.
   - Sorted by frequency to determine the most common issues.

#### **Analysis**
- Various factors contribute to customer interactions, and a deeper analysis of operational workflows may help identify opportunities for improvement.
- Additional investigation could uncover areas for efficiency improvements and customer experience enhancements.

---

### **Q3: Device Usage Trends**
📌 *Goal:* Identify customer device usage patterns to optimize user experience and marketing efforts.

#### **Query Breakdown**
1. **Understanding Available Fields**  
   - Queried a sample of the `customer_sessions` table to inspect available data on device usage.

2. **Counting Sessions by Device Type**  
   - Aggregated session counts for each device category.
   - Calculated the percentage of total sessions attributed to each device type.

#### **Analysis**
- Device trends provide insights into user engagement patterns, helping businesses tailor experiences for different platforms.
- Platform-specific optimizations, such as app performance improvements or UI/UX adjustments, can enhance the customer experience.
- Understanding device distribution also informs marketing strategies, ensuring targeted outreach on the most relevant platforms.

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
