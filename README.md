# CapX

CapX is a comprehensive portfolio tracking application designed to help users manage and monitor their investments effectively. This repository contains both the backend and frontend components necessary to run the application locally.

## Table of Contents

- [Features](#features)
- [Prerequisites](#prerequisites)
- [Steps to Run the Project Locally](#steps-to-run-the-project-locally)
- [Assumptions and Limitations](#assumptions-and-limitations)
- [Links](#links)

## Features

- **Portfolio Management:** Track and manage various investments in one place.
- **Real-time Data:** Receive up-to-date information on market trends and asset performance.
- **User Authentication:** Secure login and personalized user experience.
- **Responsive Design:** Accessible on both desktop and mobile devices.

## Prerequisites

Before running the project, ensure you have the following installed on your system:

- **Node.js** (version 14.x or higher)
- **npm** (version 6.x or higher)
- **Java Development Kit (JDK)** (version 11 or higher)
- **Docker** (optional, for containerized deployment)
- **PostgreSQL** (version 12 or higher)

## Steps to Run the Project Locally

1. **Clone the repository:**
   ```bash
   git clone https://github.com/shakyagithub/CapX.git
   cd CapX
   ```

2. **Set up the Backend:**
   - Navigate to the backend directory:
     ```bash
     cd portfolio-tracker-backend
     ```
   - Install backend dependencies:
     ```bash
     ./mvnw clean install
     ```
   - Configure the database:
     - Ensure PostgreSQL is running.
     - Create a database named `capx_db`.
     - Update the `application.properties` file with your database credentials.
   - Run the backend server:
     ```bash
     ./mvnw spring-boot:run
     ```

3. **Set up the Frontend:**
   - Open a new terminal and navigate to the frontend directory:
     ```bash
     cd ../portfolio-tracker-frontend
     ```
   - Install frontend dependencies:
     ```bash
     npm install
     ```
   - Start the frontend development server:
     ```bash
     npm start
     ```

4. **Access the Application:**
   - Open your browser and navigate to:
     ```
     http://localhost:3000
     ```

## Assumptions and Limitations

### Assumptions

- Users have the necessary permissions to install and run applications on their systems.
- The local environment has sufficient resources to run both backend and frontend servers simultaneously.

### Limitations

- The application currently supports only PostgreSQL as the database.
- Real-time data features may require additional API keys or subscriptions to third-party services.

## Links

- **Deployed Application:** [Currently not available]
- **Live API Documentation:** [Currently not available]

---
Feel free to report issues or contribute to the project by creating a pull request or opening an issue in the repository.
