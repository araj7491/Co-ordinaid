
# Co-ordinaid

**Co-ordinaid** is a web-based coordination platform built using Java, JSP, Servlets, JDBC, and MySQL. It is designed to streamline and simplify communication between coordinators and users for event or task management. The application allows coordinators to create and manage tasks, and users to view updates and interact efficiently, eliminating the need for manual messaging.

## 🧠 Project Summary

**Objective:**  
To create a centralized web platform where multiple users can receive real-time updates from a coordinator without relying on traditional messaging systems. This ensures efficiency, reduces time, and minimizes communication errors.

**Domain:** Web Application Development  
**Tools & Technologies:**
- **Frontend:** HTML, CSS, JSP
- **Backend:** Java (Servlets), JDBC
- **Database:** MySQL
- **Server:** Apache Tomcat

## 🚀 Features

- **Coordinator login and authentication**
- **Task and event creation** with descriptions
- **User interface** for accessing the latest tasks and messages
- **Real-time update system** for end-users
- **Centralized message dashboard**
- **Admin module** for coordinator control

## 📁 Project Structure

```
Co-ordinaid/
│
├── src/                       # Java Servlet and Controller logic
│   ├── AddMsg.java
│   ├── Conn.java              # Database connection logic
│   ├── Login.java
│   └── Signup.java
│
├── WebContent/               # Frontend files and JSP pages
│   ├── coordinator.jsp
│   ├── user.jsp
│   ├── login.jsp
│   ├── signup.jsp
│   └── style.css
│
├── Database/                 # MySQL schema
│   └── coordinaid.sql
│
└── README.md                 # This file
```

## ⚙️ Setup Instructions

1. **Clone the repository:**
   ```bash
   git clone https://github.com/araj7491/Co-ordinaid.git
   ```

2. **Open in your Java IDE** (e.g., Eclipse or IntelliJ).

3. **Import the `coordinaid.sql` file** into your MySQL server to create the required database and tables.

4. **Configure your database connection** by updating the `Conn.java` file with your MySQL credentials:
   ```java
   String url = "jdbc:mysql://localhost:3306/coordinaid";
   String user = "root";
   String password = "your_password";
   ```

5. **Run the project** on Apache Tomcat server.

6. **Access the application** by navigating to `http://localhost:8080/Co-ordinaid/`.

## 👤 Roles

- **Coordinator:** Can log in, post updates or tasks, and manage event information.
- **User:** Can view the latest messages and updates from the coordinator.

## 📜 License

This project is open-source and available under the [MIT License](LICENSE).
