# ALX Airbnb Backend System – User Stories

## Overview
This document outlines the main user stories for the ALX Airbnb Clone backend system.  
Each story captures a system interaction from the perspective of key actors and includes acceptance criteria written in the **Given / When / Then** format.

---

## Guest User Stories

### 1. User Registration
**As a guest, I want to create an account so that I can book properties and manage my profile.**

**Acceptance Criteria**
- **Given** I am on the registration page,  
- **When** I provide my valid name, email, password, and other required information,  
- **Then** my account should be created successfully and I should receive a confirmation email.

---

### 2. User Login
**As a guest, I want to log into the system so that I can access my bookings and saved properties.**

**Acceptance Criteria**
- **Given** I already have an account,  
- **When** I enter valid login credentials,  
- **Then** I should be logged in and redirected to my dashboard.  
- **And** if I enter invalid credentials, I should see an appropriate error message.

---

### 3. Property Search and Filtering
**As a guest, I want to search and filter properties by location, price, and date so that I can find suitable accommodations.**

**Acceptance Criteria**
- **Given** I am on the property search page,  
- **When** I enter a location, check-in/check-out dates, and optional filters,  
- **Then** the system should display a list of matching properties with pagination.

---

### 4. Property Booking
**As a registered guest, I want to book a property so that I can reserve it for specific dates.**

**Acceptance Criteria**
- **Given** I am logged in and viewing a property,  
- **When** I select my desired dates and confirm payment,  
- **Then** the booking should be saved and marked as confirmed,  
- **And** I should receive a booking confirmation notification.

---

### 5. Leave a Review
**As a guest, I want to leave a review for a property after my stay so that I can share my experience.**

**Acceptance Criteria**
- **Given** I have completed a stay at a property,  
- **When** I navigate to the property page and submit my review,  
- **Then** the review should appear publicly under that property listing.

---

## Host User Stories

### 6. Host Registration
**As a host, I want to register and create a verified account so that I can list my properties.**

**Acceptance Criteria**
- **Given** I am on the registration page,  
- **When** I fill in all host details and submit the form,  
- **Then** my account should be created and await admin verification.

---

### 7. Property Management
**As a host, I want to add, edit, and delete my property listings so that I can manage what guests see on the platform.**

**Acceptance Criteria**
- **Given** I am logged in as a host,  
- **When** I create or update a property listing,  
- **Then** the changes should reflect immediately in the system.  
- **And** I should be able to delete listings that I no longer want to show.

---

### 8. Manage Bookings
**As a host, I want to view all booking requests from guests so that I can approve or reject them.**

**Acceptance Criteria**
- **Given** I am logged in as a host,  
- **When** I open the booking dashboard,  
- **Then** I should see all pending, confirmed, and canceled bookings for my properties.

---

### 9. View Payment History
**As a host, I want to view my payment history so that I can track my earnings.**

**Acceptance Criteria**
- **Given** I am logged in as a host,  
- **When** I open my payment dashboard,  
- **Then** I should see all transactions and payout summaries.

---

## Admin User Stories

### 10. Verify Host Accounts
**As an admin, I want to verify host accounts so that only trusted users can list properties.**

**Acceptance Criteria**
- **Given** I am logged in as an admin,  
- **When** I view the list of pending hosts,  
- **Then** I should be able to approve or reject their verification requests.

---

### 11. Manage Users
**As an admin, I want to manage user accounts so that I can suspend or remove any that violate policies.**

**Acceptance Criteria**
- **Given** I am logged in as an admin,  
- **When** I open the user management panel,  
- **Then** I should be able to view, deactivate, or delete user accounts.

---

### 12. Manage Property Listings
**As an admin, I want to manage all property listings so that inappropriate or duplicate entries are removed.**

**Acceptance Criteria**
- **Given** I am logged in as an admin,  
- **When** I view all property listings,  
- **Then** I should be able to edit or remove any listing that violates platform standards.

---

### 13. Generate Reports
**As an admin, I want to generate system reports so that I can monitor platform activity and performance.**

**Acceptance Criteria**
- **Given** I am logged in as an admin,  
- **When** I select a time period or report type,  
- **Then** the system should generate a downloadable summary of bookings, users, and revenue.

---

## External System User Stories

### 14. Process Payments
**As a payment system, I want to securely process user payments so that all transactions are verified and recorded.**

**Acceptance Criteria**
- **Given** a guest has initiated a booking,  
- **When** the payment gateway receives the transaction,  
- **Then** it should confirm payment status and send a callback to the Airbnb backend.

---

### 15. Send Notifications
**As a notification service, I want to send confirmation emails for registration, bookings, and payments so that users are informed of their activities.**

**Acceptance Criteria**
- **Given** a user action triggers an event (e.g., registration or booking),  
- **When** the system processes that event,  
- **Then** an email or in-app notification should be automatically sent to the user.
