# MNIST Job Management System
A lightweight system for creating, managing, and monitoring training jobs for the MNIST dataset.  
This project is divided into two subprojects: **frontend** and **backend**.

## ✨ Features
- Create, resume, and delete training jobs.
- Real-time job monitoring with progress updates.
- Track model metrics: accuracy, loss, and training duration.
- View completed jobs and best achieved accuracy.
- Lightweight simulation of training epochs (no heavy computation required).

## 🖥 Frontend

- **Tech stack**:  
  - Next.js
  - TypeScript
  - TanStack Query (React Query)
  - Tailwind CSS 
  - Axios
  - Ant Design

- **Description**:  
  The frontend provides an intuitive interface to create new jobs, view running and completed jobs, and monitor job progress in real-time through polling.

- **Setup**:
  ```bash
  cd frontend
  npm install
  npm run dev
  ```
  Default runs at [http://localhost:3000](http://localhost:3000).

## 🔥 Backend

- **Tech stack**:
  - Node.js
  - Express.js
  - Prisma ORM
  - MySQL
  - Python
  
- **Description**:  
  The backend manages job creation, status updates, progress simulation, and database storage.  
  Jobs are simulated with random accuracy and loss improvements over epochs.

- **Setup**:
  ```bash
  npm install
  npx prisma generate
  npx prisma migrate dev --name init
  npm run dev
  ```
  Default runs at [http://localhost:5000](http://localhost:5000).
