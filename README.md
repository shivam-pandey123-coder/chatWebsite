# ChatApplication
# 💬 Real-Time Chat Application

A full-stack real-time chat application built with the **MERN Stack** (MongoDB, Express.js, React.js, Node.js) and **Socket.io** for real-time, bidirectional communication between users.

---

## 📋 Table of Contents
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Project Structure](#-project-structure)
- [Installation](#-installation)
- [Usage](#-usage)
- [API Documentation](#-api-documentation)
- [Contributing](#-contributing)
- [License](#-license)

---

## 🚀 Features

- 🔒 **User Authentication** (Register / Login with JWT tokens)
- 🧑‍🤝‍🧑 **One-to-One Chat Functionality** (Direct messaging between users)
- 🧠 **Real-Time Messaging** with Socket.io (Instant message delivery and notifications)
- 📦 **RESTful APIs** with Express.js (Scalable backend architecture)
- 💾 **MongoDB Database** for user and message storage (NoSQL document management)
- 📱 **Responsive Frontend** with React and Tailwind CSS (Mobile-friendly UI)
- 🖼️ **Rich UI** for chat layout and message threads (Intuitive user experience)
- ✅ **Message Status Tracking** (Sent, delivered, read status)
- 🔔 **Real-Time Notifications** (User online/offline status)
- 🔐 **Secure Authentication** with JWT tokens and password hashing

---

## 🛠️ Tech Stack

### Frontend:
- **React.js** - UI library for building interactive components
- **Tailwind CSS** - Utility-first CSS framework for styling
- **Axios** - HTTP client for API requests
- **Socket.io-client** - Real-time communication library
- **Vite** - Next-generation frontend tooling (Fast builds and HMR)

### Backend:
- **Node.js** - JavaScript runtime environment
- **Express.js** - Web framework for building APIs
- **MongoDB & Mongoose** - NoSQL database and ODM for data persistence
- **Socket.io** - Real-time bidirectional communication
- **JWT (jsonwebtoken)** - Secure token-based authentication
- **bcrypt** - Password hashing and security

---

## 📁 Project Structure

```
chatWebsite/
├── Frontend-of-chat-website/       # React frontend application
│   ├── src/
│   │   ├── components/             # React components
│   │   ├── pages/                  # Page components
│   │   ├─�� context/                # Context API for state management
│   │   └── App.jsx                 # Main app component
│   └── package.json
│
├── Backend/                        # Node.js backend server
│   ├── models/                     # Mongoose schemas
│   ├── routes/                     # API routes
│   ├── controllers/                # Route handlers
│   ├── middleware/                 # Authentication & validation
│   ├── socket/                     # Socket.io events
│   ├── server.js                   # Main server file
│   └── package.json
│
└── README.md                       # Project documentation
```

---

## 💻 Installation

### Prerequisites
- Node.js (v14 or higher)
- MongoDB (local or cloud instance)
- npm or yarn package manager

### Clone the Repository
```bash
git clone https://github.com/shivam-pandey123-coder/chatWebsite.git
cd chatWebsite
```

### Backend Setup
```bash
cd Backend
npm install

# Create .env file with:
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
PORT=5000
```

### Frontend Setup
```bash
cd Frontend-of-chat-website
npm install

# Create .env file with:
VITE_API_URL=http://localhost:5000
VITE_SOCKET_URL=http://localhost:5000
```

---

## 🚀 Usage

### Start Backend Server
```bash
cd Backend
npm start
# Server runs on http://localhost:5000
```

### Start Frontend Development Server
```bash
cd Frontend-of-chat-website
npm run dev
# Application runs on http://localhost:5173
```

### Build for Production
```bash
# Frontend
npm run build

# Backend
# Ensure NODE_ENV=production in .env
```

---

## 📡 API Documentation

### Authentication Endpoints
- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - User login
- `POST /api/auth/logout` - User logout

### User Endpoints
- `GET /api/users` - Get all users
- `GET /api/users/:id` - Get user profile
- `PUT /api/users/:id` - Update user profile

### Message Endpoints
- `GET /api/messages/:userId` - Get chat history with a user
- `POST /api/messages` - Send a message
- `DELETE /api/messages/:messageId` - Delete a message

### Socket Events
- `connect` - User connects to socket
- `disconnect` - User disconnects
- `send_message` - Emit new message
- `receive_message` - Listen for incoming messages
- `user_online` - User comes online
- `user_offline` - User goes offline

---

## 🔐 Authentication & Security

- JWT tokens are used for secure authentication
- Passwords are hashed using bcrypt before storage
- Protected routes require valid JWT tokens
- CORS is configured for secure cross-origin requests
- Socket.io connections are authenticated

---

## 🤝 Contributing

Contributions are welcome! Follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📝 License

This project is open source and available under the MIT License.

---

## 📧 Contact & Support

For issues, questions, or suggestions, please open an issue in the [GitHub repository](https://github.com/shivam-pandey123-coder/chatWebsite/issues).

---

## 🎯 Future Enhancements

- [ ] Group chat functionality
- [ ] Message search and filtering
- [ ] User typing indicators
- [ ] Message reactions/emojis
- [ ] File and image sharing
- [ ] End-to-end encryption
- [ ] User presence indicators
- [ ] Message edit and delete functionality

---

**Happy Chatting! 💬**
