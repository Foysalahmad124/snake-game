
# 🐍 Snake Game API + Web UI

Node.js + Express + MongoDB backend with a playable Snake web UI.

---

## 📦 Installation

```bash
npm install

# create .env
copy .env.example .env

# run dev
npm run dev

# run prod
npm start
```

---

## ⚙️ Environment Variables (`.env`)

```env
PORT=5000
NODE_ENV=development
MONGO_URI=mongodb://localhost:27017/snake_game_db
JWT_SECRET=your_secret_key_here
JWT_EXPIRE=7d
```

---

## 📁 Folder Structure

```
snake-api/
├── config/
│   └── db.js              # MongoDB connection
├── controllers/
│   ├── authController.js  # Auth logic
│   └── scoreController.js # Score logic
├── middleware/
│   ├── auth.js            # JWT protect middleware
│   ├── errorHandler.js    # Global error handler
│   └── validators.js      # Input validation
├── models/
│   ├── User.js            # User schema
│   └── Score.js           # Score schema
├── public/
│   ├── index.html         # Game UI
│   ├── styles.css         # UI styles
│   └── app.js             # Game logic + API sync
├── routes/
│   ├── auth.js            # Auth routes
│   └── scores.js          # Score routes
├── .env.example
├── package.json
└── server.js              # Entry point
`

## 🛠 Tech Stack

- Node.js
- Express.js
- MongoDB + Mongoose
- JWT + bcryptjs
- express-validator
- helmet, cors, express-rate-limit
- morgan
