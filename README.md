# Expense Tracker

This is a full-stack expense tracker application that allows users to track their income and expenses efficiently. The application features user authentication, real-time analytics, and a responsive design.

## Table of Contents
- [Tech Stack](#tech-stack)
- [Features](#features)
- [Installation and Setup](#installation-and-setup)
- [Environment Variables](#environment-variables)
- [Project Structure](#project-structure)
- [Authentication](#authentication)
- [API Endpoints](#api-endpoints)
- [Styling](#styling)
- [Deployment](#deployment)
- [License](#license)
- [Contributing](#contributing)
- [Contact](#contact)

## Tech Stack
### Frontend:
- React.js: JavaScript library for building the user interface.
- React Router: Handles client-side routing.
- Ant Design: UI framework for consistent and modern design.
- Axios: For API requests.
- Redux: State management.

### Backend:
- Node.js & Express.js: Server-side framework for handling API requests.
- MongoDB & Mongoose: NoSQL database for storing transactions and user data.
- JSON Web Token (JWT): Authentication system for user login.

## Features
- User authentication using JWT.
- Add, edit, and delete transactions.
- Categorize transactions into income and expenses.
- Real-time analytics for financial insights.
- Responsive design for desktop and mobile use.
- Toast notifications for better user experience.

## Installation and Setup
### Clone the Repository
```bash
git clone https://github.com/your-username/expense-tracker.git
```

### Navigate to the Project Directory
```bash
cd expense-tracker
```

### Install Backend Dependencies
```bash
npm install
```

### Start the Backend Server
```bash
npm start
```

### Navigate to the Client Directory
```bash
cd client
```

### Install Frontend Dependencies
```bash
npm install
```

### Start the Frontend Server
```bash
npm start
```
The application will run at `http://localhost:3000`.

## Environment Variables
Create a `.env` file in the root directory and add the following:
```
MONGO_URI=your-mongodb-connection-string
JWT_SECRET=your-secret-key
PORT=5000
REACT_APP_API_URL=http://localhost:5000
```

## Project Structure
```
expense-tracker/
│── server.js  # Main server file
│── dbConnect.js  # Database connection
│── models/
│   ├── User.js  # User schema
│   ├── Transaction.js  # Transaction schema
│── routes/
│   ├── usersRoute.js  # Authentication API routes
│   ├── transactionsRoute.js  # Transaction API routes
│── client/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── App.js
│   │   ├── index.js
│   │   ├── styles/
│   ├── public/
│   ├── package.json
```

## Authentication
The application uses JSON Web Token (JWT) for user authentication. On successful login, a token is stored in local storage and used for API requests.

## API Endpoints
### User Authentication
- `POST /api/users/register` - Register a new user.
- `POST /api/users/login` - User login.

### Transactions
- `GET /api/transactions` - Get all transactions.
- `POST /api/transactions` - Add a new transaction.
- `PUT /api/transactions/:id` - Edit a transaction.
- `DELETE /api/transactions/:id` - Delete a transaction.

## Styling
The frontend is styled using Ant Design for a professional and modern look. Responsive design ensures a seamless experience across devices.

## Deployment
The frontend can be deployed on Vercel, and the backend can be hosted on a cloud platform like Heroku or Railway.

### Steps to Deploy
1. Push your project to GitHub.
2. Connect your GitHub repository to Vercel for frontend deployment.
3. Deploy the backend using Heroku/Railway.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Contributing
We welcome contributions to this project. If you want to contribute, please follow these steps:
1. Fork the repository.
2. Create a new branch.
3. Make your changes and test thoroughly.
4. Submit a pull request with a description of your changes.

## Contact
- Email: kondasaikrishna13@gmail.com
- GitHub: https://github.com/saikrishna1909

