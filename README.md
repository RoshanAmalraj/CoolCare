# Cool Care 🔧❄️
### Trusted Home Appliance Repair Service Platform for India

<div align="center">

![Cool Care Banner](https://img.shields.io/badge/Cool%20Are-Home%20Repair%20Platform-00d4ff?style=for-the-badge&logo=tools&logoColor=white)
![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Django](https://img.shields.io/badge/Django-4.x-092E20?style=for-the-badge&logo=django&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Netlify](https://img.shields.io/badge/Netlify-Live-00C7B7?style=for-the-badge&logo=netlify&logoColor=white)

**[🌐 Live Demo](https://coolcare-app.netlify.app)** • **[📱 Mobile Friendly](#responsive-design)** • **[🔐 OTP Secured](#security)**

</div>

---

## 📋 Table of Contents

- [About the Project](#about-the-project)
- [Problem Statement](#problem-statement)
- [Live Demo](#live-demo)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Installation](#installation)
- [API Endpoints](#api-endpoints)
- [Database Schema](#database-schema)
- [Screenshots](#screenshots)
- [Cross-Device Sync](#cross-device-sync)
- [Security](#security)
- [Responsive Design](#responsive-design)
- [How It Works](#how-it-works)
- [Admin Panel](#admin-panel)
- [Future Improvements](#future-improvements)
- [Developer](#developer)
- [License](#license)

---

## 🏠 About the Project

**Cool Care** is a full-stack home appliance repair service platform built exclusively for Indian users. It connects **customers** who need appliance repairs with **certified local technicians** — making the entire booking, verification, tracking, and completion process digital, fast, and secure.

Inspired by platforms like **Urban Company**, Cool Are brings a premium service booking experience to cities and towns across India.

> *"Every feature was designed with the real Indian user in mind — from OTP security to digital receipts in their hands after every repair."*

---

## 🎯 Problem Statement

Millions of Indian households face a daily frustration:

- ❌ Finding a **trusted technician** is hard
- ❌ No way to **verify** if a technician is genuine
- ❌ No **transparency** in service pricing or timing
- ❌ No **record** of work done or money paid
- ❌ Booking is done over **phone calls** with no tracking

**Cool Care solves all of this** with a structured digital platform where every step — from booking to payment receipt — is handled transparently and securely.

---

## 🌐 Live Demo

| Link | Description |
|------|-------------|
| 🔗 [https://coolcare-app.netlify.app](https://coolcare-app.netlify.app) | Live production site |

### Demo Credentials

**Technician Login:**
| Field | Value |
|-------|-------|
| Email | `rajesh@cool.in` |
| Worker ID | `COOL-1042` |
| Password | `Rajesh@123` |

**Customer Login:**
| Field | Value |
|-------|-------|
| Email | `priya@cool.in` |
| Password | `Priya@123` |

**Demo OTP:** `123456`

---

## ✨ Features

### 👤 Customer Module

| Feature | Description |
|---------|-------------|
| 📝 Registration | Full name, email, phone, location with password strength validation |
| 🔐 Login | Email + password with wrong credential detection |
| 🔑 Forgot Password | Email-based password reset (simulated) |
| 🏠 Dashboard | Personalised greeting with name, initials, and profile stats |
| ❄️ Appliance Selection | AC, Air Cooler, Washing Machine, Refrigerator |
| 📍 Technician Listing | Nearby technicians filtered by appliance type and location |
| ⭐ Ratings | View technician star ratings and review count |
| ❤️ Favourites | Save and rebook favourite technicians |
| 📝 Complaint Booking | Product type, description, address, live GPS location |
| 📲 OTP System | 6-digit OTP generated and shown to customer for verification |
| 🧾 Digital Receipt | Full receipt with technician name, time in/out, duration |
| ⭐ Feedback | 5-star rating + written review for every technician |
| ⚠️ Complaints | File complaints against technicians — stored in Admin Panel |
| 🔍 Search & Filter | Search technicians by name or location |

### 🔧 Technician Module

| Feature | Description |
|---------|-------------|
| 📝 Registration | Full name, phone, email, Govt ID, work types, location, photo |
| 🪪 Auto Worker ID | Unique COOL-XXXX ID generated on registration, sent via SMS |
| 📸 Photo Upload | Profile photo up to 10MB (JPG, PNG, WebP) |
| 🔐 Login | Email + Worker ID + Password triple verification |
| 📊 Dashboard | Job stats — Total, Pending, Completed, Rating |
| 📋 Job Cards | Customer complaints shown as modern booking cards |
| 🗺️ Location Map | OpenStreetMap integration to view customer location |
| ✅ Accept / Reject | Accept complaint → triggers OTP to customer |
| 🔐 OTP Verification | Verify customer OTP before starting any work |
| ⏱️ Work Timer | Live timer with Start, Pause, Resume controls |
| 🧾 Receipt Generation | Auto-generated receipt with real technician name on finish |
| 🔄 Status Update | Availability auto-switches IN → OUT → IN |
| 📈 Completed Counter | Updates in real-time after each finished job |

### 🔗 Cross-Device Sync

| Feature | Description |
|---------|-------------|
| ☁️ Cloud Database | JSONBin.io free REST API as shared database |
| 📡 Real-time Sync | Technician registered on Phone A visible on Phone B |
| 🔄 Auto Refresh | Data refreshes every 30 seconds across all devices |
| 💾 Offline Cache | Local cache fallback when cloud is unavailable |
| 🔑 Setup Panel | Easy one-time API key configuration |

### 🛡️ Admin Panel (Django)

| Feature | Description |
|---------|-------------|
| 👷 Technician Management | View, approve, delete technicians |
| 👥 Customer Management | View and manage all customer accounts |
| 📋 Booking Management | View all complaints and bookings |
| ⭐ Feedback Logs | View all ratings and reviews |
| 🧾 Receipt History | Access all digital receipts |
| 📲 OTP Logs | Track all OTP verifications |
| 🚫 Block Users | Block fake or abusive users |

---

## 🛠️ Tech Stack

### Frontend
```
HTML5          →  Semantic structure
CSS3           →  Custom animations, Glassmorphism, Gradients
JavaScript     →  ES6+, Async/Await, Fetch API, LocalStorage
Leaflet.js     →  OpenStreetMap integration (free, no API key)
Font Awesome   →  Icons
Google Fonts   →  Syne, DM Sans, Space Mono
```

### Backend
```
Python 3.10+              →  Core language
Django 4.x                →  Web framework
Django REST Framework      →  API layer
JWT Authentication         →  Secure token-based auth
SQL Database              →  SQLite (dev) / PostgreSQL (production)
```

### Third-Party Services
```
JSONBin.io    →  Cross-device cloud database sync
Google Maps   →  Live location tracking (integrated)
Twilio        →  SMS OTP (simulated in frontend demo)
Netlify       →  Frontend hosting
```

### Design
```
Mobile-first responsive design
Dark theme with cyan/orange gradient palette
Glassmorphism cards
3D hover effects
CSS animations and transitions
Custom scrollbars and toast notifications
```

---

## 📁 Project Structure

```
cool-Care/
│
├── 📁 backend/                    # Django backend
│   ├── 📁 coolcare/               # Main Django project
│   │   ├── settings.py
│   │   ├── urls.py
│   │   ├── wsgi.py
│   │   └── asgi.py
│   │
│   ├── 📁 accounts/              # User authentication app
│   │   ├── models.py             # User models
│   │   ├── views.py              # Auth views
│   │   ├── serializers.py        # DRF serializers
│   │   └── urls.py
│   │
│   ├── 📁 technicians/           # Technician module
│   │   ├── models.py             # Technician model
│   │   ├── views.py              # Technician views
│   │   ├── serializers.py
│   │   └── urls.py
│   │
│   ├── 📁 customers/             # Customer module
│   │   ├── models.py             # Customer model
│   │   ├── views.py
│   │   ├── serializers.py
│   │   └── urls.py
│   │
│   ├── 📁 complaints/            # Booking & complaint system
│   │   ├── models.py             # Complaint model
│   │   ├── views.py
│   │   ├── serializers.py
│   │   └── urls.py
│   │
│   ├── 📁 receipts/              # Digital receipt system
│   │   ├── models.py
│   │   ├── views.py
│   │   └── serializers.py
│   │
│   ├── 📁 otp/                   # OTP verification system
│   │   ├── models.py
│   │   └── views.py
│   │
│   ├── manage.py
│   └── requirements.txt
│
├── 📁 frontend/                   # Frontend (HTML/CSS/JS)
│   ├── index.html                # Main single-page app
│   ├── 📁 static/
│   │   ├── 📁 css/
│   │   │   └── styles.css
│   │   ├── 📁 js/
│   │   │   ├── auth.js
│   │   │   ├── dashboard.js
│   │   │   ├── technician.js
│   │   │   ├── customer.js
│   │   │   └── sync.js
│   │   └── 📁 images/
│   │
│   └── 📁 templates/
│
├── 📁 docs/                       # Documentation
│   ├── api-docs.md
│   └── screenshots/
│
├── .env.example                   # Environment variables template
├── .gitignore
├── README.md
└── LICENSE
```

---

## 🚀 Getting Started

### Prerequisites

Make sure you have these installed:

```bash
Python 3.10+
pip
Git
virtualenv (recommended)
```

### Installation

**1. Clone the repository**
```bash
git clone https://github.com/yourusername/cool-are.git
cd cool-are
```

**2. Create and activate virtual environment**
```bash
# Windows
python -m venv venv
venv\Scripts\activate

# macOS / Linux
python3 -m venv venv
source venv/bin/activate
```

**3. Install Python dependencies**
```bash
pip install -r requirements.txt
```

**4. Set up environment variables**
```bash
cp .env.example .env
```

Edit `.env` with your values:
```env
SECRET_KEY=your-django-secret-key-here
DEBUG=True
DATABASE_URL=sqlite:///db.sqlite3
ALLOWED_HOSTS=localhost,127.0.0.1

# JWT
JWT_SECRET=your-jwt-secret

# Twilio SMS (for real OTP)
TWILIO_ACCOUNT_SID=your-twilio-sid
TWILIO_AUTH_TOKEN=your-twilio-token
TWILIO_PHONE_NUMBER=+1234567890

# Google Maps
GOOGLE_MAPS_API_KEY=your-google-maps-key

# JSONBin (cross-device sync)
JSONBIN_MASTER_KEY=your-jsonbin-master-key
```

**5. Run database migrations**
```bash
cd backend
python manage.py makemigrations
python manage.py migrate
```

**6. Create Django superuser (Admin)**
```bash
python manage.py createsuperuser
```

**7. Seed demo data (optional)**
```bash
python manage.py loaddata demo_data.json
```

**8. Start the development server**
```bash
python manage.py runserver
```

**9. Open in browser**
```
http://127.0.0.1:8000
```

**10. Access Admin Panel**
```
http://127.0.0.1:8000/admin
```

---

## 📡 API Endpoints

### Authentication
```
POST   /api/auth/register/technician/    →  Technician registration
POST   /api/auth/register/customer/      →  Customer registration
POST   /api/auth/login/technician/       →  Technician login
POST   /api/auth/login/customer/         →  Customer login
POST   /api/auth/logout/                 →  Logout
POST   /api/auth/forgot-password/        →  Password reset
POST   /api/auth/verify-otp/            →  OTP verification
```

### Technicians
```
GET    /api/technicians/                 →  List all technicians
GET    /api/technicians/?type=AC        →  Filter by appliance type
GET    /api/technicians/{id}/           →  Single technician detail
PUT    /api/technicians/{id}/status/    →  Update availability (IN/OUT)
GET    /api/technicians/{id}/reviews/   →  Get technician reviews
```

### Complaints / Bookings
```
GET    /api/complaints/                  →  List complaints (technician)
POST   /api/complaints/                  →  Create new complaint (customer)
GET    /api/complaints/{id}/             →  Complaint detail
PUT    /api/complaints/{id}/accept/      →  Accept complaint
PUT    /api/complaints/{id}/reject/      →  Reject complaint
PUT    /api/complaints/{id}/complete/    →  Mark as completed
```

### Receipts
```
GET    /api/receipts/                    →  List receipts
GET    /api/receipts/{id}/              →  Single receipt
POST   /api/receipts/                   →  Generate receipt
```

### Feedback
```
POST   /api/feedback/                   →  Submit rating + review
GET    /api/feedback/technician/{id}/   →  Get technician feedback
```

### OTP
```
POST   /api/otp/send/                   →  Send OTP to customer
POST   /api/otp/verify/                 →  Verify OTP
```

---

## 🗄️ Database Schema

```
┌─────────────────┐     ┌─────────────────┐
│   Technician    │     │    Customer     │
├─────────────────┤     ├─────────────────┤
│ id (PK)         │     │ id (PK)         │
│ name            │     │ name            │
│ email (unique)  │     │ email (unique)  │
│ worker_id       │     │ phone           │
│ phone           │     │ password_hash   │
│ govt_id         │     │ location        │
│ work_types      │     │ created_at      │
│ location        │     └────────┬────────┘
│ profile_photo   │              │
│ password_hash   │              │
│ rating_avg      │     ┌────────▼────────┐
│ availability    │     │   Complaint     │
│ created_at      │     ├─────────────────┤
└────────┬────────┘     │ id (PK)         │
         │              │ customer (FK)   │
         │              │ technician (FK) │
         └──────────────┤ product_type    │
                        │ description     │
                        │ address         │
                        │ latitude        │
                        │ longitude       │
                        │ status          │
                        │ otp_code        │
                        │ created_at      │
                        └────────┬────────┘
                                 │
                    ┌────────────▼────────────┐
                    │        Receipt          │
                    ├─────────────────────────┤
                    │ id (PK)                 │
                    │ complaint (FK)          │
                    │ technician_name         │
                    │ customer_name           │
                    │ service_type            │
                    │ time_in                 │
                    │ time_out                │
                    │ duration                │
                    │ created_at              │
                    └─────────────────────────┘
                                 │
                    ┌────────────▼────────────┐
                    │        Feedback         │
                    ├─────────────────────────┤
                    │ id (PK)                 │
                    │ receipt (FK)            │
                    │ rating (1–5)            │
                    │ review_text             │
                    │ created_at              │
                    └─────────────────────────┘
```

---



---

## 🔗 Cross-Device Sync

The biggest challenge in a HTML-only deployment is **sharing data across phones**.

### How it works:

```
Phone A (Technician)          JSONBin Cloud           Phone B (Customer)
      │                            │                         │
      │── Register ──────────────► │ ◄─────────── Pull ─────│
      │                            │                         │
      │                     [ Shared Database ]              │
      │                            │                         │
      │                            │── Sync every 30s ──────►│
      │                            │                         │
      │                            │    Tech now visible     │
      │                            │    on Phone B ✅        │
```

### Setup Steps:
1. Get a **free API key** from [jsonbin.io](https://jsonbin.io)
2. Open Cool Are → tap **🔗 Sync** button
3. Enter your API key → tap **Connect & Sync**
4. Share the generated **Bin ID** with all devices
5. All phones now share one live database ✅

---

## 🔐 Security

| Security Feature | Implementation |
|-----------------|----------------|
| Password Hashing | Django's built-in PBKDF2 hashing |
| JWT Tokens | Stateless authentication for API calls |
| OTP Verification | 6-digit random OTP before service starts |
| Email Uniqueness | Checked at registration across both user types |
| Password Strength | Min 6 chars, uppercase, lowercase, number, special char |
| Govt ID Capture | Required for every technician registration |
| Session Persistence | Secure session restore on page reload |
| Input Validation | Client-side + server-side validation on all forms |

---

## 📱 Responsive Design

Cool Are works perfectly on all screen sizes:

```
📱 Android Phones     →  320px – 480px
📱 iPhones            →  375px – 430px
📟 Tablets            →  768px – 1024px
💻 Laptops            →  1024px – 1440px
🖥️ Desktop            →  1440px+
```

Tested on:
- ✅ Android (Chrome, Samsung Browser)
- ✅ iPhone (Safari, Chrome)
- ✅ iPad
- ✅ Windows Laptop (Chrome, Edge, Firefox)
- ✅ MacBook (Safari, Chrome)

---

## ⚙️ How It Works

```
CUSTOMER FLOW:
──────────────
Register → Login → Select Appliance → View Technicians
→ Tap "Book Now" → Fill Complaint Form → Submit
→ Receive OTP → Share OTP with Technician
→ Technician Works → Receive Digital Receipt
→ Rate & Review

TECHNICIAN FLOW:
─────────────────
Register (get Worker ID via SMS) → Login
→ View Complaint Dashboard → Accept Job
→ OTP Verified → Start Work Timer
→ Complete Work → Receipt Auto-Generated
→ Status: OUT → IN (available again)

ADMIN FLOW:
────────────
Login to Django Admin → Manage Technicians
→ View Complaints → Check Receipts
→ Read Feedback → Block Users
```

---

## 🔮 Future Improvements

- [ ] Real SMS OTP via Twilio integration
- [ ] Google Pay / UPI payment integration
- [ ] Real-time chat between customer and technician
- [ ] Push notifications (Firebase FCM)
- [ ] Technician earnings dashboard
- [ ] Service price estimation
- [ ] Multi-language support (Tamil, Hindi, English)
- [ ] Android and iOS native apps (React Native)
- [ ] Machine learning for technician recommendation
- [ ] Video call support for remote diagnosis
- [ ] Subscription plans for regular maintenance

---

## 👨‍💻 Developer

<div align="center">

**B. Roshan Amalraj**

*Python Django Developer*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/yourprofile)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?style=for-the-badge&logo=github)](https://github.com/yourusername)
[![Portfolio](https://img.shields.io/badge/Portfolio-Visit-00d4ff?style=for-the-badge&logo=globe)](https://yourportfolio.com)
[![Email](https://img.shields.io/badge/Email-Contact-EA4335?style=for-the-badge&logo=gmail)](mailto:your@email.com)

*Open to work — Full Stack / Backend / Django Developer positions*

</div>

---

## 📄 License

```
MIT License

Copyright (c) 2024 B. Roshan Amalraj

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
```

---

<div align="center">

Made with ❤️ in India 🇮🇳

**Cool Care — Trusted Home Appliance Repair Services Across India**

⭐ Star this repo if you found it helpful!
</div>

---

## Screenshot 
Home:
<img width="1600" height="720" alt="Screenshot_2026-06-01-19-05-24-70_4aed3257f278fcf7bfa3abd644e23333" src="https://github.com/user-attachments/assets/77f6ff2c-732a-411b-8ad9-8e69f51fc2b1" />

Technician Registration:
<img width="1600" height="720" alt="Screenshot_2026-06-01-19-08-47-12_4aed3257f278fcf7bfa3abd644e23333" src="https://github.com/user-attachments/assets/091b5702-ff2a-4183-99b5-3fbcdc686fca" />

Technician Login:
<img width="1600" height="720" alt="Screenshot_2026-06-01-19-05-59-86_4aed3257f278fcf7bfa3abd644e23333" src="https://github.com/user-attachments/assets/6a110098-a5ad-4ec3-847b-2ba4a7e3463e" />

Technician Page:
<img width="1600" height="720" alt="Screenshot_2026-06-01-19-06-04-41_4aed3257f278fcf7bfa3abd644e23333" src="https://github.com/user-attachments/assets/219fa5ff-fc25-4ae6-b653-c8d10c43ceec" />

Technician work Confirmation:
<img width="1600" height="720" alt="Screenshot_2026-06-01-19-12-33-81_4aed3257f278fcf7bfa3abd644e23333" src="https://github.com/user-attachments/assets/6652c1d2-27e8-4391-83bd-8fe7af4edd29" />

OTP Verification:
<img width="1600" height="720" alt="Screenshot_2026-06-01-19-06-25-56_4aed3257f278fcf7bfa3abd644e23333" src="https://github.com/user-attachments/assets/185d922e-51a8-49d5-b32d-a997fc653234" />

Work Start Page:
<img width="1600" height="720" alt="Screenshot_2026-06-01-19-06-34-26_4aed3257f278fcf7bfa3abd644e23333" src="https://github.com/user-attachments/assets/9bfa12cd-7e4c-4966-a44e-9213cd6bbc8a" />

Customer Registration:
<img width="1600" height="720" alt="Screenshot_2026-06-01-19-09-01-96_4aed3257f278fcf7bfa3abd644e23333" src="https://github.com/user-attachments/assets/6ac7d720-9436-4984-96bb-fd61c1963c94" />

Customer Page:
<img width="1600" height="720" alt="Screenshot_2026-06-01-19-07-31-89_4aed3257f278fcf7bfa3abd644e23333" src="https://github.com/user-attachments/assets/90ef5206-456f-4665-a478-67a328f7d8f4" />

OTP Generate:
<img width="1600" height="720" alt="Screenshot_2026-06-01-19-08-03-87_4aed3257f278fcf7bfa3abd644e23333" src="https://github.com/user-attachments/assets/60c067d1-e6b3-4a9c-a5d8-ad8990601379" />

Online Reciept:
<img width="1600" height="720" alt="Screenshot_2026-06-01-19-08-32-40_4aed3257f278fcf7bfa3abd644e23333" src="https://github.com/user-attachments/assets/a0302999-03a7-415b-8827-ab7448d8e2d5" />

Feedback:
<img width="1600" height="720" alt="Screenshot_2026-06-01-19-08-16-23_4aed3257f278fcf7bfa3abd644e23333" src="https://github.com/user-attachments/assets/6729e80f-a73a-4cd5-8009-42400de5b52f" />

App Features:
<img width="1600" height="720" alt="Screenshot_2026-06-01-19-09-45-09_4aed3257f278fcf7bfa3abd644e23333" src="https://github.com/user-attachments/assets/99316d07-c2b8-46ad-99d6-aa6f63028d12" />

Appliance Repair:
<img width="1600" height="720" alt="Screenshot_2026-06-01-19-09-20-11_4aed3257f278fcf7bfa3abd644e23333" src="https://github.com/user-attachments/assets/8fd60b99-0384-4d04-a077-283be38f4426" />

---
