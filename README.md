# Nepify

A full-stack e-commerce web app built with the MERN stack. Users can browse products, add them to a cart or wishlist, place orders, and track them. There's a separate admin panel to manage products and orders.

## What it does

- Sign up and log in with email verification via OTP
- Browse products and view product details
- Add items to cart or wishlist
- Place orders and go through a checkout flow
- Track your order history from your profile
- Admins can add, update, or remove products and manage all orders from a dashboard
- Forgot password and reset password via email

## Tech stack

**Frontend** — React, Redux Toolkit, React Router

**Backend** — Node.js, Express, MongoDB (Mongoose)

**Auth** — JWT, bcryptjs, OTP via Nodemailer

## Project structure

```
nepify/
├── frontend/   # React app (Redux, routing, pages)
└── backend/    # Express API (routes, controllers, models)
```

## Getting started

### Backend

```bash
cd backend
npm install
```

Create a `.env` file in the `backend` folder:

```
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
EMAIL_USER=your_email@gmail.com
EMAIL_PASS=your_email_app_password
FRONTEND_URL=http://localhost:3000
```

Then run:

```bash
npm run dev
```

### Frontend

```bash
cd frontend
npm install
npm start
```

The app runs on `http://localhost:3000` and connects to the backend at `http://localhost:8000` by default.

## Seed data

To add some sample products to the database:

```bash
cd backend
npm run seed
```
