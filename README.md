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

(Add screenshots here after implementation)

---

## Author

Jatin Singh Solanki
