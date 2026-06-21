# 🌱 EcoTrack – Carbon Footprint Awareness Platform

EcoTrack is a full-stack **MERN-based Carbon Footprint Awareness Platform** designed to help users understand, calculate, track, and reduce their environmental impact.

The platform converts everyday lifestyle choices—such as transportation, electricity consumption, food habits, shopping, and waste management—into understandable carbon-emission insights. Users can track their progress, participate in eco-friendly challenges, earn points, and build sustainable habits.

## 🚀 Live Demo

🔗 **Deployed Project:**
https://carbon-foo--sonakumar5858.replit.app/

---

## 📌 Project Objective

Climate change is one of the biggest challenges faced by the world today. Many people want to adopt sustainable habits but are unaware of how their daily activities contribute to carbon emissions.

EcoTrack aims to make sustainability simple, measurable, and actionable by allowing users to:

* Calculate their estimated carbon footprint
* Understand which activities generate more emissions
* Track carbon footprint history
* Receive personalized suggestions
* Participate in eco-friendly challenges
* Earn eco points and badges
* Learn about sustainability
* Engage with an eco-conscious community

---

## ✨ Features

### 🧮 Carbon Footprint Calculator

Users can calculate their estimated carbon footprint based on:

* Transportation habits
* Distance travelled
* Vehicle type and fuel usage
* Electricity consumption
* LPG and appliance usage
* Food and diet preferences
* Shopping habits
* Plastic usage
* Recycling habits
* Waste generation

### 📊 Personal Dashboard

The dashboard helps users track their sustainability journey through:

* Current carbon footprint score
* Previous footprint records
* Carbon footprint breakdown
* Emission category charts
* Eco points
* Completed challenges
* Carbon savings
* Sustainable habit progress
* Personalized recommendations

### 🌍 Eco Challenges

Users can participate in sustainability challenges such as:

* Plastic-Free Week
* No Car Day
* Vegetarian Week
* Save Electricity Challenge
* Reusable Bottle Challenge
* Walk 5 km Challenge
* Zero Food Waste Day
* Public Transport Week
* Plant a Tree Challenge

Users can join challenges, update progress, complete them, and earn eco points.

### 📚 Sustainability Learning Hub

The platform includes awareness content related to:

* Climate change basics
* Carbon footprint awareness
* Sustainable transportation
* Renewable energy
* Eco-friendly food habits
* Recycling and waste management
* Sustainable lifestyle choices

### 👥 Community Section

Users can interact with the EcoTrack community by:

* Sharing eco tips
* Posting sustainability updates
* Sharing challenge completion updates
* Liking posts
* Commenting on posts
* Viewing community leaderboard rankings

### 🔐 Secure Authentication

* User registration and login
* JWT-based authentication
* Password hashing using bcrypt
* Protected routes
* Secure user dashboard access
* Persistent login using local storage

### 📱 Responsive Design

EcoTrack is designed to work smoothly on:

* Desktop
* Laptop
* Tablet
* Mobile devices

---

## 🛠 Tech Stack

### Frontend

* React.js
* Vite
* Tailwind CSS
* React Router DOM
* Axios
* Recharts
* React Toastify
* Lucide React Icons

### Backend

* Node.js
* Express.js
* MongoDB
* Mongoose
* JSON Web Token (JWT)
* bcrypt.js

### Tools and Deployment

* GitHub
* Replit
* MongoDB Atlas
* Postman
* VS Code

---

## 📂 Project Structure

```bash
ecotrack/
│
├── client/
│   ├── src/
│   │   ├── assets/
│   │   ├── components/
│   │   ├── context/
│   │   ├── hooks/
│   │   ├── pages/
│   │   ├── services/
│   │   ├── utils/
│   │   ├── App.jsx
│   │   └── main.jsx
│   ├── package.json
│   └── vite.config.js
│
├── server/
│   ├── config/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   ├── seed/
│   ├── utils/
│   ├── server.js
│   └── package.json
│
├── .env.example
└── README.md
```

---

## 🔗 API Endpoints

### Authentication APIs

| Method | Endpoint             | Description                |
| ------ | -------------------- | -------------------------- |
| POST   | `/api/auth/register` | Register a new user        |
| POST   | `/api/auth/login`    | Login user                 |
| GET    | `/api/auth/me`       | Get logged-in user details |

### User APIs

| Method | Endpoint                 | Description           |
| ------ | ------------------------ | --------------------- |
| GET    | `/api/users/profile`     | Get user profile      |
| PUT    | `/api/users/profile`     | Update user profile   |
| GET    | `/api/users/leaderboard` | Get leaderboard users |

### Carbon Footprint APIs

