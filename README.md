# 📊 CRM Application - MERN Stack

A simple and beginner-friendly Customer Relationship Management (CRM) system built with the MERN stack (MongoDB, Express.js, React.js, and Node.js).

## 🎯 Features

- **User Authentication**: Secure registration and login with JWT tokens
- **Customer Management**: Complete CRUD operations (Create, Read, Update, Delete)
- **Responsive Design**: Works on desktop, tablet, and mobile devices
- **Form Validation**: Input validation and error handling
- **User-Friendly Interface**: Clean and modern design

## 🛠️ Technologies Used

### Backend
- Node.js
- Express.js
- MongoDB
- Mongoose
- JWT (JSON Web Tokens)
- Bcrypt.js

### Frontend
- React.js
- React Router
- Axios
- CSS3

## 📁 Project Structure

```
crm-mern-app/
├── backend/
│   ├── config/
│   │   └── db.js              # MongoDB connection
│   ├── models/
│   │   ├── User.js            # User model
│   │   └── Customer.js        # Customer model
│   ├── routes/
│   │   ├── auth.js            # Authentication routes
│   │   └── customers.js       # Customer CRUD routes
│   ├── middleware/
│   │   └── auth.js            # JWT verification middleware
│   ├── .env                    # Environment variables
│   ├── server.js              # Main server file
│   └── package.json
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   │   ├── Login.js
│   │   │   ├── Register.js
│   │   │   ├── Dashboard.js
│   │   │   ├── CustomerForm.js
│   │   │   └── Navbar.js
│   │   ├── services/
│   │   │   └── api.js         # API service
│   │   ├── App.js
│   │   └── App.css
│   └── package.json
└── README.md
```

## 🚀 Setup Instructions

### Prerequisites
- Node.js (v14 or higher)
- MongoDB (local or MongoDB Atlas)
- npm or yarn

### Backend Setup

1. **Navigate to backend folder**
   ```bash
   cd backend
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Configure environment variables**
   - Open the `.env` file
   - Update `MONGO_URI` with your MongoDB connection string
   - Update `JWT_SECRET` with a secure secret key

   ```env
   MONGO_URI=mongodb://localhost:27017/crm_database
   JWT_SECRET=your_super_secret_jwt_key_here_change_this
   PORT=5000
   ```

4. **Start the backend server**
   ```bash
   npm start
   ```
   
   Or for development with auto-reload:
   ```bash
   npm run dev
   ```

   The backend will run on `http://localhost:5000`

### Frontend Setup

1. **Open a new terminal and navigate to frontend folder**
   ```bash
   cd frontend
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the frontend development server**
   ```bash
   npm start
   ```

   The frontend will run on `http://localhost:3000`

## 📝 API Endpoints

### Authentication
- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - Login user

### Customers (Protected Routes)
- `GET /api/customers` - Get all customers
- `POST /api/customers` - Create new customer
- `PUT /api/customers/:id` - Update customer
- `DELETE /api/customers/:id` - Delete customer

## 🎨 Features Breakdown

### User Authentication
- Secure registration with password hashing
- Login with JWT token generation
- Token-based authentication for protected routes
- Automatic logout functionality

### Customer Management
- **Create**: Add new customers with validation
- **Read**: View all customers in a responsive grid
- **Update**: Edit customer information
- **Delete**: Remove customers with confirmation

### Responsive Design
- Mobile-friendly interface
- Clean and modern UI
- Gradient backgrounds
- Smooth animations and transitions

## 🐛 Troubleshooting

**Backend not starting?**
- Make sure MongoDB is running
- Check if port 5000 is available
- Verify environment variables in `.env`

**Frontend not connecting to backend?**
- Ensure backend is running on port 5000
- Check `API_URL` in `frontend/src/services/api.js`

**MongoDB connection error?**
- Verify MongoDB is running
- Check connection string in `.env`
- For MongoDB Atlas, ensure your IP is whitelisted

## 👨‍💻 Author

Created as part of MERN Stack Assignment - Enhancing CRM Solutions with MERN Integration

## 📄 License

This project is created for educational purposes.



