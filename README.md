# Fullstack Real-Time Chat Application

A comprehensive real-time chat application built using the MERN stack (MongoDB, Express, React, Node.js) and Socket.io for live communication.

## 🚀 Features

- **Real-Time Messaging**: Instant messaging between users powered by Socket.io.
- **Authentication & Authorization**: Secure user login and registration using JWT (JSON Web Tokens).
- **Online Status Indicator**: See who's currently online in real-time.
- **Media Sharing**: Upload and share images within chats, powered by Cloudinary.
- **Global State Management**: Fast and scalable frontend state management utilizing Zustand.
- **Modern UI/UX**: Beautiful, responsive design built with Tailwind CSS and DaisyUI.
- **Robust Error Handling**: Comprehensive error handling on both the client and server sides.

## 💻 Tech Stack

### Frontend
- **React 18** (Vite)
- **Tailwind CSS** + **DaisyUI**
- **Zustand** (State Management)
- **Socket.io-Client**
- **Axios**
- **React Router**

### Backend
- **Node.js** + **Express.js**
- **MongoDB** + **Mongoose**
- **Socket.io** (WebSockets)
- **Cloudinary** (Image hosting)
- **JWT** & **Bcryptjs** (Security)

## 🛠️ Getting Started

### Prerequisites

Make sure you have [Node.js](https://nodejs.org/) and [npm](https://www.npmjs.com/) installed on your machine. You will also need a MongoDB database and a Cloudinary account for image hosting.

### 1. Clone the repository
```shell
git clone https://github.com/brishibhatia/FullStackchatApp.git
cd FullStackchatApp
```

### 2. Install Dependencies

The project uses concurrently to install and run both frontend and backend scripts.

```shell
# Install backend dependencies
cd backend
npm install

# Install frontend dependencies
cd ../frontend
npm install
```

### 3. Environment Variables

Create a `.env` file in the `backend` directory and configure the following variables:

```env
# MongoDB Connection String
MONGODB_URI=your_mongodb_connection_string

# Server Port
PORT=5001

# JWT Secret Key
JWT_SECRET=your_jwt_secret_key

# Cloudinary Setup for image uploads
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret

# Environment
NODE_ENV=development
```

## 🏃‍♂️ Running Locally

To start the application in development mode (with hot-reloading for both backend and frontend):

**Backend:**
```shell
cd backend
npm run dev
```

**Frontend:**
```shell
cd frontend
npm run dev
```

The frontend will typically run on `http://localhost:5173` and the backend on `http://localhost:5001`.

## 📦 Building for Production

To build the frontend and serve it from the Node.js backend:

```shell
# From the root directory
npm run build
npm start
```

## 📄 License

This project is licensed under the ISC License.
