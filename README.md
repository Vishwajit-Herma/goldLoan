# Gold Loan Website
http://gold-loan-mllwrelrl-vishwajit-hermas-projects.vercel.app

## Overview
The Gold Loan Website is a responsive web application that simplifies the process of applying for gold loans. Built using the MERN (MongoDB, Express.js, React.js, Node.js) stack, it allows users to register, log in, and verify their accounts via email before applying for loans.

## Features
- **User Authentication**:
  - Login and Register functionality.
  - Email verification to ensure account security.

- **Loan Application**:
  - Simple form to apply for a gold loan.
  - Loan applications stored securely in the database.

- **Responsive Design**:
  - Optimized for both desktop and mobile devices.

## Technology Stack
- **Frontend**:
  - React.js
  - CSS for styling

- **Backend**:
  - Node.js with Express.js

- **Database**:
  - MongoDB

- **APIs and Libraries**:
  - Nodemailer for email verification.

## Endpoints

### Authentication
1. **Register User**
   - **URL**: `/api/auth/register`
   - **Method**: POST
   - **Description**: Register a new user.
   - **Payload**:
     ```json
     {
       "name": "string",
       "email": "string",
       "password": "string"
     }
     ```

2. **Login**
   - **URL**: `/api/auth/login`
   - **Method**: POST
   - **Description**: Login as a user.
   - **Payload**:
     ```json
     {
       "email": "string",
       "password": "string"
     }
     ```

3. **Email Verification**
   - **URL**: `/api/auth/verify`
   - **Method**: GET
   - **Description**: Verify the user's email address.

### Loan Management
4. **Apply for Loan**
   - **URL**: `/api/loans/apply`
   - **Method**: POST
   - **Description**: Submit a loan application.
   - **Payload**:
     ```json
     {
       "amount": "number",
       "goldWeight": "number",
       "loanDuration": "number"
     }
     ```

## Installation and Setup

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/gold-loan-website.git
   ```

2. **Install Dependencies**:
   - Navigate to the project directory and install backend dependencies:
     ```bash
     cd gold-loan-website/backend
     npm install
     ```
   - Navigate to the frontend directory and install dependencies:
     ```bash
     cd ../frontend
     npm install
     ```

3. **Environment Variables**:
   - Create a `.env` file in the backend directory and add the following:
     ```env
     MONGO_URI=your_mongodb_connection_string
     JWT_SECRET=your_jwt_secret
     EMAIL_SERVICE=your_email_service_provider
     EMAIL_USER=your_email_address
     EMAIL_PASS=your_email_password
     ```

4. **Run the Application**:
   - Start the backend server:
     ```bash
     cd backend
     npm run dev
     ```
   - Start the frontend server:
     ```bash
     cd ../frontend
     npm start
     ```

## Usage
- Open the application in your browser.
- Register and verify your email.
- Log in to your account.
- Apply for a gold loan using the simple application form.

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request for any changes or enhancements.

## Acknowledgments
- Nodemailer for email verification.
- Responsive design inspiration from modern web applications.