| Method | Endpoint                 | Description                  |
| ------ | ------------------------ | ---------------------------- |
| POST   | `/api/footprints`        | Save carbon footprint result |
| GET    | `/api/footprints`        | Get user footprint history   |
| GET    | `/api/footprints/latest` | Get latest footprint result  |
| DELETE | `/api/footprints/:id`    | Delete a footprint record    |

### Challenge APIs

| Method | Endpoint                        | Description               |
| ------ | ------------------------------- | ------------------------- |
| GET    | `/api/challenges`               | Get all eco challenges    |
| POST   | `/api/challenges/:id/join`      | Join a challenge          |
| PUT    | `/api/challenges/:id/progress`  | Update challenge progress |
| PUT    | `/api/challenges/:id/complete`  | Complete a challenge      |
| GET    | `/api/challenges/my-challenges` | Get joined challenges     |

### Community APIs

| Method | Endpoint                 | Description           |
| ------ | ------------------------ | --------------------- |
| GET    | `/api/posts`             | Get community posts   |
| POST   | `/api/posts`             | Create a new post     |
| PUT    | `/api/posts/:id/like`    | Like or unlike a post |
| POST   | `/api/posts/:id/comment` | Add a comment         |
| DELETE | `/api/posts/:id`         | Delete own post       |

---

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/ecotrack.git
cd ecotrack
```

### 2. Install Frontend Dependencies

```bash
cd client
npm install
```

### 3. Install Backend Dependencies

```bash
cd ../server
npm install
```

### 4. Create Environment Variables

Create a `.env` file inside the `server` folder.

```env
PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
CLIENT_URL=http://localhost:5173
```

Create a `.env` file inside the `client` folder.

```env
VITE_API_URL=http://localhost:5000/api
```

### 5. Start the Backend Server

```bash
cd server
npm run dev
```

The backend server will run on:

```bash
http://localhost:5000
```

### 6. Start the Frontend Application

Open a new terminal:

```bash
cd client
npm run dev
```

The frontend application will run on:

```bash
http://localhost:5173
```

---

## 🧠 Carbon Footprint Calculation Categories

EcoTrack estimates emissions from the following areas:

| Category       | Examples                                |
| -------------- | --------------------------------------- |
| Transportation | Car, bike, bus, train, metro, flights   |
| Home Energy    | Electricity, LPG, AC, water heater      |
| Food           | Vegan, vegetarian, non-vegetarian diet  |
| Shopping       | Online shopping and product consumption |
| Waste          | Plastic usage, recycling, food waste    |

The calculator combines category-wise emissions to generate:

* Total carbon footprint
* Carbon score
* Emission breakdown
* Personalized sustainability recommendations

---

## 🎯 Carbon Score Categories

| Score Level | Meaning                                              |
| ----------- | ---------------------------------------------------- |
| Excellent   | Very low carbon footprint                            |
| Good        | Sustainable lifestyle with room for improvement      |
| Moderate    | Average footprint; improvements recommended          |
| High        | Higher emissions; action required                    |
| Critical    | Significant emissions; immediate changes recommended |

---

## 🧩 Challenges Faced

### 1. Designing Carbon Calculation Logic

Different activities produce different levels of carbon emissions. The solution was to divide the calculator into structured categories such as transportation, energy, food, shopping, and waste.

### 2. Managing Multi-Step Form Data

The carbon calculator includes multiple user inputs across different steps. This was handled using reusable React components, validation, progress indicators, and organized state management.

### 3. Secure Authentication

The application needed protected user dashboards and secure data access. JWT authentication, bcrypt password hashing, and protected backend routes were implemented.

### 4. Visualizing Complex Data

Carbon emission data can be difficult to understand. Charts, progress indicators, emission categories, eco points, and suggestions were used to make the data clear and engaging.

### 5. Responsive User Interface

The platform was designed to work across mobile, tablet, and desktop screens using Tailwind CSS, responsive grids, reusable components, and a mobile navigation menu.

---

## 📈 Future Enhancements

* Integration with real-time carbon emission APIs
* AI-based personalized sustainability recommendations
* Google Maps integration for greener travel routes
* Carbon offset donation system
* Social sharing for completed eco challenges
* Push notifications and reminders
* Gamification with levels and rewards
* Mobile application using React Native or Flutter
* Admin dashboard for managing users, challenges, and articles

---

## 👨‍💻 Author

**Ravi Kumar**

* GitHub: Add your GitHub profile link here
* LinkedIn: Add your LinkedIn profile link here
* Email: Add your email address here

---

## 🤝 Contributions

Contributions, issues, and feature requests are welcome.

1. Fork this repository
2. Create a new branch
3. Make your changes
4. Commit your changes
5. Push the branch
6. Create a Pull Request

---

## 📄 License

This project is created for educational, portfolio, hackathon, and awareness purposes.

---

## 🌎 Final Note

EcoTrack is built with the belief that small sustainable actions can create a large collective impact.

**Track today. Protect tomorrow.** 🌱
