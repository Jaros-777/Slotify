# 🛎️ Slotify
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=Vite&logoColor=white)
![React](https://img.shields.io/badge/-ReactJs-61DAFB?logo=react&logoColor=black&style=for-the-badge)
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)
![License](https://img.shields.io/github/license/Jaros-777/slotify-frontend?style=for-the-badge)



**Slotify** is an educational, full-stack appointment booking application inspired by **Reservio**.  
This project was built for learning purposes and as a portfolio piece, showcasing modern web development practices, clean architecture, and deployment strategies.

> ⚠️ This is **not a commercial project**. It is intended purely for educational purposes.

---
# 🌍 Live Demo
### 🔗[LIVE DEMO](https://slotify7.netlify.app/)

## 🎥 Video

[![Watch the demo](https://img.youtube.com/vi/rlHsbHehBqY/maxresdefault.jpg)](https://youtu.be/rlHsbHehBqY)



## 🌟 Features

- 🧑‍🤝‍🧑 User registration, login, and account management  
- 📅 Create, edit, and delete bookings  
- 🕒 View available time slots and manage appointments  
- 📱 Mobile view available **only on Home and Booking pages**  
- 💻 Admin interface **desktop-only**  
- 🛎️ Customers can book services online  
- 🌴 Vacation mode for users  
- 📋 Client list with CSV export  
- 🎨 Responsive design and clean UI  
- 🏗️ Full-stack separation: **Frontend** + **Backend**  
- 🐳 Easy setup with **Docker Compose** or manual setup  
- 🧹 Clean, modular, and maintainable codebase for learning purposes  

---

## 🛠 Technologies Used

### Frontend  
![React](https://img.shields.io/badge/React-61DAFB?logo=react&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?logo=vite&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?logo=tailwind-css&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-0db7ed?logo=docker&logoColor=white)
![Axios](https://img.shields.io/badge/Axios-5A29E4?logo=axios&logoColor=white)
* **Framework:** React.JS + TypeScript + Vite  
* **Styling:** Tailwind CSS / SCSS  
* **Containerization:** Docker   
* **API Requests:** Axios

### Backend
![Java](https://img.shields.io/badge/Java-ED8B00?logo=openjdk&logoColor=white)
![Spring](https://img.shields.io/badge/Spring-6DB33F?logo=spring&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?logo=postgresql&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?logo=supabase&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-C71A36?logo=apachemaven&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-0db7ed?logo=docker&logoColor=white)
* **Language:** Java 20+
* **Framework:** Spring Boot 3.x
* **Database (local):** PostgreSQL, Supabase (only for storage profiles and services pictures)
* **Database (prod):** Supabase
* **Build Tool:** Maven
* **Containerization:** Docker

### DevOps / Deployment
![Docker](https://img.shields.io/badge/Docker-0db7ed?logo=docker&logoColor=white)
![Docker Compose](https://img.shields.io/badge/Docker_Compose-2496ED?logo=docker&logoColor=white)
- **Docker & Docker Compose** for containerized setup  
- Environment variables for configuration  
- Ready for local development and deployment  

---

## 📦 Installation & Setup

### 🐳 Running Slotify with Docker Compose

You can run the full Slotify application using Docker Compose. Follow these steps carefully.

### 1️⃣ Clone the repositories

Clone the **main repo**, as well as **frontend** and **backend** repositories:

```bash
# Main repo
git clone https://github.com/Jaros-777/Slotify.git
cd Slotify

# Frontend repo
git clone https://github.com/Jaros-777/slotify-frontend.git frontend

# Backend repo
git clone https://github.com/Jaros-777/slotify-backend.git backend
```
Make sure the folder structure looks like this:
```bash
Slotify/
├─ slotify-frontend/      <-- React frontend project
├─ slotify-backend/       <-- Spring Boot backend project
└─ docker-compose.yml
```
### 2️⃣ Prepare Docker Compose file
1. Locate the file named:
```docker-compose.example.yml```

2. Rename it to remove ".example":
```mv docker-compose.example.yml docker-compose.yml```

3. Edit paths if needed in ```docker-compose.yml``` to point to the correct frontend and backend folders. For example:
```bash
services:
  backend:
    build:
      context: ./backend    # <- make sure this points to your backend folder or paste full path e.g. C:\Users\User\Desktop\slotify-backend

  frontend:
    build:
      context: ./frontend   # <- make sure this points to your frontend folder or paste full path e.g. C:\Users\User\Desktop\slotify-frontend
```
This step is important if you cloned the repos into custom folder names.

### 3️⃣ Run Docker Compose
Build and start all services:  
```docker-compose up --build```
- Backend will be available at: http://localhost:8080  
- Frontend will be available at: http://localhost:3000  




### 🖥️ Run Frontend or Backend separately
To run frontend or backend separately, please go to the respective repositories for setup instructions:
- Frontend repo - https://github.com/Jaros-777/slotify-frontend  
- Backend repo - https://github.com/Jaros-777/slotify-backend

Each repo contains detailed instructions on installation, environment variables, and running locally.

---

### 💡 Notes
- This project is a portfolio and educational project, not intended for production.
- Designed to showcase modern web development practices and full-stack architecture.

---

### 👤 Author
Filip Jarocki - [GitHub profile](https://github.com/Jaros-777)

---

### 🖥️ Other repos
Frontend repo - https://github.com/Jaros-777/slotify-frontend  
Backend repo - https://github.com/Jaros-777/slotify-backend

## ⚖ License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.

