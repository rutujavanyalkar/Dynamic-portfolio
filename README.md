# 🌐 Dynamic Portfolio — MERN Stack

A full-stack dynamic portfolio website built using the **MERN Stack** (**MongoDB, Express.js, React.js, Node.js**).  
This portfolio is fully dynamic, where personal details, skills, projects, and contact information are managed through backend APIs and stored in MongoDB, making updates easy without changing frontend code repeatedly.

---

## 🚀 Tech Stack

| Layer       | Technology |
|------------|------------|
| Frontend   | React.js |
| Backend    | Node.js, Express.js |
| Database   | MongoDB Atlas |
| ODM        | Mongoose |
| Env Mgmt   | dotenv |

---

## 📁 Project Structure

```bash
mern-portfolio/
├── config/
│   └── dbConfig.js         # MongoDB connection setup
├── routes/
│   └── portfolioRoute.js   # API routes for portfolio data
├── server.js              # Express app entry point
├── staticData.js          # Seed/static data
├── .env                   # Environment variables (not committed)
├── package.json
└── README.md
```

## ⚙️ Getting Started

### 📌 Prerequisites

- Node.js (v16 or above)
- MongoDB Atlas Account
- npm

---

### 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/mern-portfolio.git
cd mern-portfolio
```

### 2️⃣ Install Dependencies

```bash
npm install
```
### 3️⃣ Configure Environment Variables

Create a .env file in the root directory:
```bash
mongo_url=your_mongodb_connection_string
PORT=5000
```
⚠️ Never commit your .env file. Add it to .gitignore.

### 4️⃣ Run Project

Development Mode
```bash
npx nodemon server.js
```
Production Mode
```bash
node server.js
```

### 5️⃣ Server URL
```bash
http://localhost:5000
```

## 🔌 API Endpoints
```bash
Base URL: /api/Portfolio
```
| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | /intro | Fetch intro data |
| GET | /about | Fetch about data |
| GET | /contacts | Fetch contact data |

## 🌱 Static Data

The staticData.js file includes:

Intro Section
About Section
Contact Section
### 🔒 Security Notes
Store credentials in .env
Add .env to .gitignore
Never expose MongoDB URI publicly
Use separate environment variables for production
### 📦 Dependencies
```bash
{
  "cors": "^2.8.5",
  "dotenv": "^16.4.5",
  "express": "^4.19.2",
  "mongoose": "^8.5.1",
  "nodemon": "^3.1.4"
}
```


