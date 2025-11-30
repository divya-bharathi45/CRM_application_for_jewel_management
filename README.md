# CRM Application for Jewel Management (Salesforce Project)

### Project Overview
The **CRM Application for Jewel Management** is a Salesforce-based system designed to automate jewellery business operations such as **Customer Orders**, **Item Management**, and **Billing**. This project integrates **custom objects**, **automated email flows**, and **custom reports** to ensure efficient management of customer interactions, item tracking, and billing communication.

---

##  Key Features

1. **Customer Order Management** – Store and track jewellery orders from customers.  
2. **Item Management** – Maintain detailed records of ornaments, types, weights, and prices.
3. **Billing Management** – Create bills automatically linked to items and orders.  
4. **Automated Email Notifications** – Trigger emails to customers when billing is created or updated.  
5. **Custom Reports** – Generate combined reports showing Billings, Items, and Customer Orders.  
6. **Error Handling** – Flow gracefully manages missing or invalid field data.

---

## Objectives

- Automate the billing and notification process using Salesforce Flow.  
- Build strong relationships between Customer Order, Item, and Billing objects.  
- Generate real-time analytical reports to support decision-making.  
- Improve customer communication through instant email notifications.  
- Eliminate manual billing errors and streamline jewellery business processes.

---

##  Tools & Technologies Used

| Category | Tools/Technologies |
|-----------|--------------------|
| **CRM Platform** | Salesforce Lightning |
| **Automation** | Record-Triggered Flow |
| **Reporting** | Custom Report Types, Dashboards |
| **Design** | Schema Builder, ER Diagrams |
| **Documentation** | Google Docs, Word, GitHub |
| **Collaboration** | SmartInternz Platform |

---

##  System Architecture
Customer Order → Item → Billing → Flow Trigger → Email → Report

**Objects and Relationships:**
- **Billing → Item (Lookup Relationship)**
- **Item → Customer Order (Lookup Relationship)**  
- **Customer Order → Customer (Lookup Relationship)**

 Data flows seamlessly through Salesforce to maintain data integrity and automate operations.

---

##  Modules in the System

| Module | Description |
|---------|-------------|
| **Customer Management** | Stores customer details and manages relationships. |
| **Item Management** | Tracks jewellery item details like type, ornament, weight, and price. |
| **Billing** | Generates billing records linked to items and customer orders. |
| **Email Automation** | Sends billing confirmation emails via Salesforce Flow. |
| **Reports & Dashboards** | Visualizes business insights for admins and owners. |

---

##  Flow Logic (Automation)

**Trigger:** When a Billing record is Created or Updated  
**Flow Type:** Record-Triggered Flow  
**Actions:**
1. Fetch related Item and Customer details  
2. Use Text Template for Email Body  
3. Send Email → Customer’s registered Email ID  

**Email Template Body Example:**
Hello,

Customer Name: {!$Record.Item__r.Customer_Name__r.Name}

Here are your purchase details:
Item Type: {!$Record.Item__r.Item_Type__c}
Ornament: {!$Record.Ornament__c}
Weight: {!$Record.Weight__c} grams
Amount: {!$Record.Amount__c}

##  Conclusion

The CRM Application for Jewel Management efficiently automates jewellery store operations. It provides a reliable, accurate, and automated approach to managing customer orders, items, and billing while maintaining seamless customer communication.  This Salesforce solution reduces manual effort, improves operational transparency, and enhances business decision-making.

##  Author

**Name:** : Divya Bharathi M, Ancy Rani T, Dhanuja Ancy D, HariDevi G   
**Role:** : Salesforce Developer  
**Institution:** : Einstein College Of Engineering 
**Team ID:** :  4CF9B0641590872B2C04C54C5A691F2E
**Email:** : divyabharathimmk4547@gmail.com
**GitHub:** : https://github.com/divya-bharathi45/CRM_application_for_jewel_management.git


