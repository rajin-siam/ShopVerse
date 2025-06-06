# 🛒 ShopVerse - Full-Stack E-Commerce Platform

**ShopVerse** is a full-featured e-commerce platform offering a modern shopping experience. The backend is powered by **Spring Boot** and the frontend by **React + Vite**. It supports product browsing, cart management, secure payments, user profiles, and an admin dashboard.

> 🎥 **Demo Video**:

[Watch the video](https://youtu.be/oOdKLAR-aLU)

---

## 🔗 Live Demo & Repositories

### Live Demo
* Frontend: [https://shopverse-frontend-rabt.onrender.com](https://shopverse-frontend-rabt.onrender.com)
* Backend API: [https://shopverse-backend-u9q6.onrender.com](https://shopverse-backend-u9q6.onrender.com)

### Source Code
* Backend Repository: [https://github.com/rajin-siam/ShopVerse-Backend](https://github.com/rajin-siam/ShopVerse-Backend)
* Frontend Repository: [https://github.com/rajin-siam/ShopVerse-Frontend](https://github.com/rajin-siam/ShopVerse-Frontend)

### Deployment
* Frontend and Backend: Deployed on [Render](https://render.com)
* Database: MySQL hosted on [Railway](https://railway.app)

---

### User Account and Password
* username: user1, admin
* password: password1, adminPass

## 📦 Tech Stack

### Backend

* Java 17, Spring Boot 3.3.5
* Spring Security, JWT Authentication
* MySQL, Spring Data JPA
* Stripe Integration
* Google OAuth2
* Swagger/OpenAPI for API docs

### Frontend

* React with Vite
* React Router v6, Context API
* Tailwind CSS
* React Hot Toast for notifications
* Google OAuth2 & JWT

---

## 🚀 Features

### 👤 User Features

* Register/Login via email or Google
* Role-based access control (User/Admin)
* Update profile and manage addresses
* Wishlist and order history

### 🛍️ Shopping Experience

* Product listing, filtering, and searching
* Ratings and reviews for products
* Add to cart, manage cart items
* Multi-step checkout with Stripe payment
* Order confirmation and tracking

### 🛠️ Admin Features

* Dashboard for analytics
* Product & inventory management
* Category & order management

---

## 🗂️ Project Structure

### Backend (Spring Boot)

```
src/
├── controllers/
├── services/
├── repositories/
├── models/
├── security/
├── config/
└── util/
```

### Frontend (React + Vite)

```
src/
├── assets/
├── common/
│   ├── components/
│   ├── constants/
│   ├── contexts/
│   └── hooks/
├── features/
│   ├── admin/
│   ├── auth/
│   ├── cart/
│   ├── checkout/
│   ├── home/
│   ├── products/
│   └── user/
├── pages/
└── shared/
```

---

## ⚙️ Installation & Setup

### Backend

#### Prerequisites:

* Java 17
* MySQL
* Maven
* Stripe & Google API credentials

#### Environment Variables (`.env`)

```env
SPRING_DATASOURCE_URL=jdbc:mysql://localhost:3306/ecommerce2
SPRING_DATASOURCE_USERNAME=root
SPRING_DATASOURCE_PASSWORD=root
JWT_SECRET=your_jwt_secret_key
JWT_EXPIRATION_MS=86400000
JWT_COOKIE_NAME=shopverse
STRIPE_API_KEY=your_stripe_api_key
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret
PROJECT_IMAGE_DIR=images/
PORT=8080
```

#### Run the backend:

```bash
git clone https://github.com/yourusername/shopverse.git
cd shopverse
./mvnw clean install
./mvnw spring-boot:run
```

App will run at: `http://localhost:8080`

#### Swagger API Docs:

* Swagger UI: `/swagger-ui/`
* OpenAPI Spec: `/v3/api-docs/`

### Frontend

#### Setup:

```bash
git clone https://github.com/yourusername/shopverse-frontend.git
cd shopverse-frontend
npm install
```

#### Environment Variables (`.env`)

```env
VITE_API_BASE_URL=http://localhost:8080/api
```

#### Run the frontend:

```bash
npm run dev
```

App will run at: `http://localhost:5174`

---

## 🐳 Docker Support (Backend)

To containerize the backend:

```bash
docker build -t shopverse .
docker run -p 8080:8080 shopverse
```

---

## 📱 Responsive Design

* Fully responsive for mobile, tablet, and desktop
* Tailwind CSS ensures consistent styling across devices

---

## 📄 License

This project is licensed under the **MIT License** – see the LICENSE file for details.

---


