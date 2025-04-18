# Movie Squad: MERN Stack Single-Page Application
![License](https://img.shields.io/badge/License-MIT-blue.svg)
<img alt="React" src="https://img.shields.io/badge/React-18+-blue.svg">
<img alt="GraphQL" src="https://img.shields.io/badge/GraphQL-16+-purple.svg">
<img alt="Apollo" src="https://img.shields.io/badge/Apollo-3.7+-blueviolet.svg">
<img alt="MongoDB" src="https://img.shields.io/badge/MongoDB-4.4+-green.svg">
<img alt="Express" src="https://img.shields.io/badge/Express-4.17+-green.svg">
<img alt="Node.js" src="https://img.shields.io/badge/Node.js-16+-green.svg">

## Project Overview
Movie Squad is an interactive full MERN stack single page application designed to help movie buffs save lists of their favorite movies and write reviews. Users can create watchlists, rate movies, write reviews and comment on other user reviews.

## Key Features

- **Movie Search (Using OMDB API)**
  - See top rated movies.
  - Enter a **movie name** and get results for that movie.
  - Options to **rate** the movie, add to a list of saved movies, and add to a movie watchlist.
  - View and write **movie reviews**.

- **Movie Reviews**
  - **Write reviews** on movies.
  - **Comment** on user reviews.

- **Saved Movies and Movie Watchlist**
  - **Save a list** of movies you have seen.
  - **Create a watchlist** of movies you are interested in.

## Live Deployment

[Movie Squad live](https://moviesquad.onrender.com/)

## Screenshots

### **Homepage:**
![MovieSquad-Homepage](https://github.com/user-attachments/assets/760959ef-e3d5-4fab-9b41-5ecb1355a4d1)

### **Profile Page:**
![Profile page](https://github.com/user-attachments/assets/88d091e0-c2d8-4105-bf8a-da2522d1342d)

### **Movie Search/Watchlist**
![watchlist page](https://github.com/user-attachments/assets/e61559f1-cc9a-4ec3-ba73-9d7d0ed41d8d)
![filled watchlist](https://github.com/user-attachments/assets/fd0f146e-e6f0-417c-b468-046be99e3c55)


## Project Setup

### **1️⃣ Clone the Repository**
```sh
git clone <repository_url>
cd moviesquad
```

### **2️⃣ Install Dependencies**
```sh
npm install
```

### **3️⃣ Setup Environment Variables**
To use the required APIs, each team member must create a `.env` file with their own API keys. Follow these steps:

1. **Copy the `.env.example` file**
   ```sh
   cp .env.example .env
   ```
2. **Open the `.env` file and add your API keys**
   ```plaintext
   OMDB_API_KEY=your_omdb_key_here
   MONGODB_URI=your_mongodb_uri_here
   ```
3. **Save the file.**

🔹 **Important:** `.env` is included in `.gitignore` and **should never be committed** to GitHub.

### **4️⃣ Start the Development Server**
```sh
npm run develop
```

### **5️⃣ Update `.gitignore`**
Ensure `.gitignore` includes the `.env` file:
```plaintext
# Environment Variables
.env
.env.local
.env.*.local
```
If not, add these lines **manually** to prevent accidental commits of API keys.

---

## API Endpoints & Usage

### 🔹 Movie Search
**Get**
#### 🔹 **Returns**: A list of movies.
```json
[
    {
        "movieId": "1",
        "title": "Inception",
        "posterPath": "https://image.tmdb.org/t/p/w500/9gk7adHYeDvHkCSEqAvQNLV5Uge.jpg",
        "description": "A thief who steals corporate secrets through the use of dream-sharing technology is given the inverse task of planting an idea into the mind of a CEO.",
        "releaseDate": "2010-07-16",
        "year": 2010,
        "director": "Christopher Nolan",
        "actors": ["Leonardo DiCaprio", "Joseph Gordon-Levitt", "Elliot Page"],
        "genres": ["Sci-Fi", "Action", "Thriller"]
    }
]
```

## Deployment Guide

- **Ensure your `.env` file is set up.**
- Deploy on **Render** as a **Web Service**.
- Ensure the database **(MongoDB) is set up and connected through MongoDB Atlas**.

## API Integrations
Movie Squad integrates the OMDB API to view movies, descriptions and more.

## Technologies Used
### **Frontend:** 
- **React** (TypeScript, Vite)
- **React Router** (Navigation)
- **TailwindCSS** (Styling)
### **Backend:** 
- **Node.js, Express.js** (Server)
- **TypeScript** (For static type safety)
- **OMDB API** (Movie Search)
- **PostgreSQL** (Sequelize ORM)
- **JWT Authentication** (Secure login system)
### **Other Tools:** 
- **Render** (Deployment)
- **MongoDB Atlas** (Database)
- **ApolloSandbox** (Queries)

## Future Enhancements
- Allow users to make threads for discussing movies
- Implement reviews and comments for movies
- Implement movie rating
- Sorting and searching of movies by genre, year, type (live-action, animated)
