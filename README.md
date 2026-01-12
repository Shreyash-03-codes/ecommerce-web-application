# 🛒 E-commerce Web Application

A **full-stack E-commerce web application** built using **Angular** for the frontend and **Spring Boot** for the backend. This project demonstrates real-world features such as user authentication, product management, cart & order handling, and secure payment integration using **Stripe**.

---

## 🚀 Tech Stack

### Frontend
- **Angular**
- TypeScript
- Bootstrap & Bootstrap Icons
- Stripe JS (publishable key only)

### Backend
- **Spring Boot**
- Spring Security (JWT Authentication)
- Spring Data JPA (Hibernate)
- PostgreSQL
- Stripe Payment Gateway

---

## ✨ Features

### 👤 User & Authentication
- User registration & login
- JWT-based authentication
- Role-based access control (Admin / User)

### 🛍️ Product Management
- View product listings
- Product categories
- Admin product management (CRUD)

### 🛒 Cart & Orders
- Add/remove items from cart
- Update product quantities
- Place orders
- Order history tracking

### 💳 Payments
- Secure online payments using **Stripe**
- Stripe Payment Intent flow
- No secret keys exposed in frontend or repository

---

## 🏗️ Project Architecture

```
ecommerce-web-application/
│
├── frontend/        # Angular application
│
├── backend/         # Spring Boot application
│   ├── controller/
│   ├── service/
│   ├── repository/
│   ├── entity/
│   └── security/
│
└── README.md
```

---

## 🔐 Environment Variables (Important)

> ⚠️ **Secrets are NOT committed to this repository**

Create a `.env` file locally (ignored by Git):

```env
DB_PASSWORD=your_db_password
STRIPE_SECRET_KEY=sk_test_xxxxxxxxxxxxxx
```

Update `application.properties` to use environment variables:

```properties
spring.datasource.password=${DB_PASSWORD}
stripe.secret-key=${STRIPE_SECRET_KEY}
```

---

## ▶️ Running the Application

### Backend (Spring Boot)
```bash
cd backend
./mvnw spring-boot:run
```

Backend runs on:
```
http://localhost:8080
```

---

### Frontend (Angular)
```bash
cd frontend
npm install
ng serve
```

Frontend runs on:
```
http://localhost:4200
```

---

## 🧪 Testing
- Backend unit & integration tests using JUnit
- Stripe secrets mocked via environment variables

---

## 🔒 Security Best Practices Followed

- ❌ No API keys committed
- ✅ Environment variable based secrets
- ✅ GitHub Push Protection compliant
- ✅ JWT-based authentication

---

## 📌 Future Improvements

- Product reviews & ratings
- Order invoice generation
- Docker & Docker Compose setup
- CI/CD with GitHub Actions
- Deployment on AWS / Render

---

## 👨‍💻 Author

**Shreyash Gurav**  
Full Stack Developer (Angular | Spring Boot)

---

## ⭐ Support

If you like this project, please ⭐ the repository and share your feedback!

---

> *This project is built for learning, portfolio, and real-world full-stack development practice.* 🚀

