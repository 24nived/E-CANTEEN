# E-Canteen

**E-Canteen** is a canteen management system designed to streamline operations for both in-house services and online ordering. It simplifies order management, inventory tracking, and customer interaction, providing an efficient and user-friendly experience.

---

## Features

- **Order Management**:
  - Online ordering for customers.
  - Real-time order tracking for canteen staff.

- **Inventory Management**:
  - Automatic inventory updates with each order.
  - Alerts for low-stock items.

- **Menu Management**:
  - Dynamic menu updates by the admin.
  - Pricing and availability control.

- **Customer Experience**:
  - Intuitive interface for browsing and ordering.
  - Payment integration for secure transactions.

- **Reports**:
  - Sales reports for daily, weekly, and monthly performance.

---

## Technologies Used

- **Frontend**:
  - HTML, CSS, JavaScript
  - Frameworks/Libraries: React.js (optional if SPA)

- **Backend**:
  - Node.js with Express.js

- **Database**:
  - MongoDB

- **Deployment**:
  - Hosted on AWS EC2 or any cloud platform.

---

@echo off
REM E-Canteen Installation Script

echo Starting E-Canteen installation...

REM Step 1: Clone the Repository
echo Cloning the repository...
git clone https://github.com/yourusername/E-Canteen.git
cd E-Canteen || exit /b

REM Step 2: Install Dependencies
echo Installing dependencies...
npm install

REM Step 3: Configure Environment Variables
echo Setting up environment variables...
echo DB_URI=your-mongodb-connection-string> .env
echo PORT=3000>> .env

echo .env file created with default values. Update it with your MongoDB connection string if needed.

REM Step 4: Start the Server
echo Starting the server...
npm start

echo E-Canteen installation and setup complete!
echo Visit http://localhost:3000 to access the application.
pause
