# 🏨 BEDSPACE PROJECT - Hostel & PG Management System

> A complete MySQL 8.0 database project for managing hostel/PG bookings, beds, tenants, payments and complaints.

*🔗 Repository:* https://github.com/ajaypinapatruni-commits/BEDSPACE_PROJECT

<br>

# 📌 Project Overview
---
BEDSPACE is designed to digitize hostel and PG operations. It handles users, hostels, rooms, beds, amenities, bookings, and payments and automates business logic using advanced MySQL features.

<br>

# 🎯 Objectives
---
- To develop a centralized database for hostel and PG management.
- To automate bed allocation and prevent double-booking / overbooking.
- To maintain complete user history, bookings, and payment records.
- To generate revenue reports and occupancy reports easily.
- To reduce manual work for hostel owners using Views, Procedures and Triggers.
- To ensure data integrity using Foreign Keys and Constraints.

<br>

# ✨ Features
---
- *8 Normalized Tables* - 3NF compliant design
- *Relationships* - Proper Foreign Keys linking all modules
- *Views* - For available beds, monthly revenue, user history
- *Stored Procedures* - For booking a bed, checkout, payment entry
- *Triggers* - Auto-update bed availability after booking
- *ENUM & Constraints* - For gender, room sharing, payment status

<br>

# 🗄️ Database Structure (8 Tables)
---

### 1. users - Tenant / User details
- Stores name, email, phone, gender, city

### 2. hostels - Hostel/PG details
- Stores name, type (PG/Hostel/Co-Living), city, rating, total_rooms

### 3. amenities - Facilities master
- Stores WiFi, Food, AC, Laundry etc with category and icon

### 4. hostel_amenities - Hostel wise amenities mapping
- Links hostels and amenities, is_free flag

### 5. rooms - Rooms in each hostel
- Stores room_type (1/2/3/4 Sharing), rent_per_bed, capacity, floor

### 6. beds - Individual beds
- Stores bed_number, is_available, is_ac

### 7. bookings - Booking history
- Links user, bed, hostel with check_in, check_out, status

### 8. payments - Rent and deposit payments
- Stores booking_id, amount, method (UPI/Card/Cash), status

<br>

# 🚀 How to Run
---
1.  Clone this repo:
    git clone https://github.com/ajaypinapatruni-commits/BEDSPACE_PROJECT.git
2.  Open MySQL Workbench
3.  Create database and run all CREATE TABLE queries



# ⚠️ Limitations
---
- Currently backend-only project (No Frontend UI / Website yet).
- Payment gateway integration is not included, only payment records.
- No user authentication / login system.
- Notification system (SMS/Email alerts for rent due) not implemented.
- Room availability check needs trigger enhancement.

<br>

# 🔮 Future Enhancements
---
- Develop a Web Application using React + Node.js.
- Add User Login for Owners and Tenants with Role-Based Access.
- Integrate Online Payment Gateway (UPI, Razorpay, Stripe).
- Add Real-time Bed Availability Dashboard with Charts.
- Implement Automated Rent Reminders via Email / SMS.
- Add Aadhaar / KYC Verification and Document Upload Feature.
- Mobile App for Tenants to Raise Complaints and Pay Rent.

<br>

# 🏁 Conclusion
---
The BEDSPACE project successfully demonstrates how MySQL can be used to solve real-world hostel management problems. By using 8 normalized tables, foreign keys, and ENUM constraints, the system ensures data accuracy and prevents manual errors. This project is a strong foundation that can be scaled into a full-stack product.

<br>

# 👨‍💻 Author
---
*Ajay Pinapatruni* <br>
GitHub: @ajaypinapatruni-commits ee data vundi andulo