# Multi-Vendor E-Commerce — Backend API

Node.js/Express REST API serving the customer app, vendor app, and admin panel for a multi-vendor e-commerce platform.

## Features

- **Authentication** — JWT-based auth for customers, vendors, and admins with bcrypt password hashing
- **Products** — create, update, filter by category/subcategory, search, popular and top-rated lists
- **Orders** — full order lifecycle: creation, status updates (processing → delivered), payment tracking
- **Vendors** — vendor registration, store profiles, product and order management
- **Categories & Subcategories** — organized product taxonomy with banner images
- **Banners** — homepage promotional banner management
- **Payments** — Stripe card payments + Cash on Delivery (COD)

## Tech Stack

- Node.js + Express 4.19.2
- MongoDB + Mongoose 8.3.1
- bcryptjs — password hashing
- jsonwebtoken — JWT auth
- cors — cross-origin support

## Getting Started

```bash
npm install
node index.js
```

Create a `.env` file with the following:

```
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
STRIPE_SECRET_KEY=your_stripe_secret
```

## API Routes

| Prefix | Description |
|--------|-------------|
| `/api/auth` | Customer sign up, sign in, profile |
| `/api/vendors` | Vendor sign up, sign in, store management |
| `/api/products` | Product CRUD, search, filtering |
| `/api/orders` | Order creation, status updates, history |
| `/api/categories` | Category and subcategory management |
| `/api/banners` | Homepage banner management |

## Related Repositories

| Repo | Role |
|------|------|
| **backend-api** | Node.js/Express REST API + MongoDB |
| [customer-app](https://github.com/YoussefAlaaSaad/customer-app) | Flutter mobile app for shoppers |
| [vendor-app](https://github.com/YoussefAlaaSaad/vendor-app) | Flutter mobile app for vendors |
| [admin-panel](https://github.com/YoussefAlaaSaad/admin-panel) | Flutter web dashboard for admins |
