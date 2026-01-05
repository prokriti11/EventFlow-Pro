<div align="center">

# 🎟️ EventFlow Pro

### Smart Event Discovery, Community Engagement & Ticketing Platform

[![License](https://img.shields.io/badge/license-All%20Rights%20Reserved-red.svg)](LICENSE)
[![Node.js](https://img.shields.io/badge/node.js-v16+-green.svg)](https://nodejs.org/)
[![PostgreSQL](https://img.shields.io/badge/postgresql-13+-blue.svg)](https://www.postgresql.org/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

**EventFlow Pro** is a full-stack, scalable event discovery and ticket booking platform designed to help users explore events, receive personalized recommendations, book tickets securely, and engage with a live community.

[Features](#-core-features) • [Tech Stack](#-tech-stack) • [Installation](#-installation--setup) • [API Docs](#-api-endpoints) • [Architecture](#-system-architecture) • [Demo Video](#-demo-video)

</div>

---

## 🎬 Demo Video

<div align="center">

[![EventFlow Pro Demo](https://img.shields.io/badge/▶️-Watch%20Demo-red?style=for-the-badge&logo=youtube)](https://your-video-link-here.com)

**[🎥 Click here to watch the full demo video](https://drive.google.com/file/d/1ldTGPJ8dQiw-obJdYNCPk3XK2H4pG0CG/view?usp=sharing)**

</div>

> 💡 **Replace `https://your-video-link-here.com`** with your actual video link (YouTube, Vimeo, Loom, etc.)

---

## 📌 Problem Statement

Event discovery today is **fragmented** across multiple platforms, lacks personalization, and provides minimal social context. Users struggle to:

- 🔍 Find relevant events that match their interests
- 📊 Assess event popularity and credibility
- 👥 Understand what their friends or community are attending
- 🎫 Book tickets seamlessly without switching platforms

**EventFlow Pro** solves this by unifying event discovery, personalization, ticket booking, and community engagement into a single intelligent platform.

---

## 🎯 Project Objectives

✅ **Centralize** event discovery across multiple categories  
✅ **Personalize** event recommendations using AI-ready algorithms  
✅ **Streamline** secure and seamless ticket booking  
✅ **Engage** users through community and social features  
✅ **Build** a scalable, production-ready backend architecture  

---

## 🚀 Core Features

### 🔍 Event Discovery
Browse events across diverse categories:
- 🎵 Music
- ⚽ Sports
- 🎭 Theater
- 💼 Conferences
- 🍽️ Food & Drink
- 🎨 Art & Culture
- 👨‍👩‍👧 Family

**Additional Discovery Tools:**
- Featured and trending events
- Advanced search and filters
- Location-based exploration

### 🎫 Ticket Booking
- 💳 Transparent pricing with no hidden fees
- ⏱️ Real-time availability tracking
- ✅ Instant booking confirmation
- 📱 Digital ticket access

### 🎯 Personalized Recommendations
Powered by an intelligent matching algorithm:
- **Match Score** (e.g., 95% Match)
- **Interest-driven curation**
- **Regional popularity signals**
- **Friend activity insights**

**Recommendation Factors:**
```
• User interests
• Event popularity score
• Friends' activity
• Category preferences
• Location relevance
```

### 👥 Community & Social Features
- 📊 Live activity feed (views and bookings)
- 🔥 "Popular with friends" indicators
- 💬 Community testimonials and reviews
- 📅 Friends' saved and attended events

### 🔴 Live Activity Tracking
- 👁️ Real-time viewer count
- 🔔 Booking notifications
- 📈 Event popularity signals

### 📩 User Retention & Engagement
- 📧 Newsletter subscriptions
- 🎁 Early-bird discounts
- 🎟️ Exclusive pre-sales
- 🔔 Personalized event alerts

---

## 🧠 AI & Personalization Vision

EventFlow Pro is designed with an **AI-first mindset**.

### Current Implementation
**Rule-based recommendation engine** using:
- User interest matching
- Popularity scoring
- Social proof signals
- Geographic relevance

**Output:**
```json
{
  "matchPercentage": 95,
  "reason": "Based on your interest in music and local events",
  "socialProof": "12 friends are interested"
}
```

### 🔮 Future AI Enhancements
- 🤖 **Collaborative filtering** for user-based recommendations
- 🧠 **Deep learning models** for behavioral prediction
- 📊 **Event demand forecasting** for dynamic pricing
- ⚡ **Real-time personalization** using streaming data
- 🎯 **Content-based filtering** with NLP on event descriptions

---

## 🧱 System Architecture

```
┌─────────────────────────────────────────────┐
│          Frontend (HTML/CSS/JS)             │
│  • Event Discovery UI                       │
│  • Booking Interface                        │
│  • User Dashboard                           │
└──────────────────┬──────────────────────────┘
                   │ REST API
┌──────────────────▼──────────────────────────┐
│       Backend (Node.js + Express)           │
│  • Authentication & Authorization           │
│  • Business Logic                           │
│  • API Routes                               │
└──────────────────┬──────────────────────────┘
                   │ Prisma ORM
┌──────────────────▼──────────────────────────┐
│         PostgreSQL Database                 │
│  • Users, Events, Bookings                  │
│  • Activity Logs                            │
└──────────────────┬──────────────────────────┘
                   │
┌──────────────────▼──────────────────────────┐
│      AI / Recommendation Engine             │
│  • Personalization Logic                    │
│  • Match Score Calculation                  │
└─────────────────────────────────────────────┘
```

---

## 🛠️ Tech Stack

### Frontend
- **HTML5** - Semantic markup
- **CSS3** - Modern, responsive design
- **JavaScript** - Dynamic interactions

### Backend
- **Node.js** - Runtime environment
- **Express.js** - Web framework
- **Prisma ORM** - Database toolkit
- **JWT** - Secure authentication
- **bcrypt** - Password hashing

### Database
- **PostgreSQL** - Relational database

### Real-Time
- **WebSockets** - Live activity tracking

### AI Layer
- **Rule-based engine** - Current recommendation system
- **ML-ready architecture** - Future integration support

### Deployment Options
- **Render** - Backend hosting
- **AWS** - Cloud infrastructure
- **Supabase** - Database hosting

---

## 🗂️ Project Structure

```
EventFlow-Pro/
│
├── frontend/
│   ├── index.html
│   ├── styles/
│   │   ├── main.css
│   │   └── components.css
│   └── scripts/
│       ├── app.js
│       ├── events.js
│       └── booking.js
│
├── backend/
│   ├── src/
│   │   ├── controllers/
│   │   │   ├── authController.js
│   │   │   ├── eventController.js
│   │   │   └── bookingController.js
│   │   ├── routes/
│   │   │   ├── auth.js
│   │   │   ├── events.js
│   │   │   └── bookings.js
│   │   ├── models/
│   │   ├── middleware/
│   │   │   ├── auth.js
│   │   │   └── validation.js
│   │   ├── utils/
│   │   │   ├── jwt.js
│   │   │   └── recommendations.js
│   │   ├── app.js
│   │   └── server.js
│   │
│   ├── prisma/
│   │   └── schema.prisma
│   │
│   ├── package.json
│   └── .env.example
│
└── README.md
```

---

## 🗄️ Database Schema

### 👤 Users
```prisma
model User {
  id         Int       @id @default(autoincrement())
  name       String
  email      String    @unique
  password   String
  interests  String[]
  createdAt  DateTime  @default(now())
  bookings   Booking[]
  activities Activity[]
}
```

### 🎟️ Events
```prisma
model Event {
  id               Int       @id @default(autoincrement())
  title            String
  category         String
  description      String
  location         String
  date             DateTime
  price            Float
  availableTickets Int
  popularityScore  Float     @default(0)
  bookings         Booking[]
  activities       Activity[]
}
```

### 🧾 Bookings
```prisma
model Booking {
  id          Int      @id @default(autoincrement())
  userId      Int
  eventId     Int
  quantity    Int
  totalPrice  Float
  bookingTime DateTime @default(now())
  user        User     @relation(fields: [userId], references: [id])
  event       Event    @relation(fields: [eventId], references: [id])
}
```

### 🔴 Activity
```prisma
model Activity {
  id        Int      @id @default(autoincrement())
  userId    Int
  eventId   Int
  action    String   // "view" or "book"
  timestamp DateTime @default(now())
  user      User     @relation(fields: [userId], references: [id])
  event     Event    @relation(fields: [eventId], references: [id])
}
```

---

## 🔗 API Endpoints

### Authentication
| Method | Endpoint | Description |
|--------|----------|-------------|
| `POST` | `/api/auth/register` | Register new user |
| `POST` | `/api/auth/login` | User login |

### Events
| Method | Endpoint | Description |
|--------|----------|-------------|
| `GET` | `/api/events` | Get all events |
| `GET` | `/api/events/:id` | Get event by ID |
| `GET` | `/api/events/category/:type` | Get events by category |
| `POST` | `/api/events` | Create event (Admin) |

### Ticket Booking
| Method | Endpoint | Description |
|--------|----------|-------------|
| `POST` | `/api/tickets/book` | Book tickets |

### Recommendations
| Method | Endpoint | Description |
|--------|----------|-------------|
| `GET` | `/api/recommendations` | Get personalized recommendations |

### Live Activity
| Method | Endpoint | Description |
|--------|----------|-------------|
| `POST` | `/api/activity/view` | Log event view |
| `POST` | `/api/activity/book` | Log booking activity |
| `GET` | `/api/activity/live` | Get live activity feed |

---

## 🎫 Ticket Booking Flow

```
1. User selects an event
           ↓
2. Validate ticket availability
           ↓
3. Reserve tickets temporarily
           ↓
4. Create booking record
           ↓
5. Log activity
           ↓
6. Return confirmation
           ↓
7. Send digital ticket
```

---

## 🔐 Authentication & Security

✅ **JWT-based authentication** with secure token handling  
✅ **Password hashing** using bcrypt (salt rounds: 10)  
✅ **Protected API routes** with middleware validation  
✅ **Input validation** and sanitization  
✅ **SQL injection prevention** via Prisma ORM  
✅ **CORS configuration** for cross-origin security  
🔮 **Role-based access control** (future enhancement)  

---

## ⚙️ Installation & Setup

### Prerequisites
- Node.js v16 or higher
- PostgreSQL 13+
- npm or yarn

### Backend Setup

1. **Clone the repository**
```bash
git clone https://github.com/prokriti11/eventflow-pro.git
cd eventflow-pro/backend
```

2. **Install dependencies**
```bash
npm install
```

3. **Configure environment variables**
```bash
cp .env.example .env
```

Edit `.env`:
```env
DATABASE_URL="postgresql://user:password@localhost:5432/eventflow"
JWT_SECRET="your-super-secret-key"
PORT=5000
```

4. **Run database migrations**
```bash
npx prisma migrate dev
```

5. **Seed the database (optional)**
```bash
npm run seed
```

6. **Start the server**
```bash
npm start
```

Server will run on `http://localhost:5000`

### Frontend Setup

1. **Navigate to frontend directory**
```bash
cd ../frontend
```

2. **Open in browser**
```bash
# Simply open index.html in your browser
# Or use a local server:
npx serve .
```

---

## 🧪 Testing

```bash
# Run unit tests
npm test

# Run integration tests
npm run test:integration

# Test coverage
npm run test:coverage
```

---

## 📈 Scalability & Future Enhancements

### Payment Integration
- 💳 Stripe payment gateway
- 🔐 Secure payment processing
- 📧 Automated receipt generation

### AI & ML Enhancements
- 🤖 Collaborative filtering algorithms
- 🧠 Deep learning recommendation models
- 📊 Predictive analytics for event demand

### Platform Expansion
- 📱 Native mobile applications (iOS/Android)
- 🎯 Event organizer dashboards
- 📊 Admin analytics panel
- 🔔 Push notification system
- 📧 Advanced email campaigns

### Advanced Features
- 🎥 Live streaming integration
- 🏆 Gamification and rewards
- 💬 In-app chat for attendees
- 🗺️ Interactive venue maps

---

## 🧪 Use Cases

### For Users
- 🔍 Discovering local events based on interests
- 🎫 Booking tickets seamlessly
- 👥 Planning social outings with friends
- 📊 Staying updated on trending events

### For Professionals
- 💼 Finding and attending conferences
- 🎓 Networking at industry events
- 📚 Professional development workshops

### For Communities
- 🤝 Community-driven event engagement
- 🎉 Local festival organization
- 🏘️ Neighborhood gatherings

### For Organizers
- 📢 Event promotion and marketing
- 📊 Audience analytics
- 💰 Revenue optimization

---

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📝 License

© 2025 **EventFlow Pro**. All rights reserved.

This project is proprietary software. Unauthorized copying, distribution, or modification is strictly prohibited.

---

## 👥 Team

**EventFlow Pro Development Team**

For inquiries: [contact@eventflowpro.com](mailto:contact@eventflowpro.com)

---

<div align="center">

**Built with ❤️ by the EventFlow Pro Team**

⭐ **Star this repo** if you find it helpful!

</div>
