# 🏟️ TurfBooker

TurfBooker is a full-stack application designed to connect players with turf owners. It features:

- A user-friendly interface for discovering and booking sports facilities.
- A powerful admin dashboard for turf owners to manage listings, bookings, and availability.

Built with a modern tech stack — including **Next.js**, **NestJS**, **Prisma**, and **PostgreSQL** — TurfBooker provides a secure, fast, and scalable solution for both users and admins.

---

## 💻 Technology Stack

**Frontend:**
- React
- Next.js
- Tailwind CSS
- React Context API

**Backend:**
- NestJS
- Prisma ORM
- Passport.js (JWT & Google OAuth 2.0)

**Database:**
- PostgreSQL (managed locally via Docker)

---

## 🚀 Getting Started

Follow the steps below to get a local development environment up and running.

### ✅ Prerequisites

Make sure the following are installed:

- [Node.js](https://nodejs.org/)
- npm or yarn
- [Docker Desktop](https://www.docker.com/products/docker-desktop)

---

## 🔧 Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/turf-booking-app.git
2. Backend Setup
cd turf-booking-app/turf-booking-backend
npm install
Create a .env file and add your database/API credentials:
DATABASE_URL=postgresql://postgres:password@localhost:5432/turf
JWT_SECRET=your_jwt_secret
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret
Start the PostgreSQL database using Docker:
docker run --name turf-postgres -e POSTGRES_PASSWORD=password -p 5432:5432 -d postgres
Apply Prisma database migrations:
npx prisma migrate dev
3. Frontend Setup
cd ../turf-booking-frontend
npm install
Update .env.local with your backend URL if needed:
NEXT_PUBLIC_API_URL=http://localhost:3001
🖥️ Run the Application
Start the backend server:
cd ../turf-booking-backend
npm run start:dev
Start the frontend server:
cd ../turf-booking-frontend
npm run dev
The application will be available at:
👉 http://localhost:3000
📁 Project Structure
turf-booking-app/
├── turf-booking-backend/    # NestJS backend
│   ├── src/
│   ├── prisma/
│   └── .env
│
├── turf-booking-frontend/   # Next.js frontend
│   ├── pages/
│   └── .env.local
🧹 .gitignore
The project uses a consolidated .gitignore file to exclude:
Dependencies (/node_modules)
Environment files (.env*)
Build and cache output (/dist, .next/, /out)
Logs (*.log)
OS and IDE-specific files (.DS_Store, .vscode/, .idea/, etc.)
🤝 Contributing
Feel free to fork the repo and submit pull requests. Make sure to:
Format your code
Write clean commits
Test before pushing
🛡️ License
Distributed under the MIT License. See LICENSE for more information.
📬 Contact
For questions or collaborations, feel free to reach out via GitHub Issues.

Let me know if you want it tailored for deployment (e.g., Railway, Vercel, etc.) or include screenshots and API docs.
