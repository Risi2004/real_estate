# real_estate

A Java Spring Boot-based real estate web application for managing property listings, user bookings, payments, and owner-buyer communication — using **text file storage** instead of a traditional database.

---

## ✨ Features

### 🔐 User & Admin Management
- Register & login system
- Session-based authentication
- Admin dashboard with:
  - Total users
  - Total properties
  - Unread contact requests

### 🏡 Property Management
- Owners can **add**, **edit**, and **delete** properties
- Buyers can view property details
- Property attributes:
  - Location, Country, Price, Type (Sale/Rent), Size, Image
- Properties stored in `properties.txt`
- **Binary Search Tree (BST)** used for location-wise sorting
- **Quick Sort** used for sorting by price
- **Levenshtein Distance Algorithm** used for intelligent location-based search, allowing fuzzy search (e.g., "Colmbo" still finds "Colombo")

### 📩 Contact Owner Feature
- Contact form for buyers to message property owners
- Data stored in `contact.txt`
- Owners notified on login
- Admin view to **mark as read**

### 🧾 Booking System
- Buyers can book properties
- Booking details saved to `bookings.txt`
- Admin dashboard shows all bookings

### 💳 Payment Gateway (File-based)
- First-time property listing requires payment
- Payment form with:
  - Card masking
  - Expiry & CVV validation
- Details stored in `payments.txt`
- Unique invoice number per transaction
- **PDF receipt generated**

### 📬 Newsletter Subscription
- Visitors can subscribe via form
- Submissions stored in `newsletters_subscription.txt`

### ⭐ Customer Reviews
- Users can submit reviews from the homepage
- Stored in `reviews.txt`
- Dynamically displayed on home

### 🔍 Intelligent Search
- BST used for efficient property search by location
- **Levenshtein Distance** algorithm for fuzzy search results

---

## 🧠 Technologies Used

| Layer        | Tools                     |
|--------------|---------------------------|
| Backend      | Java, Spring Boot         |
| Frontend     | HTML, CSS, JavaScript     |
| Styling      | Custom CSS                |
| Storage      | File-based (`.txt` files) |
| Email        | JavaMailSender            |
| PDF Reports  | jsPDF                     |

---
