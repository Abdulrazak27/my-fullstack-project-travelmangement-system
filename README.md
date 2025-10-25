# Travel Management System – Full Stack Deployment

## Project Overview
This project is a full-stack Travel Management System developed for the university healthcare portal. It allows users to register, login, and access a dashboard showing travel modules including Destinations, Bookings, and Payments.  

**Key Features:**
- User Signup and Login with authentication
- Dashboard with Destinations, Bookings, and Payments
- Integration of Frontend and Backend
- Multi-container deployment using Docker Compose
- Data persistence using MySQL

---

## Technology Stack

| Layer       | Technology                 |
|------------|----------------------------|
| Backend    | Java Spring Boot           |
| Frontend   | React + Vite               |
| Database   | MySQL                     |
| Deployment | Docker Compose            |

---

## Folder Structure



my-fullstack-project-travelmangement-system/
│
├── carrental-backend/
│ ├── src/
│ ├── pom.xml
│ └── application.properties
│
├── carrental-frontend/
│ ├── src/
│ ├── package.json
│ └── vite.config.js
│
└── README.md


---

## Local Setup Instructions

### Backend
1. Navigate to the backend folder:
```bash
cd carrental-backend


Update MySQL connection in application.properties:

spring.datasource.url=jdbc:mysql://localhost:3306/travel_db
spring.datasource.username=root
spring.datasource.password=yourpassword
server.port=8081


Run the backend:

mvn spring-boot:run


Test API endpoints:

Signup → http://localhost:8081/auth/signup

Login → http://localhost:8081/auth/login

Frontend

Navigate to the frontend folder:

cd carrental-frontend


Install dependencies:

npm install


Run development server:

npm run dev


Open in browser:

http://localhost:5173

Docker Compose Deployment

Run the full stack using Docker Compose to start backend, frontend, and MySQL together:

docker-compose up --build


Ports:

MySQL → 3306

Backend → 8081

Frontend → 5173

Verify:

Signup/Login works

Dashboard displays Destinations, Bookings, Payments

Data persists in MySQL

CI/CD Best Practices Implemented

Separate Dockerfiles for frontend and backend

Environment variables used for database credentials

Local testing before deployment

Single GitHub repository for version control

Multi-container deployment via Docker Compose



Authors

Abdul Razak – University Student, Full-Stack Developer
Email: 2300032428@klnuniversity.in

GitHub Repository

https://github.com/Abdulrazak27/my-fullstack-project-travelmangement-system

Notes

Successfully cloned, configured, and executed full-stack Travel Management System locally.

Deployed using Docker Compose for multi-container setup.

All modules verified and working.

