## 🔗 **API Endpoints**

### 🔐 **Authentication**

* `POST /api/auth/register` — Register new user
* `POST /api/auth/login` — Login user
* `POST /api/auth/logout` — Logout user

---

### 🏡 **Properties**

* `GET /api/properties` — Get all properties
* `GET /api/properties/:id` — Get property details
* `POST /api/properties` — Create property (host only)
* `PUT /api/properties/:id` — Update property
* `DELETE /api/properties/:id` — Delete property

---

### 📅 **Bookings**

* `GET /api/bookings` — Get user bookings
* `POST /api/bookings` — Create booking
* `GET /api/bookings/:id` — Get booking details
* `PUT /api/bookings/:id` — Update booking
* `DELETE /api/bookings/:id` — Cancel booking

---

### 💬 **Messages**

* `GET /api/messages` — Get conversations
* `GET /api/messages/:conversationId` — Get messages in conversation
* `POST /api/messages` — Send message
* `POST /api/messages/create-conversation` — Create conversation

---

### ⭐ **Reviews**

* `GET /api/reviews/:propertyId` — Get property reviews
* `POST /api/reviews` — Create review
* `PUT /api/reviews/:id` — Update review
* `DELETE /api/reviews/:id` — Delete review

---

### 👤 **Users**

* `GET /api/users/:id` — Get user profile
* `PUT /api/users/:id` — Update user profile
* `GET /api/users/:id/reviews` — Get user reviews
