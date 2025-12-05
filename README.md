# 🌟 **Smart Rent – Modern MERN Property Rental Platform**

<p align="center">
  <img src="https://img.shields.io/badge/MERN-Stack-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Node.js-Backend-yellow?style=for-the-badge" />
  <img src="https://img.shields.io/badge/React-Frontend-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/MongoDB-Database-brightgreen?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Status-Active-success?style=for-the-badge" />
</p>

<p align="center">
  A polished, full-stack rental platform that brings together guests, hosts, and admins with real-time interactions, seamless booking flows, and a stunning UI experience.
</p>

---

# ✨ **Overview**

Smart Rent is a complete property rental ecosystem built on the MERN stack.
It delivers:

* Smooth property browsing with filters
* Secure JWT authentication
* Real-time messaging powered by Socket.io
* Host listing workflows
* Booking + trip management for guests
* Admin dashboard for moderation
* Fully responsive, modern UI with Tailwind

Designed to look good. Built to scale.

---

# 🔥 **Feature Highlights**

### 👤 **Guest Experience**

* JWT-based login & registration
* Explore properties with category slider
* Powerful search + dynamic filters
* Instant booking with calendars
* Trip history & booking management
* Real-time chat with hosts
* Write & read reviews
* Wishlist favorite homes

---

### 🏡 **Host Experience**

* Create advanced property listings
* Upload images (Cloudinary integration)
* Manage bookings from guests
* Chat with guests instantly
* View analytics & reviews

---

### 🛠️ **Admin Panel**

* User account management
* Listing moderation
* Booking monitoring
* Handle reports & concerns

---

# 🧠 **Tech Stack**

<p align="center">
  <img src="https://skillicons.dev/icons?i=react,nodejs,express,mongodb,tailwind,js" />
</p>

### **Frontend**

* React 18
* TailwindCSS
* React Router v7
* Axios
* Leaflet Maps
* Context API

### **Backend**

* Node.js + Express
* MongoDB + Mongoose
* JWT Authentication
* Cloudinary Uploads
* Socket.io Messaging
* Nodemailer
* Helmet + Mongo Sanitize
* Joi Validation

---

# 🏗️ **Project Structure**

```
smart-rent/
│
├─ backend/
│  ├─ controllers/     # Route logic
│  ├─ models/          # DB schemas
│  ├─ routes/          # API endpoints
│  ├─ middleware/      # Auth, error handling
│  ├─ services/        # Email, utilities
│  ├─ app.js
│  └─ server.js
│
├─ frontend/
│  ├─ src/
│  │  ├─ components/   # Reusable UI
│  │  ├─ pages/
│  │  ├─ contexts/     # Auth, Settings
│  │  ├─ hooks/
│  │  ├─ services/     # API calls
│  │  ├─ utils/
│  │  ├─ data/
│  │  ├─ App.js
│  │  └─ index.js
│
└─ docs/
   ├─ API.md
   ├─ FEATURES.md
   ├─ CONTRIBUTING.md
   └─ UI-UX.md
```

---

# 🚀 **Getting Started**

## **Backend Setup**

```bash
cd backend
npm install
```

Create `.env`:

```env
PORT=8000
MONGODB_URI=
JWT_SECRET=
CLOUDINARY_NAME=
CLOUDINARY_KEY=
CLOUDINARY_SECRET=
EMAIL_USER=
EMAIL_PASS=
```

Start backend:

```bash
npm run dev
```

→ Runs at: `http://localhost:8000`

---

## **Frontend Setup**

```bash
cd frontend
npm install
npm start
```

→ Runs at: `http://localhost:3000`

---

# 🌍 **Environment Variables**

### Backend

```env
PORT
MONGODB_URI
JWT_SECRET
CLOUDINARY_NAME
CLOUDINARY_KEY
CLOUDINARY_SECRET
EMAIL_USER
EMAIL_PASS
NODE_ENV
```

### Frontend

```env
REACT_APP_API_URL
```

---

# 🧪 **Scripts**

### Backend

* `npm run dev` — Development with nodemon
* `npm start` — Production build

### Frontend

* `npm start`
* `npm run build`

---

# 📘 **Documentation Index**

| Documentation       | Description                                  |
| ------------------- | -------------------------------------------- |
| **[API.md](./API.md)**              | All API routes with request/response samples |
| **[FEATURES.md](./FEATURES.md)**    | Deep dive into feature behavior              |
| **[CONTRIBUTING.md](./CONTRIBUTING.md)** | Branch rules, code style, PR process |

---

# 📦 **Deployment**

### Backend

* Render / Railway / VPS
* MongoDB Atlas setup
* Environment variables added

### Frontend

* Vercel / Netlify
* Deploy build folder
* Configure `REACT_APP_API_URL`

---

# 🤝 **Contributing**

Pull requests are welcome!
See **[CONTRIBUTING.md](./CONTRIBUTING.md)**  for rules, workflow, and commit conventions.

---

# 📄 **License**

ISC License — use freely with attribution.

---

# 💬 **Support**

For any issues, create a GitHub Issue or contact the maintainers.
