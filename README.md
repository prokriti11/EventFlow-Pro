# 🎟️ EventFlow Pro

**Smart Event Discovery, Community Engagement & Ticketing Platform**

EventFlow Pro is a full-stack, scalable event discovery and ticket booking platform that enables users to explore events, receive personalized recommendations, book tickets securely, and engage with a live community. The platform is designed with a **modern UI**, a **robust backend**, and an **AI-ready recommendation system**.

---

## 📌 Problem Statement

Users often struggle to:

* Discover relevant events across categories
* Trust event quality and popularity
* Receive personalized recommendations
* Track what friends or communities are attending
* Book tickets smoothly and securely

**EventFlow Pro solves this by combining discovery, personalization, and community-driven engagement in one platform.**

---

## 🎯 Project Objectives

* Centralize event discovery across multiple domains
* Provide personalized, interest-based recommendations
* Enable real-time ticket booking and activity tracking
* Build a social layer around events
* Design an AI-ready backend for future scalability

---

## 🧠 AI & Personalization Vision

EventFlow Pro is designed with an **AI-first mindset**, even if deployed initially with rule-based logic.

### Current Personalization Logic

* User interests
* Event popularity
* Friends’ activity
* Category preferences
* Location relevance

### Recommendation Output

* Match percentage (e.g., 95% Match)
* Contextual explanation (e.g., “Based on your interest in music”)

### AI-Ready Future

* ML-based collaborative filtering
* Behavioral learning models
* Real-time personalization
* Demand prediction for events

---

## 🚀 Core Features

### 🔍 Event Discovery

* Browse events by category:

  * Music
  * Sports
  * Theater
  * Conferences
  * Food & Drink
  * Art & Culture
  * Family
* Featured & trending events
* Search-based discovery

---

### 🎫 Ticket Booking

* Transparent pricing
* Real-time availability
* Instant booking confirmation
* Digital ticket generation

---

### 🎯 Personalized Recommendations

* Match-score-based suggestions
* User interest tracking
* Region-based popularity
* Wellness & lifestyle curation

---

### 👥 Community & Social Features

* Live activity feed (bookings & views)
* “Popular with friends” indicator
* Friends’ saved & attended events
* Community testimonials

---

### 🔴 Live Activity Tracking

* Real-time viewer count
* Booking notifications
* Event interest heat signals

---

### 📩 User Retention

* Newsletter subscription
* Early-bird discounts
* Personalized alerts
* Exclusive pre-sales

---

## 🧱 System Architecture

```
Frontend (UI)
   |
REST API
   |
Backend (Node + Express)
   |
PostgreSQL Database
   |
AI / Recommendation Logic
```

---

## 🛠️ Tech Stack

### Frontend

* HTML5
* CSS3 (Modern responsive design)
* JavaScript (Dynamic rendering)

### Backend

* Node.js
* Express.js
* Prisma ORM
* JWT Authentication

### Database

* PostgreSQL

### Real-Time

* WebSockets (Live activity)

### AI Layer

* Rule-based engine (ML-upgradable)

### Deployment Ready

* Render / AWS / Supabase compatible

---

## 🗂️ Project Structure

```
EventFlow-Pro/
│
├── frontend/
│   ├── index.html
│   ├── styles/
│   └── scripts/
│
├── backend/
│   ├── src/
│   │   ├── controllers/
│   │   ├── routes/
│   │   ├── models/
│   │   ├── middleware/
│   │   ├── utils/
│   │   ├── app.js
│   │   └── server.js
│   │
│   ├── prisma/
│   │   └── schema.prisma
│   └── package.json
│
└── README.md
```

---

## 🧾 Database Design

### 👤 Users

* id
* name
* email
* password (hashed)
* interests
* created_at

### 🎟️ Events

* id
* title
* category
* description
* location
* date
* price
* available tickets
* popularity score

### 🧾 Bookings

* id
* user_id
* event_id
* quantity
* total_price
* booking_time

### 🔴 Activity

* id
* user_id
* event_id
* action (view/book)
* timestamp

---

## 🔐 Authentication & Security

* JWT-based authentication
* Password hashing with bcrypt
* Protected routes
* Role-based access (future)
* Input validation & sanitization

---

## 🔗 API Endpoints

### Authentication

```
POST /api/auth/register
POST /api/auth/login
```

### Events

```
GET  /api/events
GET  /api/events/:id
GET  /api/events/category/:type
POST /api/events (Admin)
```

### Tickets

```
POST /api/tickets/book
```

### Recommendations

```
GET /api/recommendations
```

### Live Activity

```
POST /api/activity/view
POST /api/activity/book
GET  /api/activity/live
```

---

## 🎫 Ticket Booking Flow

1. User selects event
2. Availability is validated
3. Tickets are reserved
4. Booking is created
5. Activity is logged
6. Confirmation is returned

---

## ⚙️ Installation & Setup

### Backend Setup

```bash
git clone https://github.com/your-username/eventflow-pro.git
cd backend
npm install
npx prisma migrate dev
npm start
```

### Frontend Setup

```bash
Open frontend/index.html in browser
```

---

## 📈 Scalability & Future Enhancements

* Payment gateway integration (Stripe)
* ML-based recommendation engine
* Organizer dashboards
* Admin analytics panel
* Push notifications
* Mobile app support

---

## 🧪 Use Cases

* Music & art enthusiasts
* Professionals attending conferences
* Community-based event discovery
* Social group planning
* Event organizers promoting events

---

## 🏆 Video
Link : https://drive.google.com/file/d/1ldTGPJ8dQiw-obJdYNCPk3XK2H4pG0CG/view?usp=sharing

---

## Screenshots
<img width="1919" height="975" alt="image" src="https://github.com/user-attachments/assets/53188f99-b144-4af9-a5f2-b11e81b59359" />
<img width="1919" height="963" alt="image" src="https://github.com/user-attachments/assets/2b308a5c-9ba3-45b1-a6e1-e2636174db76" />
<img width="1919" height="976" alt="image" src="https://github.com/user-attachments/assets/eb216db8-b98e-4bd0-a3d0-21b35ea00e32" />
<img width="1919" height="965" alt="image" src="https://github.com/user-attachments/assets/63971557-4557-4789-9c31-c088cca778a3" />
<img width="1918" height="964" alt="image" src="https://github.com/user-attachments/assets/37573245-2a98-402d-9e53-5ec58c0fceca" />

---

## 📄 License

© 2025 EventFlow Pro
All rights reserved.

---
Just tell me what to do next.
