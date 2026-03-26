# Pawsome - Pet Care & Adoption Platform

A full-stack microservices-based application built with React, Node.js, Express, and MongoDB.

## About the Project
This system allows users to browse different types of pets (dogs, cats, birds, etc.), view their details (age, breed, health status, price), and either adopt or purchase them. It provides a convenient and centralized way to manage pet listings and connect pet seekers with providers.

## Architecture
This application strictly follows a microservices architecture:

1. **Frontend (Port 3000):** React (Vite) Single Page Application featuring a premium glassmorphism UI.
2. **API Gateway (Port 5000):** Routes incoming frontend requests to correct backend services.
3. **User Service (Port 5001):** Handles auth (JWT) and user profiles.
4. **Pet Service (Port 5002):** Manages pet listings and adoptions.
5. **Booking Service (Port 5003):** Handles vet appointment bookings.
6. **Notification Service (Port 5004):** Performs logging and notification services (mocking emails).

## Prerequisites
- **Node.js** (v16+)
- **MongoDB** (Running locally on 27017)

## Setup & Running

1. **Start MongoDB:**
   - Ensure your local MongoDB service is running on port 27017.

2. **Install Dependencies and Start Services:**
   You can run the `start_all.ps1` script to boot everything at once or run services individually:

   **API Gateway:**
   ```bash
   cd api-gateway
   npm start
   ```

   **User Service:**
   ```bash
   cd user-service
   npm start
   ```

   **Pet Service:**
   ```bash
   cd pet-service
   npm start
   ```

   **Booking Service:**
   ```bash
   cd booking-service
   npm start
   ```

   **Notification Service:**
   ```bash
   cd notification-service
   npm start
   ```

   **Frontend:**
   ```bash
   cd frontend
   npm run dev
   ```

3. **Access the App:**
   Open your browser to `http://localhost:3000` to interact with the Pawsome platform.
