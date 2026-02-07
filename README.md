# 🎥 VideoConnect

### Enterprise-Grade Full Stack Video Conferencing Platform

A modern, scalable, and production-ready video conferencing platform built with **Spring Boot, React, WebSockets, and AgoraRTC**, designed for real-time communication, collaboration, and secure meeting management.

---

## 🌍 Live Demo (Optional but Powerful)

> 🔗 Add deployed frontend link here
> 🔗 Add backend API link (if hosted)

---

## ✨ Key Highlights

* 🔐 Secure JWT Authentication & Authorization
* 🎥 Real-time Video & Audio Streaming (AgoraRTC)
* 💬 Live Chat System using WebSockets (STOMP over SockJS)
* 🏠 Dynamic Meeting Room Creation & Management
* 👥 Real-time Participant Tracking
* 📝 Meeting History & Records
* 📱 Fully Responsive UI (Mobile Friendly)
* ⚡ High Performance RESTful APIs
* 🧩 Clean Architecture (Frontend & Backend Separation)

---

## 🏗️ System Architecture

Client (React + Vite)
⬇ REST + WebSocket
Spring Boot Backend
⬇
MySQL Database
⬇
Agora Cloud (Media Streaming)

---

## 🛠️ Tech Stack

### 💻 Backend

* Spring Boot
* Spring Security + JWT
* JPA (Hibernate)
* MySQL
* WebSockets (STOMP + SockJS)
* REST API Architecture

### 🌐 Frontend

* React (Vite)
* Tailwind CSS
* AgoraRTC SDK
* Axios
* React Router
* WebSocket Client (SockJS + STOMP)

---

## 🔐 Security Implementation

* JWT-based stateless authentication
* Protected API routes
* Secure WebSocket messaging
* Password encryption (BCrypt)
* Role-based access (extendable)

---

## 📡 Real-Time Communication

WebSocket Endpoint:

```
ws://localhost:8080/ws
```

Subscriptions:

```
/topic/chat/{roomId}
/topic/participants/{roomId}
```

Agora handles:

* Audio streaming
* Video streaming
* Channel-based room communication

---

## 🗄️ Database Design (Core Tables)

* users
* meetings
* participants
* chat_messages

(You can add ER diagram screenshot here for next-level polish 🔥)

---

## ⚙️ Installation & Setup

### 🔧 Prerequisites

* Java 17+
* Node.js 18+
* MySQL
* Maven
* Agora Developer Account

---

## 🧪 Backend Setup

```bash
cd backend
```

Create database:

```sql
CREATE DATABASE videoconnect;
```

Update `application.properties`:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/videoconnect
spring.datasource.username=root
spring.datasource.password=yourpassword

spring.jpa.hibernate.ddl-auto=update

jwt.secret=your_secure_secret_key

agora.app-id=your_agora_app_id
```

Run backend:

```bash
./mvnw spring-boot:run
```

---

## 🎨 Frontend Setup

```bash
cd frontend
npm install
```

Create `.env` file:

```
VITE_BACKEND_URL=http://localhost:8080
VITE_AGORA_APP_ID=your_agora_app_id
```

Run frontend:

```bash
npm run dev
```

---

## 📡 REST API Overview

| Method | Endpoint             | Description    |
| ------ | -------------------- | -------------- |
| POST   | /api/auth/register   | Register user  |
| POST   | /api/auth/login      | Login          |
| POST   | /api/meetings/create | Create meeting |
| GET    | /api/meetings        | Fetch meetings |
| GET    | /api/meetings/{id}   | Join meeting   |

---

## 🧠 Advanced Features

* Real-time bidirectional communication
* Scalable backend design
* Modular frontend architecture
* Extendable for:

  * Screen Sharing
  * Cloud Recording
  * PWA Support
  * Meeting Analytics
  * Email Notifications

---

## 📸 UI Preview

Add screenshots like:

* Login Page
* Dashboard
* Meeting Room
* Chat Panel

(Repositories with screenshots look 10x more serious.)

---

## 📦 Tools & Development Environment

* IntelliJ IDEA
* VS Code
* Postman
* MySQL Workbench
* Agora Console

---

## 🧪 Future Roadmap

* 🎥 Screen Sharing
* 📼 Cloud Recording
* 📊 Meeting Analytics Dashboard
* 🔔 Real-time Notifications
* 🧾 Meeting Summary & Notes
* 🧠 AI-based Meeting Insights

---

## 🤝 Contribution

Currently maintained and developed by:

**Souvik Kamila**

If you’d like to collaborate:

```bash
git clone https://github.com/yourusername/VideoConnect.git
```

---

## 📄 License

This project is for educational and portfolio purposes.

---

