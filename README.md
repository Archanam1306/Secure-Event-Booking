# Secure Event Booking

A backend system for handling event bookings, including seat reservations, user authentication, and event capacity management. This system features secure authentication, CRUD operations, and error handling for smooth event management.

## Features

- **User Authentication**: Secure authentication using JWT or other advanced methods.
- **Event Booking**: Users can reserve seats for events, with seat availability and capacity management.
- **CRUD Operations**: Supports basic Create, Read, Update, and Delete operations for events, users, and bookings.
- **Error Handling & Validation**: Proper data validation and error handling to ensure a reliable system.
- **Database Integration**: Works with databases such as MongoDB or PostgreSQL for efficient data storage.

## Technologies Used

- **Node.js** (Backend)
- **Express.js** (Framework)
- **MongoDB / PostgreSQL** (Database)
- **JWT** (Authentication)
- **Mongoose** / **Sequelize** (ORM, depending on DB used)
- **Validation**: Express-validator for input validation
- **Error Handling**: Custom error handling middleware

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/Archanam1306/Secure-Event-Booking.git
    ```

2. Navigate to the project directory:
    ```bash
    cd Secure-Event-Booking
    ```

3. Install dependencies:
    ```bash
    npm install
    ```

4. Set up environment variables. Create a `.env` file in the root directory with the following:

    ```bash
    DB_CONNECTION_STRING=your_database_connection_string
    JWT_SECRET=your_jwt_secret_key
    ```

5. Start the development server:
    ```bash
    npm start
    ```

## API Endpoints

- **Authentication**
  - `POST /api/auth/register` - Register a new user
  - `POST /api/auth/login` - Login with credentials

- **Events**
  - `GET /api/events` - Get all events
  - `POST /api/events` - Create a new event (Admin only)
  - `PUT /api/events/:id` - Update an event (Admin only)
  - `DELETE /api/events/:id` - Delete an event (Admin only)

- **Bookings**
  - `POST /api/bookings` - Book seats for an event
  - `GET /api/bookings` - Get all bookings for a user


