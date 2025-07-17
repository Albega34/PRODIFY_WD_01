# 🚀 Deploy MERN App (Frontend + Backend)

This project is a full-stack **MERN (MongoDB, Express, React, Node.js)** web application with integrated **user authentication** and **product routing**. It is structured to support **deployment on Vercel** for both frontend and backend services.

## 🧩 Project Structure

```
deploy-mern-app-1-main/
├── backend/       # Node.js + Express API
├── frontend/      # React App
```

---

## 📦 Backend (Node.js + Express)

### Features:
- User authentication (JWT-based)
- Middleware validation
- MongoDB integration using Mongoose
- RESTful API for users and products

### Key Files:
- `index.js`: App entry point
- `Controllers/`: Logic for routes
- `Routes/`: Auth and Product routers
- `Models/`: Mongoose models (User, DB connection)
- `Middlewares/`: Auth and Validation handlers

### Run Locally:
```bash
cd backend
npm install
npm run dev
```

> Make sure to set your MongoDB URI and JWT secret in `.env`

---

## 💻 Frontend (React)

### Features:
- Functional React app
- User login and registration
- Product UI (depends on backend data)
- Environment configuration ready for Vercel

### Key Files:
- `App.js`: Root component
- `RefrshHandler.js`: Handles token refresh logic
- Public assets and metadata files

### Run Locally:
```bash
cd frontend
npm install
npm start
```

> Configure `.env` to point to your backend server

---

## 🚀 Deployment

### Vercel:
Both `frontend` and `backend` folders contain `vercel.json` for custom configuration.

- Set up two Vercel projects: one for the frontend and one for the backend.
- Add environment variables in the Vercel dashboard.
- Frontend should call the backend via Vercel’s provided URL.

---

## 📁 Environment Variables

### Backend (`/backend/.env`)
```
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
```

### Frontend (`/frontend/.env`)
```
REACT_APP_API_
```

---


## 🙌 Acknowledgments

Special thanks to the open-source community and tools that made building and deploying this MERN app smooth and efficient.

---

## 📬 Contact

For suggestions, contributions, or issues, feel free to open an issue or submit a pull request.
