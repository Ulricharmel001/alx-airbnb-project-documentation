# ALX Airbnb Clone Backend Documentation

## Overview

This project is a **backend system** for an Airbnb-like platform, developed using **Django** and **Django REST Framework (DRF)**.  
The system handles **user authentication**, **property management**, **booking**, and **payment processing**.  
It provides RESTful APIs for interaction between users (Guests, Hosts, and Admins) and the system.

---

## 1. User Authentication

### Functional Requirements
- Allow users (Guests and Hosts) to **register**, **log in**, and **log out**.
- Use JWT-based authentication (`djangorestframework-simplejwt`).
- Secure password storage using Django’s built-in PBKDF2 hasher.
- Ensure unique emails for registration and prevent duplicate accounts.
- Admin can deactivate or verify user accounts.

### API Endpoints

| Method | Endpoint | Description |
|---------|-----------|-------------|
| POST | `/api/auth/register/` | Register a new user account |
| POST | `/api/auth/login/` | Authenticate user and return JWT tokens |
| POST | `/api/auth/logout/` | Blacklist refresh token and log out |

### Request & Response Examples

**Register (POST `/api/auth/register/`)**
```json
{
  "username": "guest_user",
  "email": "guest@example.com",
  "password": "StrongPass123"
}



### Response

{
  "message": "User registered successfully",
  "user": {
    "id": 1,
    "username": "guest_user",
    "email": "guest@example.com"
  },
  "tokens": {
    "access": "eyJ0eXAiOiJKV1QiLCJhbGci...",
    "refresh": "eyJ0eXAiOiJKV1QiLCJhbGci..."
  }
}
