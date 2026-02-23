
---

# 🌍 GeoSentinel

### Smart Tourist Safety Monitoring System using Geofencing & Blockchain

> AI-powered geofencing and blockchain-secured tourist safety monitoring platform designed to enhance traveler protection in real time.

---

## 🚀 Overview

**GeoSentinel** is a full-stack web application built to ensure tourist safety using:

* 📍 Real-time GPS tracking
* 🗺️ Google Maps integration
* 🚧 Intelligent geofencing alerts
* 🚨 SOS emergency system
* 🔐 Blockchain-based tamper-proof logs
* 👨‍💼 Admin monitoring dashboard

This system helps detect restricted zone entry, trigger emergency alerts, and provide live monitoring for authorities.

---

## ✨ Key Features

### 🔐 Authentication System

* User login via Phone or Gmail
* OTP verification for new registrations
* Secure JWT authentication
* Role-based access (User / Admin)

---

### 🗺️ Live Smart Map

* Real-time GPS tracking
* Google Maps integration
* Nearby search:

  * Hotels
  * Gas stations
  * Temples
  * Tourist places
  * Hospitals
  * Police stations
  * Restaurants
  * ATMs

---

### 🚧 Geofencing Alerts

* Detects entry into restricted zones
* Real-time warning notifications
* Alert logging system
* Blockchain-backed violation records

---

### 🚨 SOS Emergency System

* Floating SOS button
* Sends alert to Admin dashboard
* Stores GPS coordinates
* Direct emergency call to **100**
* Real-time alert tracking

---

### 👨‍💼 Admin Dashboard

* Overview analytics:

  * Total users
  * Active users
  * SOS alerts count
* Live user tracking map
* Access to:

  * User database
  * Queries & support tickets
  * Feedback records
  * SOS logs
* Filter & search options

---

### 🎨 UI & UX

* Premium dark theme (Black + Brown palette)
* Glassmorphism design
* Smooth animations
* Responsive layout
* Live digital clock
* Weather widget
* Hidden smart interactions

---

## 🏗️ Tech Stack

### 🎨 Frontend

* React
* Tailwind CSS
* Google Maps API
* Responsive Design

### ⚙️ Backend

* FastAPI
* SQL (PostgreSQL / MySQL)
* SQLAlchemy ORM
* JWT Authentication
* Pydantic Validation

### 🔗 Blockchain (Mock Implementation)

* Hash-based logging system
* Tamper-proof alert records

---

## 🗂️ Project Structure

```
GeoSentinel/
│
├── frontend/
│   ├── components/
│   ├── pages/
│   ├── services/
│   └── styles/
│
├── backend/
│   ├── app/
│   │   ├── models/
│   │   ├── schemas/
│   │   ├── routes/
│   │   ├── services/
│   │   └── main.py
│   ├── database/
│   └── requirements.txt
│
└── README.md
```

---

## 🗄️ Database Design

### Users Table

* id
* name
* phone
* email
* password_hash
* is_verified
* created_at

### Admins Table

* id
* phone
* password_hash
* created_at

### OTP Logs

* id
* phone_or_email
* otp
* expiry
* verified

### SOS Alerts

* id
* user_id
* latitude
* longitude
* timestamp
* status

### Queries & Feedback

* id
* user_id
* message
* rating
* created_at

---

## 🔌 API Endpoints

### Auth

* `POST /auth/user/signup`
* `POST /auth/user/login`
* `POST /auth/admin/login`
* `POST /auth/verify-otp`

### User

* `GET /user/profile`
* `POST /user/query`
* `POST /user/feedback`

### SOS

* `POST /sos/trigger`
* `GET /admin/sos`

### Admin

* `GET /admin/dashboard`
* `GET /admin/users`
* `GET /admin/queries`
* `GET /admin/feedback`

### Geofence

* `POST /geofence/violation`

---

## ⚙️ Installation & Setup

### Backend Setup

```bash
cd backend
pip install -r requirements.txt
uvicorn app.main:app --reload
```

### Frontend Setup

```bash
cd frontend
npm install
npm start
```

---

## 🔐 Security Features

* JWT-based authentication
* OTP verification
* Role-based access control
* Secure password hashing
* Blockchain-style tamper-proof logs

---

## 🌟 Future Enhancements

* WebSocket live tracking
* Real blockchain integration (Ethereum/Polygon)
* AI-based risk prediction
* Mobile app version
* Multi-language support

---

## 📜 License

This project is developed for educational and hackathon purposes.

---

## 👥 Team

Developed for innovation in tourist safety monitoring.

---
