# Student Attendance Management App

The Student Attendance Management App is a simple application designed to manage and track student attendance. It allows users to add, edit, and delete student information and mark attendance for each student.

## Features

- Add, edit, and delete student information
- Mark attendance for students
- View attendance reports

## Tech Stack ⚒

*   **Backend:** Node.js, Express
*   **Frontend:** HTML, CSS, JavaScript
*   **Database:** MySQL
*   **Packages/Libraries:**
    *   `axios`: For making HTTP requests
    *   `body-parser`: For parsing incoming request bodies
    *   `cors`: For enabling Cross-Origin Resource Sharing
    *   `express`: For creating the web server and handling routing
    *   `mysql2`: For interacting with the MySQL database
    *   `sequelize`: For Object-Relational Mapping (ORM) with the MySQL database

## Installation ⬇️

#### Prerequisites

- Node.js (>= 14.x)
- npm
- MySQL

#### Steps

1. **Clone the repository**:
   ```sh
   git clone https://github.com/SpNain/Student-Attendance-Management-App.git
   cd Student-Attendance-Management-App
   ```

2. **Install dependencies**:
   ```sh
   npm install
   npm install --save-dev nodemon  # OR npm i -D nodemon
   ```

3. **Set up MySQL database and secrets.js**:
   Create a database in MySQL and a `secrets.js` file in the util directory.
   Add the following in `secrets.js`:
   ```
   DB_NAME : 'mysql_database_name',
   DB_USER : 'mysql_database_user_name',
   DB_PASSWORD : 'mysql_database_password'
   ```

4. **Run the application**:
   ```sh
   npm start
   ```

5. **Access the application**:
   Open your browser and navigate to `http://localhost:3000`.

## API Endpoints

### Student Routes

- `GET /student/allstudents`: Get all students
- `POST /student/addStudentData`: Add a new student
- `DELETE /student/delete/:id`: Delete a student by ID
- `PUT /student/edit/:id`: Edit a student by ID

### Attendance Routes

- `GET /attendance/home`: Get the home page for attendance
- `POST /attendance/attendancedatawithdate`: Add attendance data with date
- `GET /attendance/report`: Get attendance report
- `GET /attendance/:date`: Get attendance data for a specific date

