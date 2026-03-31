# ✨ **Smart Rent Feature Documentation**

<p align="center">
  <img src="https://img.shields.io/badge/MERN-STACK-4CAF50?style=for-the-badge&labelColor=333333" />
  <img src="https://img.shields.io/badge/NODE.JS-BACKEND-FFB300?style=for-the-badge&labelColor=333333" />
  <img src="https://img.shields.io/badge/REACT-FRONTEND-2196F3?style=for-the-badge&labelColor=333333" />
  <img src="https://img.shields.io/badge/MONGODB-DATABASE-43A047?style=for-the-badge&labelColor=333333" />
</p>

A deep dive into Smart Rent’s feature behavior, covering how the platform handles listings, bookings, messaging, user flows, and more.

---

# 🧭 **1. User Features**

## 🔐 Authentication

* Secure JWT-based registration & login
* Password hashing with bcrypt
* Auth-protected routes validated server-side
* Tokens stored client-side for persistent login

**Flow:**

1. User submits credentials
2. Backend verifies → issues JWT
3. Client stores token
4. Protected requests include `Authorization: Bearer <token>`

---

## 🏡 Property Listings

* Browse properties with category-based filtering
* Search by price, location, amenities, number of guests
* Mobile-friendly listing grid
* Map preview via Leaflet
* Property detail page includes:

  * Photo gallery
  * Amenities
  * Host profile
  * Rating
  * Booking widget

**Flow:**

1. Frontend sends filters
2. Backend returns matching results
3. UI updates instantly

---

## 📅 Bookings

* Date picker for check-in & check-out
* Automatic total price calculation
* Clash prevention with existing bookings
* Stores booking details in user dashboard
* Cancel upcoming stays

**Flow:**

1. User chooses dates
2. Backend checks availability
3. Booking created if valid
4. Confirmation returned

---

## 🧳 Trip Management

* View upcoming stays
* View past stays
* Cancel future bookings
* Direct link to leave a review

---

## ⭐ Reviews

* Users leave ratings after completed stays
* Displayed on property detail pages
* Rating average recalculated in real time

---

## ❤️ Wishlist

* Save & remove properties
* Persisted in database
* Synced across sessions/devices

---

## 👤 Profile Management

* Edit profile information
* Upload avatars via Cloudinary
* View personal reviews
* See account-level activity

---

# 🏠 **2. Host Features**

## 📝 Listing Creation

* Multi-step listing form
* Upload photos (Cloudinary storage)
* Add pricing, amenities, location
* Modify or delete existing listings

---

## 📊 Booking Management

* Hosts view guest bookings
* See stay dates, guest info, and payment totals
* Manage booking cancellations (if feature enabled)

---

## 💬 Messaging with Guests

* Host ↔ Guest real-time chat
* Messages stored in conversations
* Typing indicators & timestamps

---

## 📈 Host Analytics

* Metrics include:

  * Total bookings
  * Listing performance
  * Average rating
* Helps hosts optimize listings

---

# 🛠️ **3. Admin Features**

## 👥 User Management

* View, edit, and moderate accounts
* Handle profile violations and bans

---

## 🏡 Property Moderation

* Approve/deny property listings
* Take down reported or fraudulent listings

---

## 📅 System-Wide Booking View

* All booking activity visible to admins
* Useful for dispute resolution

---

## 🚨 Report Handling

* Users can report:

  * Properties
  * Hosts
  * Guests
  * Messages
* Admin dashboard shows pending reports

---

# 🌐 **4. Key Pages Overview**

| Page                    | Purpose                            |
| ----------------------- | ---------------------------------- |
| **Home**                | Category slider, trending listings |
| **Listings**            | Search, filters, map view          |
| **Property Detail**     | Gallery, reviews, booking widget   |
| **Become Host**         | Listing creation form              |
| **Account**             | Profile, wishlist, trips           |
| **Messages**            | Chat interface                     |
| **Help / Policy pages** | FAQ, terms, privacy, cancellations |

---

# 🗄️ **5. Database Models (Feature Behavior)**

Each feature interacts with the following core models:

| Model            | Used For                                   |
| ---------------- | ------------------------------------------ |
| **User**         | Authentication, profile, wishlist          |
| **Property**     | Listing details, amenities, host reference |
| **Booking**      | Reservations & trip management             |
| **Review**       | Ratings & comments                         |
| **Message**      | Chat system storage                        |
| **Conversation** | Thread grouping for chat                   |

---

# 🧪 **6. Sample Data Categories**

Smart Rent includes 40+ category types:

* Apartments
* Villas
* Cabins
* Treehouses
* Domes
* Containers
* Beachfront
* Mountain homes
* Luxury homes
* Tiny homes
* Castles
* Windmills

---

# 🏁 **7. Feature Summary Table**

| Feature        | Description                           |
| -------------- | ------------------------------------- |
| Authentication | JWT login/logout, protected routes    |
| Listings       | Filters, categories, maps             |
| Bookings       | Date validation & availability checks |
| Messaging      | Real-time Socket.io communication     |
| Reviews        | Ratings & comment submission          |
| Wishlist       | Saved properties per user             |
| Host Tools     | Listing creation & management         |
| Admin Tools    | Moderation & global monitoring        |
