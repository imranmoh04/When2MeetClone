# 🗓️ Final Exam - Group Scheduling App (When2Meet Clone)

## 📌 Overview

This is the final project for **CSE 477: Web Application Development (Spring 2025)**. The application is a clone and extension of [When2Meet](https://www.when2meet.com), a group scheduling platform that allows users to collaboratively determine the best meeting time using an interactive grid-based interface.

The primary goal of this project is to demonstrate mastery of core web development concepts, including:

- Reactive frontend design
- Secure, data-driven backend architecture
- Real-time client synchronization using WebSockets
- Persistent session and state management
- Full-stack deployment using Docker and Google Cloud

---

## 🔐 Features

### 1. **User Authentication**
- Secure sign-up and login with encrypted passwords
- Session-based authentication with protected routes

### 2. **Event Management**
- **Create Event**: Users can create new events by specifying name, date range, daily hours, and invitee list
- **Join Event**: Invitees can view and access events they were invited to

### 3. **Availability Grid**
- Interactive grid of 30-minute slots across selected dates
- Users can mark each time slot as:
  - ✅ Available (Green)
  - 🤔 Maybe (Yellow)
  - ❌ Unavailable (Gray)
- Drag-to-select and click interactions supported
- Selections are stored and rendered persistently

### 4. **Heatmap Visualization**
- Dynamic color intensity to reflect group availability
- Live feedback based on the number of available participants

### 5. **Best Time Calculation**
- Highlights the most optimal meeting time using:
  1. Max "Available" count
  2. Fewest "Unavailable"
  3. Earliest time in case of ties

### 6. **Real-Time Sync (WebSockets)**
- All availability updates, heatmaps, and best time calculations are synchronized across all active clients **without page refresh**
- Built using a WebSocket-based architecture (e.g., Socket.IO or native WebSocket API)

---

## 🛠️ Tech Stack

- **Frontend**: React.js / Vue.js / Svelte (choose your stack)
- **Backend**: Node.js with Express / Flask / Django (choose your backend)
- **Database**: PostgreSQL / MongoDB (as required)
- **Authentication**: Sessions with bcrypt hashing
- **Real-Time Communication**: WebSockets
- **Deployment**: Docker + Google Cloud Run

---

## 🚀 Deployment Instructions

1. **Clone the Repository**
   ```bash
   git clone https://gitlab.com/your-username/final-exam.git
   cd final-exam
