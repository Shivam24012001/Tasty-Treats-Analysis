# 🍽️ Tasty Treats - Customer Segmentation & Cancellation Analysis

## 🎯 Project Goal

To improve customer satisfaction and reduce online food order cancellations at Tasty Treats, a modern restaurant in Bangalore. This project involves cleaning the data, analyzing cancellation trends, segmenting customers using RFM analysis, and developing a dynamic Excel dashboard for insights and decision-making.

## 🧾 Dataset Provided

* **RFM\_Segmentation.csv**: Contains predefined customer segmentation based on RFM scores.
* **Message.csv**: Contains tailored messages based on major cancellation reasons.
* **Raw Data tab in Excel**: All order-level details including order status, delivery status, and feedback.

## 🛠️ Tools Used

* Microsoft Excel
    * Pivot Tables & Charts
    * Conditional Formatting
    * Data Validation & Dropdowns
    * Dynamic Named Ranges
    * Lookup Functions (VLOOKUP/XLOOKUP)
    * IF, AND, OR, TEXTJOIN, COUNTIF formulas

## ✅ Task Breakdown

### 📌 Task 1: Data Preparation

#### 🧹 Step 1: Data Cleaning
* Add a tab: **Data Cleaning**
* Clean raw order-level data.
* Fix missing values, formatting issues, and inconsistent item names.

#### 📦 Step 2: Order Data Extraction
* Add tab: **Order\_data**
* Extract item price & category.
* Calculate **Item Total** = Quantity \* Price.

### 📌 Task 2: Cancellation Analysis

#### 📍 Step 1: Cancellation Report
* Add tab: **Cancellation Report**
* Analyze cancellation reasons dark store-wise.
* Use pivot tables for summarized metrics.

#### 📊 Step 2: Sales Dashboard
* Add tab: **Sales Dashboard**
* Highlight dark stores with high cancellation rates.
* Create dynamic report with dropdown-based filtering by store.
* Add **Feedback Cause Analysis**:
    * Two most frequent cancellation causes.
    * Dynamic highlight for high-rate causes.

### 📌 Task 3: RFM Segmentation

#### 📥 Step 1: Import RFM\_Segmentation.csv
* Add tab: **Segment Table**
* Load customer segmentation mapping.

#### 📊 Step 2: Create RFM Segmentation Table
* Add tab: **RFM Segmentation**
* For each customer:
    * Calculate: **Recent Visit Date**, **Frequency**, **Monetary**, **Recency** (in days).

#### 🔢 Step 3: RFM Score Calculation
* Add tab: **RFM Score Calculation**
* Calculate:
    * Mean, Deviation, Mean±Deviation for Recency, Frequency, Monetary
    * Apply scoring logic (1 to 3 scale)
    * Assign customer segment based on RFM Score:
        * Top-tier Customers
        * Loyal Customers
        * Potential Loyal Customers

### 📌 Task 4: Champion Customer Analysis Dashboard

#### 📋 Step 1: Dashboard Creation
* Add tab: **Champion Customer Analysis**
* Use dropdown to select customer category.
* Create dynamic “**Delivery Status Report**”:
    * Last 5 orders per customer.
    * Highlight cancelled: Red (#ea9999), delivered: Green (#d9ead3)
    * Tag: “Consecutive Cancellation” or “No Consecutive Cancellation”

#### 💬 Step 2: Feedback Analysis
* Dynamically list:
    * Customers with cancelled orders
    * Their feedback count & types
    * Highlight **Major Issues** (most frequent excluding “change of plan”)

#### 📈 Step 3: Category-wise Feedback
* Show total feedback frequency per type for selected segment.

### 📌 Task 5: Personalized Messaging

#### 📥 Step 1: Import Message.csv
* Add tab: **Message**

#### 📨 Step 2: Customized Messaging Report
* Add tab: **Customized Message**
* Dynamically update based on:
    * Customers with consecutive cancellations or last cancellation
    * Match **Major Issues** from feedback
    * Fetch matching messages from **Message.csv**

### 📊 Example Screenshots

* **Sales Dashboard with filters**
* **RFM Score Table**
* **Delivery Status Highlighting**
* **Dynamic Feedback Analysis**
* **Customized Messages for Issues**



## 🎯 Key Insights

* **Dark stores with highest cancellation rate**: (e.g., Whitefield, Koramangala)
* **Major reasons**: Delayed delivery, item out of stock
* **Top-tier customers** experienced fewer cancellations
* Customers with recurring issues now receive **tailored communication**

## 📬 Future Enhancements

* Integration with Power BI for real-time updates and more advanced visualizations.
* Predictive analytics to forecast potential cancellations and proactively address them.
* Development of personalized loyalty campaigns based on RFM segments to improve customer retention.
