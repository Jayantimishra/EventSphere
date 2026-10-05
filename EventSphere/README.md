# EventSphere — Full-Stack Event Booking Platform

EventSphere is a full-stack event booking platform built with the MERN stack. It allows users to explore events, submit booking requests, track booking status, and manage their reservations. Administrators can manage events, review booking requests, monitor payments, and track platform activity through an admin dashboard.

## Features

### Authentication

- User registration and login
- JWT-based authentication
- Password hashing with bcrypt
- Email OTP verification for account activation and booking confirmation

### User Features

- Browse available events
- View event details
- Submit booking requests
- Track booking status
- Cancel bookings
- Access a personal dashboard

### Admin Features

- Create, update, and delete events
- Manage free and paid events
- Review and process booking requests
- Confirm or reject bookings
- Track payment status
- Monitor booking activity and revenue

### Booking Management

- OTP verification before booking
- Pending, confirmed, and rejected booking states
- Seat availability validation
- Overbooking prevention
- Payment-status tracking

### Notifications

- Automated email notifications using Nodemailer

### Frontend

- Responsive React interface
- Tailwind CSS styling
- Interactive UI components

## Technology Stack

| Category | Technologies |
|---|---|
| Frontend | React, Tailwind CSS |
| Backend | Node.js, Express.js |
| Database | MongoDB |
| Authentication | JWT, bcrypt, OTP |
| Email | Nodemailer |
| Development | Git, npm |

## Project Structure

```text
EventSphere/
├── client/
│   ├── src/
│   └── ...
├── server/
│   ├── ...
│   └── ...
└── README.md
```

## Environment Variables

Create a `.env` file inside the `server` directory:

```env
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
EMAIL_USER=your_email_address
EMAIL_PASS=your_email_app_password
PORT=5000
```

> **Note:** Never commit `.env` files or credentials to GitHub.

## Installation

### 1. Clone the Repository

```bash
git clone <repository-url>
cd EventSphere
```

### 2. Install Dependencies

From the project root:

```bash
npm install
npm run install:all
```

Or install dependencies separately.

#### Backend

```bash
cd server
npm install --legacy-peer-deps
```

#### Frontend

```bash
cd ../client
npm install
```

## Running the Application

### Start the Backend

```bash
cd server
npm run dev
```

The backend runs on:

```text
http://localhost:5000
```

### Start the Frontend

Open a new terminal:

```bash
cd client
npm run dev
```

The frontend will be available at the local development URL provided by Vite.

## Key Concepts Demonstrated

- MERN stack application architecture
- REST API development
- JWT authentication and authorization
- Role-based access control
- MongoDB data modelling
- Booking workflow management
- OTP-based verification
- Frontend-backend integration
- Email notification workflows
- Administrative dashboard development

## Future Improvements

- Online payment gateway integration
- Event search and filtering
- Automated booking confirmation
- Cloud-based image storage
- Production deployment and monitoring