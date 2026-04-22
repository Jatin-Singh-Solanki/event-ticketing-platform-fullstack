# Event Ticketing Platform (Full-Stack)

## Overview

A full-stack **Event Ticketing Platform** that allows users to browse events, purchase tickets, and manage bookings, while organizers can create events, manage seat tiers, and track performance.

This project demonstrates real-world implementation of **scalable backend APIs**, **modern frontend architecture**, and **database-driven workflows**.

---

## Tech Stack

**Backend**

* Node.js
* Express.js
* TypeScript
* Prisma ORM
* SQLite

**Frontend**

* Next.js (App Router)
* TypeScript
* Tailwind CSS

**Authentication**

* JWT (JSON Web Tokens)
* bcrypt password hashing

**Other**

* QR Code generation for tickets

---

## Features

* User Authentication (Login/Register)
* Event Listing & Details
* Seat Tier Management
* Promo Code Support
* Ticket Booking System
* Booking Cancellation & Refund Logic
* QR Code Ticket Generation
* Organizer Dashboard (Analytics & Stats)

---

## Project Structure

```
backend/
  src/
    routes/
    middleware/
    lib/
  prisma/

frontend/
  src/
    app/
    components/
    contexts/
    lib/
    types/
```

---

## Getting Started

### 1. Install Dependencies

```
npm run install:all
```

### 2. Setup Database

```
npm run db:setup
```

### 3. Run Application

```
npm run dev
```

---

## Application URLs

* Frontend: http://localhost:3000
* Backend API: http://localhost:4000

---

## Test Credentials

**Organizer**

* [organizer1@example.com](mailto:organizer1@example.com) / organizer123

**Attendee**

* [alice@example.com](mailto:alice@example.com) / attendee123

---

## Environment Variables

### Backend (`backend/.env`)

```
DATABASE_URL="file:./dev.db"
JWT_SECRET="your-secret-key"
PORT=4000
FRONTEND_URL="http://localhost:3000"
```

### Frontend (`frontend/.env.local`)

```
NEXT_PUBLIC_API_URL=http://localhost:4000
```

---

```
## Project Structure

```bash
.
├── backend
│   ├── src
│   │   ├── index.ts                # Express app entry point
│   │   ├── routes                 # API routes
│   │   │   ├── auth.ts
│   │   │   ├── events.ts
│   │   │   ├── bookings.ts
│   │   │   ├── checkin.ts
│   │   │   ├── dashboard.ts
│   │   │   ├── tiers.ts
│   │   │   ├── promoCodes.ts
│   │   │   └── waitlist.ts
│   │   ├── middleware             # Auth middleware
│   │   │   └── auth.ts
│   │   ├── lib                    # Core utilities
│   │   │   ├── jwt.ts
│   │   │   ├── qr.ts
│   │   │   ├── capacity.ts
│   │   │   ├── transfer.ts
│   │   │   ├── validations.ts
│   │   │   └── prisma.ts
│   ├── prisma
│   │   ├── schema.prisma          # Database schema
│   │   │── seed.ts                # Seed data
│   └── package.json

├── frontend
│   ├── src
│   │   ├── app                    # Next.js App Router
│   │   │   ├── page.tsx           # Home (events list)
│   │   │   ├── events/[id]        # Event details & booking
│   │   │   ├── bookings           # User bookings
│   │   │   ├── tickets/[id]       # Ticket QR view
│   │   │   ├── login              # Login page
│   │   │   ├── register           # Register page
│   │   │   └── dashboard          # Organizer dashboard
│   │   ├── components             # UI components
│   │   ├── contexts               # Global state (Auth)
│   │   ├── lib                    # API & utilities
│   │   │   ├── api.ts
│   │   │   └── utils.ts
│   │   └── types                  # TypeScript types
│   └── package.json

├── submission                     # Screenshots for evaluation
├── DECISIONS.md                   # Design decisions
├── USER_REQUIREMENTS.md           # Feature requirements
├── package.json                   # Root scripts
└── README.md
```
```

## Key Modules

* Booking System → Ticket purchase & cancellation
* Capacity Management → Seat availability tracking
* Transfer Utility → Ticket reassignment logic
* QR Module → Ticket verification

---

## Improvements & Future Enhancements

* Ticket Transfer Feature (User-to-User)
* Event Waitlist System
* Payment Gateway Integration
* Email Notifications
* Role-based access improvements
* Security enhancements (rate limiting, validation hardening)

---

## Screenshots

<img width="1536" height="1024" alt="test1-create-promo-code" src="https://github.com/user-attachments/assets/9fa525f6-b408-4bd4-8ef4-3fd48aa07cd2" />


---

## Author

Jatin Singh Solanki
