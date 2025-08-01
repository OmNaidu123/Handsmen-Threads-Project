# Handsmen-Threads-Project
HandsMen Threads' Salesforce-powered solution transforms data management and customer engagement with intelligent automation, a clean user interface, and scalable backend support. Designed to improve business operations, enhance customer satisfaction, and maintain accurate inventory across the organization.

## 🚀 Key Features

### 🧱 Robust Data Modeling
- Custom Objects and Relationships designed to support complex business entities including Manufacturing, Customers, and Orders.

### ✅ UI-Based Data Integrity
- Real-time validation using **Validation Rules** and **Record-Triggered Flows** to ensure accurate and consistent data entry.

### 📧 Email Automation
- **Order Confirmations**: Triggered via Flow post-purchase to confirm orders instantly.
- **Stock Alerts**: Automated email alerts to warehouse when inventory (via custom thresholds) falls below 5 units.

### 🏆 Dynamic Loyalty Program
- Loyalty tiers are auto-assigned using **Flows** or **Apex Triggers** based on customer purchase history.

### ⏰ Scheduled Order Processing
- Uses **Scheduled Apex** or **Batch Jobs** to:
  - Update bulk orders
  - Sync inventory records
  - Reconcile financial data
  - All scheduled at midnight daily for optimal performance

---

## 🛠️ Tech Stack
- Salesforce Lightning Platform
- Flows, Apex, Process Builder
- Custom Objects & Fields
- Scheduled & Batch Apex
- Email Alerts & Notifications

## 📦 Objects Overview

| Object Label          | Type           | Description                                         |
|-----------------------|----------------|-----------------------------------------------------|
| HandsMen Customer     | Custom Object  | Stores customer details and loyalty status          |
| HandsMen Orders       | Custom Object  | Captures order records with totals and customer ref |
| HandsMen Products     | Custom Object  | Holds product catalog, pricing, and stock levels    |
| Inventorys            | Custom Object  | Tracks available stock and warehouse assignments    |
| Marketing Campaigns   | Custom Object  | Manages promotions and targeted marketing efforts   |


---

## ⚙️ Flows & Automation

- ✅ **Order Confirmation Flow** *(Record-Triggered)*  
  Sends confirmation email to customers immediately after order creation.

- ⚠️ **Stock Alert Flow** *(Scheduled Flow)*  
  Triggers automated alert when product stock drops below 5 units.

- 🧠 **Loyalty Update Flow** *(Apex Trigger)*  
  Dynamically updates customer loyalty status based on purchase history.

- 🌙 **Midnight Batch Job** *(Apex Batch Class)*  
  Handles bulk processing of orders, inventory updates, and financials during off-peak hours.

---

## 💌 Email Templates

### 🔹 Order Confirmation Email  
- Uses dynamic merge fields: `Customer Name`, `Order Total`, and `Item List`.

### 🔸 Stock Alert Email  
- Automatically sent to the warehouse team for proactive inventory control.

---

## 📈 Business Impact
- Enhanced data consistency
- Faster order processing
- Improved customer satisfaction
- Scalable architecture ready for growth
