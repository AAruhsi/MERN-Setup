# MERN Setup

A complete **MERN** (MongoDB, Express, React, Node.js) stack application template with backend API and React frontend.

## 📋 Table of Contents

- [Prerequisites](#prerequisites)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Environment Variables](#environment-variables)
- [Running the Application](#running-the-application)
- [API Documentation](#api-documentation)
- [Technologies Used](#technologies-used)

## 📦 Prerequisites

Before you begin, ensure you have installed:

- **Node.js** (v16 or higher) - [Download](https://nodejs.org/)
- **npm** or **yarn** - Comes with Node.js
- **MongoDB Atlas Account** - [Create Free Account](https://www.mongodb.com/cloud/atlas)
- **Git** - [Download](https://git-scm.com/)

## 📁 Project Structure

```
MERN Setup/
├── backend/
│   ├── server.js
│   ├── package.json
│   ├── .env (create this)
│   └── .gitignore
├── client/
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── .gitignore
└── README.md
```

## 🚀 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/AAruhsi/MERN-Setup.git
cd MERN-Setup
```

### 2. Install Backend Dependencies

```bash
cd backend
npm install
```

### 3. Install Client Dependencies

```bash
cd ../client
npm install
```

## ⚙️ Environment Variables

### Backend Setup

Create a `.env` file in the `backend` folder:

```bash
cd backend
```

Add the following variables:

```env
PORT=5000
ATLAS_URI=mongodb+srv://username:password@cluster.mongodb.net/dbname
NODE_ENV=development
```

**How to get MongoDB Atlas URI:**
1. Go to [MongoDB Atlas](https://www.mongodb.com/cloud/atlas)
2. Create a cluster
3. Go to "Connect" → "Connect your application"
4. Copy the connection string and replace with your credentials

## 🎯 Running the Application

### Development Mode

**Terminal 1 - Start Backend:**
```bash
cd backend
npm run dev
```
Backend runs on `http://localhost:5000`

**Terminal 2 - Start Frontend:**
```bash
cd client
npm run dev
```
Frontend runs on `http://localhost:5173` (or as shown in terminal)

### Production Mode

**Backend:**
```bash
cd backend
npm start
```

**Client:**
```bash
cd client
npm run build
```

## 📡 API Documentation

### Current Endpoints

- Base URL: `http://localhost:5000`

More endpoints to be added...

## 🛠️ Technologies Used

### Backend
- **Express.js** - Web framework
- **MongoDB** - NoSQL database
- **Mongoose** - MongoDB object modeling
- **CORS** - Cross-Origin Resource Sharing
- **Dotenv** - Environment variable management
- **Nodemon** - Auto-restart development server

### Frontend
- **React** - UI library
- **Vite** - Build tool

## 📝 Scripts

### Backend Scripts
```bash
npm start    # Run production server
npm run dev  # Run development server with auto-reload
```

### Client Scripts
```bash
npm run dev      # Start development server
npm run build    # Build for production
npm run preview  # Preview production build
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit changes (`git commit -m 'Add amazing feature'`)
4. Push to branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the ISC License - see the LICENSE file for details.

## 💡 Tips

- Keep your `.env` file secure and never commit it to version control
- Use `git pull` before starting work to stay updated
- Check MongoDB Atlas status if connection fails
- Ensure ports 5000 and 5173 are not in use

## 🆘 Troubleshooting

**MongoDB Connection Error:**
- Verify ATLAS_URI in `.env` is correct
- Check if IP is whitelisted in MongoDB Atlas

**Port Already in Use:**
- Change PORT in `.env` to a different port
- Or kill the process using the port

**Module Not Found:**
- Run `npm install` in respective folders
- Delete `node_modules` and reinstall if issues persist

---

**Happy Coding! 🎉**
