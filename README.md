# Chatty

## 📖 Project Overview
Chatty is a full-stack real-time chat application designed to enable instant, seamless messaging between users. It uses WebSockets for real-time communication, ensuring that messages are delivered instantly without the need for page reloads.

## 🚀 Features
- **Real-Time Messaging:** Send and receive messages instantly with zero delay.
- **Secure Authentication:** User signup and login system to protect accounts.
- **Live Online Status:** See which users are currently online and active.
- **Persistent Chat History:** Seamlessly load past conversations and messages.
- **Responsive Design:** A beautiful UI that works perfectly on both mobile phones and desktop browsers.
- **Profile Management:** Users can manage their accounts and personalize their profiles.

## 💻 Tech Stack

| Category | Technologies |
| :--- | :--- |
| 🎨 **Frontend** | React 19 <br> Vite (TypeScript) <br> Tailwind CSS v4 <br> Zustand <br> React Query <br> Socket.io-client <br> React Hook Form & Zod |
| ⚙️ **Backend** | Node.js <br> Express.js <br> MongoDB (Mongoose) <br> Redis <br> Socket.io <br> JWT & bcryptjs |
| 🐳 **DevOps** | Docker <br> Docker Compose |

## ⚡ Quickstart Guide

1. **Clone the repository:**
   ```bash
   git clone <repo-url>
   cd chatty
   ```

2. **Setup environment variables:**
   - Create `backend/.env` (Requires `PORT`, `MONGO_URI`, `JWT_SECRET`, and `REDIS_URL`).
   - Create `frontend/.env` (Requires `VITE_API_URL`).

## 💻 Running Locally

### 1. Start the Backend
Open a terminal and run:
```bash
cd backend
npm install
npm run dev
```

### 2. Start the Frontend
Open a new terminal window and run:
```bash
cd frontend
npm install
npm run dev
```

## 🐳 Docker Deployment
You can use Docker Compose to easily spin up the required background services (like Redis or MongoDB) without installing them locally.

```bash
cd backend
docker-compose up -d
```
This will start the services defined in `backend/docker-compose.yaml` in the background.
