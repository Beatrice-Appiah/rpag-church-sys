# RPAG Church Management System

A web-based Church Management System designed for **Resurrection Power Assemblies of God**. This system digitizes administrative tasks, allowing the church to manage membership records, track service attendance, and record financial contributions effectively.

This project was developed as part of the **Field Trip and Report Writing** course for the BSc. Computer Science program at **Ghana Communication Technology University (GCTU)**.

## 🚀 Key Features

### 🔐 Security & Access Control
* **Role-Based Authentication:** Secure Login/Signup system restricted to church staff.
* **Staff Roles:** Supports distinct roles for "Pastors" (Full Access) and "Executives" (Administrative Access).

### 👥 Church Management
* **Membership Database:** Register new members and view a digital directory of the congregation.
* **Attendance Tracking:** Record and monitor headcount for Sunday and Mid-week services.
* **Treasury Dashboard:** Record tithes/offerings (Cash, Mobile Money) and view automated total income reports.

## 🛠️ Technology Stack

* **Frontend:** React.js (Hooks, Functional Components)
* **Backend:** Node.js, Express.js (REST API)
* **Database:** MySQL (Relational Data Management)
* **Styling:** CSS3 (Custom Professional UI)

## ⚙️ Prerequisites

Before running this project, ensure you have the following installed:

* [Node.js](https://nodejs.org/) (v14 or higher)
* [MySQL Server](https://dev.mysql.com/downloads/installer/)

## 📦 Installation & Setup

### 1. Database Setup
1.  Open your MySQL tool (e.g., PHPMyAdmin, Workbench, or Command Line).
2.  Create a new database named `rpag_db`.
3.  **Crucial:** Import the `database.sql` file provided in this repository. This will create the required tables:
    * `users` (for login credentials)
    * `members` (for church members)
    * `attendance` (for service records)
    * `donations` (for financial records)

### 2. Backend Setup (Server)
Navigate to the server directory and install dependencies:
```bash
cd server
npm install
```

## Create a .env file in the server folder with your database credentials:

DB_HOST=localhost
DB_USER=root
DB_PASSWORD=your_password
DB_NAME=rpag_db
PORT=5000

## Start the backend server:
```bash
node server.js
```
The server will run on http://localhost:5000

### 3. Frontend Setup (Client)
Open a new terminal, navigate to the client directory, and install dependencies:

```bash
cd client
npm install
```

## Start the React application:
```bash
npm start
```

* The application will open automatically at http://localhost:3000

## How to Use
- Register Staff: On the initial Login screen, click "Register Here" to create a staff account (e.g., Select "Pastor" role).

- Login: Use your new credentials to access the Dashboard.

- Manage: Use the navigation bar to switch between Membership, Attendance, and Giving modules.

## 📸 Screenshots
![Attendnace Page](./screenshots/Attendance-1.png)
![Attendnace Page-2](./screenshots/Attendance-2.png)

![Giving Page](./screenshots/giving-1.png)
![Giving Page-2](./screenshots/giving-2.png)

![Memebers Page](./screenshots/members-1.png)
![Memebers Page](./screenshots/members-2.png)


### 👤 Author
* Beatrice Naa-Meryea Appiah
* Institution: Ghana Communication Technology University
* Level: 300 (Computer Science Top-up)