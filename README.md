# Wallet Application

A full-stack wallet application that allows users to manage their finances, including signing up, signing in, viewing their account balance, and transferring money between accounts.

## Features

- **User Authentication:** Secure sign up and sign in functionalities.
- **Account Balance:** View the current balance of your account.
- **Money Transfers:** Transfer money between users seamlessly.
- **User Search:** Search for other users on the platform.

## Getting Started

Follow the steps below to set up and run the Wallet Application on your local machine.

### Prerequisites

Ensure you have the following installed:

- **Node.js:** [Download and install Node.js](https://nodejs.org/)
- **MongoDB:** [Download and install MongoDB](https://www.mongodb.com/try/download/community)

   ### Installation

   **Clone the Repository:**

   Clone the project from GitHub to your local machine.
  
   ```bash
   git clone https://github.com/ashishranjan9585/Wallet_Application.git
   ```

   ### Set Up Frontend Configuration:

  In the `frontend` directory, create a `config.js` file with the following content:
   
```javascript
export const SIGNUP_URL = "<backend_URL>/api/user/signup";
export const SIGNIN_URL = "<backend_URL>/api/user/signin";
export const USERS_URL = "<backend_URL>/api/user/bulk?filter=";
export const MONEY_TRANSFER_URL = "<backend_URL>/api/account/transfer";
export const BALANCE_URL = "<backend_URL>/api/account/balance";
```

### Install Dependencies

 Navigate to the project directory and install the required dependencies

 Frontend:
```bash
cd frontend
npm install
```

 Backend:
```bash
cd backend
npm install
```

## Running the Application

# Start the Backend Server:

Run the backend server with the following command:

```bash
cd backend
node index.js
```

# Start the Frontend Development Server:

Run the frontend development server:

```bash
cd frontend
npm run dev
```

## Technology Stack

### Frontend

- **React:** Library for building user interfaces.
- **React DOM:** For DOM manipulation in React.
- **React Router DOM:** Declarative routing for React applications.
- **Axios:** Promise-based HTTP client for the browser and Node.js.
- **Tailwind CSS:** A utility-first CSS framework for rapid UI development.

### Backend

- **Node.js:** JavaScript runtime for server-side development.
- **Express:** Web framework for building REST APIs.
- **MongoDB:** NoSQL database for storing user and account data.
- **Mongoose:** ODM (Object Data Modeling) library for MongoDB and Node.js.
- **JWT (JSON Web Tokens):** For secure user authentication and authorization.
- **Zod:** Schema declaration and validation library.
- **Body-Parser:** Middleware for parsing incoming request bodies.
- **CORS:** Middleware to enable Cross-Origin Resource Sharing.

## API Endpoints

### User Endpoints
```bash
- POST /api/user/signup: Register a new user.
- POST /api/user/signin: Log in an existing user.
- GET /api/user/bulk:    Retrieve a list of users with optional filtering.
```
### Account Endpoints
```
- GET /api/account/balance:   Retrieve the current balance of the user's account.
- POST /api/account/transfer: Transfer money to another user.
```
