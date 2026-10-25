# 🏨 BEDSPACE PROJECT - Hostel & PG Management System

> A complete MySQL 8.0 database project for managing hostel/PG bookings, beds, tenants, payments and complaints.

### 🔗 Repository: https://github.com/ajaypinapatruni-commits/BEDSPACE_PROJECT

---

### 📌 Project Overview
BEDSPACE is designed to digitize hostel and PG operations. It handles property owners, hostels, rooms, beds, tenants, bookings, payments and automates business logic using advanced MySQL features.

### 🎯 Objectives
- To develop a centralized database for hostel and PG management.
- To automate bed allocation and prevent double-booking / overbooking.
- To maintain complete tenant history, bookings, and payment records.
- To generate revenue reports and occupancy reports easily.
- To reduce manual work for hostel owners using Views, Procedures and Triggers.
- To ensure data integrity using Foreign Keys and Constraints.

### ✨ Features
- **8 Normalized Tables** - 3NF compliant design
- **Relationships** - Proper Foreign Keys with ON DELETE CASCADE
- **Views** - For available beds, monthly revenue, tenant history
- **Stored Procedures** - For booking a bed, checkout, payment entry
- **Triggers** - Auto-update bed status, prevent overbooking
- **Functions & Indexes** - For fast searching and reporting

### 🗄️ Database Structure (8 Tables)
1. `owners` - Property owners details
2. `hostels` - Hostel/PG details linked to owners
3. `rooms` - Rooms in each hostel
4. `beds` - Individual beds with status (Available/Occupied)
5. `tenants` - Tenant / Student details
6. `bookings` - Booking history with check-in/check-out
7. `payments` - Rent and deposit payments
8. `complaints` - Tenant complaints & resolution

### 🚀 How to Run
1. Clone this repo:
   git clone https://github.com/ajaypinapatruni-commits/BEDSPACE_PROJECT.git
2. Open MySQL Workbench
3. Create database and run:
   SOURCE BEDSPACE_V2.sql;

### ⚠️ Limitations
- Currently backend-only project (No Frontend UI / Website yet).
- Payment gateway integration is not included, only payment records.
- No user authentication / login system for tenants and owners.
- Notification system (SMS/Email alerts for rent due) not implemented.
- Supports single location management only.

### 🔮 Future Enhancements
- Develop a Web Application using React + Node.js / Python Django.
- Add User Login for Owners and Tenants with Role-Based Access.
- Integrate Online Payment Gateway (UPI, Razorpay, Stripe).
- Add Real-time Bed Availability Dashboard with Charts.
- Implement Automated Rent Reminders via Email / SMS.
- Add Aadhaar / KYC Verification and Document Upload Feature.
- Mobile App for Tenants to Raise Complaints and Pay Rent.

### 🏁 Conclusion
The BEDSPACE project successfully demonstrates how MySQL can be used to solve real-world hostel management problems. By using normalized tables, views, stored procedures, and triggers, the system ensures data accuracy, prevents manual errors, and provides valuable business insights. This project is a strong foundation that can be scaled into a full-stack product.

### 👨‍💻 Author
**Ajay Pinapatruni**
GitHub: @ajaypinapatruni-commits