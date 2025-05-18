# Elegance Jewels E-Commerce Platform

A full-stack e-commerce application built with Node.js, React, and MongoDB.

## Features

- User authentication (Firebase Auth)
- Product browsing and filtering by category
- Detailed product views with images and descriptions
- Shopping cart functionality
- Checkout with direct credit card processing or cash on delivery
- Order processing and tracking
- PDF receipt generation
- Admin dashboard for managing products, orders, and users
- Responsive UI with Bootstrap

## Tech Stack

### Backend
- Node.js
- Express.js
- MongoDB
- Firebase Authentication
- PDF Generation (jsPDF)

### Frontend
- React.js
- Redux Toolkit
- React Router
- Bootstrap 5
- Axios
- React Toastify
- jsPDF for receipt generation

## Project Structure

```
ecom-project/
├── client/              # React frontend
│   ├── public/
│   └── src/
│       ├── components/  # Reusable UI components
│       ├── pages/       # Page components
│       ├── contexts/    # React contexts
│       ├── redux/       # Redux state management
│       ├── utils/       # Utility functions
│       └── ...
└── server/              # Node.js backend
    ├── config/          # Configuration files
    ├── controllers/     # Route controllers
    ├── middleware/      # Custom middleware
    ├── models/          # MongoDB models
    └── routes/          # API routes
```

## Getting Started

### Prerequisites

- Node.js (v14 or higher)
- MongoDB account (MongoDB Atlas setup)
- Firebase account (for authentication)

### Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd ecom-project
   ```

2. Install dependencies for the server:
   ```bash
   cd server
   npm install
   ```

3. Install dependencies for the client:
   ```bash
   cd ../client
   npm install
   ```

4. Set up Firebase authentication:
   ```bash
   cd ../server
   npm run setup-firebase
   ```
   Follow the prompts to configure Firebase authentication.

5. Start the server:
   ```bash
   cd ../server
   npm run dev
   ```

6. Start the client:
   ```bash
   cd ../client
   npm start
   ```

7. Open your browser and navigate to `http://localhost:3000`.

## Troubleshooting

If you encounter issues during setup or running the application, please refer to the [Troubleshooting Guide](TROUBLESHOOTING.md) for solutions to common problems.

## API Endpoints

### Authentication
- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - Login user
- `GET /api/auth/me` - Get current user
- `GET /api/auth/logout` - Logout user

### Products
- `GET /api/products` - Get all products
- `GET /api/products/:id` - Get single product
- `POST /api/products` - Create a product (Admin only)
- `PUT /api/products/:id` - Update a product (Admin only)
- `DELETE /api/products/:id` - Delete a product (Admin only)

### Categories
- `GET /api/categories` - Get all categories
- `GET /api/categories/:id` - Get single category
- `POST /api/categories` - Create a category (Admin only)
- `PUT /api/categories/:id` - Update a category (Admin only)
- `DELETE /api/categories/:id` - Delete a category (Admin only)

### Orders
- `GET /api/orders` - Get all orders (Admin only)
- `GET /api/orders/:id` - Get single order
- `POST /api/orders` - Create an order
- `PUT /api/orders/:id` - Update an order (Admin only)
- `GET /api/orders/my-orders` - Get user orders

### Users
- `GET /api/users` - Get all users (Admin only)
- `GET /api/users/:id` - Get single user (Admin only)
- `PUT /api/users/:id` - Update a user (Admin only)
- `DELETE /api/users/:id` - Delete a user (Admin only)
- `PUT /api/users/profile` - Update user profile
"# ProjetFinAnn-e" 
