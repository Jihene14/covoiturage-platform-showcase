# 🚗 Carpooling Platform

> **A full-stack carpooling platform designed to connect drivers and passengers traveling along similar routes.**

🇹🇳 **A project inspired by transportation challenges in Tunisia and the potential of shared mobility.**

---

## 💡 The Idea

Every day, people make similar journeys to work, university, and between cities — while many cars travel with empty seats.

Carpooling offers a simple idea: **share the journey.**

By connecting drivers and passengers traveling along similar routes, carpooling can help make transportation:

* 💰 More economical
* ⏱️ More time-efficient
* 🌱 More sustainable
* 🚗 Better optimized
* 🤝 More social

This project explores what a digital carpooling platform could look like in Tunisia.

> **The project is currently a technical proof of concept. Its deployment as a real-world service would require an appropriate legal and regulatory framework.**

---

## 🎯 Project Goal

I challenged myself to design and develop a **complete full-stack carpooling platform independently**, from the database and backend APIs to the frontend interface and administrative features.

The goal was not simply to build CRUD operations, but to create a coherent platform with authentication, business rules, reservations, role-based access, notifications, ratings, and administration.

---

## ✨ Features

### 👤 User Management

* User registration and login
* Profile management
* Secure authentication
* Role-based authorization
* User validation

### 🚗 Vehicle Management

* Add vehicles
* Edit vehicle information
* Delete vehicles
* Manage personal vehicles
* Ownership-based access control

### 🗺️ Trip Management

* Create trips
* Search and browse available trips
* Manage departure and destination
* Define available seats
* Manage trip information
* Business-rule validation

### 🎫 Reservations

* Reserve available seats
* View reservations
* Manage reservation status
* Seat availability management

### ⭐ Ratings

* Rate completed journeys
* Manage ratings and reviews

### 🔔 Notifications

* User notifications
* Notification management
* Notification types
* Backend notification service

### 🛡️ Administration

* Dedicated Admin Dashboard
* Platform statistics
* Administrative management
* Role-based access control
* Protected administrative operations

---

## 🏗️ Architecture

The application follows a layered full-stack architecture:

```text
┌─────────────────────────┐
│       Angular           │
│     Frontend / UI       │
└────────────┬────────────┘
             │
             │ REST API
             ▼
┌─────────────────────────┐
│      Spring Boot        │
│       Backend           │
├─────────────────────────┤
│ Controllers             │
│ Services                │
│ Repositories            │
│ Entities / DTOs         │
│ Security                │
└────────────┬────────────┘
             │
             ▼
┌─────────────────────────┐
│        MariaDB          │
│      Relational DB      │
└─────────────────────────┘
```

### Backend

The backend is organized around:

* Controllers
* Services
* Repositories
* Entities
* DTOs
* Security
* Global exception handling
* Database migrations

### Frontend

The Angular application is organized into feature-based modules/components including:

* Authentication
* Profile
* Trips
* Vehicles
* Reservations
* Ratings
* Notifications
* Administration

---

## 🛠️ Tech Stack

| Layer              | Technology                     |
| ------------------ | ------------------------------ |
| Frontend           | Angular, TypeScript, HTML, CSS |
| Backend            | Java, Spring Boot              |
| Database           | MariaDB                        |
| ORM                | Spring Data JPA / Hibernate    |
| API                | REST                           |
| Database Migration | Flyway                         |
| UI                 | Bootstrap                      |
| Authentication     | JWT                            |
| Version Control    | Git / GitHub                   |

---

## 📸 Screenshots

### Home

![Home](docs/screenshots/home.png)

### Trip Search & Listing

![Trips](docs/screenshots/trips.png)
![TripsList](docs/screenshots/Mytrips-list.png)
### Trip Details & Reservation

![Reservations](docs/screenshots/reservations.png)

### User Profile

![Profile](docs/screenshots/profile.png)

### Rating user

![UserRating](docs/screenshots/user-rating.png)

### Notifications

![Notifications](docs/screenshots/notifications.png)

### Admin Dashboard

![AdminDashboard](docs/screenshots/admin-dashboard.png)

---

## 📂 Project Structure

```text
covoiturage-platform/
│
├── backend/
│   └── src/
│       └── main/
│           ├── java/
│           └── resources/
│
├── frontend/
│   └── src/
│       └── app/
│           ├── core/
│           ├── features/
│           ├── shared/
│           └── ...
│
├── docs/
│   ├── diagrams/
│   ├── mockups/
│   ├── 01-project-vision.md
│   ├── 02-requirements.md
│   ├── 03-user-stories.md
│   ├── 04-database-design.md
│   ├── 05-api-design.md
│   ├── 06-ui-ux.md
│   ├── 07-roadmap.md
│   └── 08-development-journal.md
│
├── .env.example
├── .gitignore
└── README.md
```

---

## ⚙️ Getting Started

### Prerequisites

Make sure you have installed:

* Java 17+
* Node.js
* Angular CLI
* MariaDB
* Maven

### 1. Clone the repository

```bash
git clone https://github.com/Jihene14/covoiturage-platform.git
cd covoiturage-platform
```

### 2. Configure environment variables

Copy the example configuration:

```bash
cp .env.example .env
```

Configure the required database and JWT values according to your local environment.

> Never commit your `.env` file or production secrets.

### 3. Start the backend

```bash
cd backend
./mvnw spring-boot:run
```

On Windows:

```powershell
.\mvnw.cmd spring-boot:run
```

### 4. Start the frontend

```bash
cd frontend
npm install
ng serve
```

The application will then be available through the Angular development server.

---

## 📚 Documentation

The `docs/` directory contains additional project documentation covering:

* [Project Vision](docs/01-project-vision.md)
* [Requirements](docs/02-requirements.md)
* [User Stories](docs/03-user-stories.md)
* [Database Design](docs/04-database-design.md)
* [API Design](docs/05-api-design.md)
* [UI/UX](docs/06-ui-ux.md)
* [Roadmap](docs/07-roadmap.md)
* [Development Journal](docs/08-development-journal.md)

---

## 🚀 Future Vision

This project is currently a technical proof of concept.

My hope is that Tunisia can eventually develop a clear framework allowing **safe, responsible and regulated carpooling platforms** to operate.

Potential future directions include:

* 📍 GPS-based route matching
* 🗺️ Interactive maps
* 📱 Mobile application
* 💬 In-app communication
* 🧠 Smarter trip matching
* 🛡️ Additional safety and verification mechanisms

---

## 👩‍💻 About the Project

This project was **independently designed and developed as a full-stack engineering challenge**.

Building it alone meant working across the entire application:

**Idea → Requirements → UI/UX → Database → Backend → API → Security → Frontend → Administration**

The project allowed me to go beyond learning individual technologies and focus on how they work together to build a complete product.

---

## 🌱 Vision

> **Technology doesn't always need to create something new. Sometimes, it can simply help us use what we already have — better.**

🚗 **One journey. Multiple people. Better use of every seat.**
