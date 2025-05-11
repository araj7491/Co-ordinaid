# Co-Ordinaid: Volunteer Management System

A full-stack Java web application designed to streamline the management of volunteers, assignments, timesheets, skills, and nonprofit organizations (NGOs). Developed using **Spring Boot**, **JDBC**, **Thymeleaf**, and **MySQL**, this system empowers NGOs with a centralized platform to manage their volunteers efficiently.

---

## 📌 Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Technology Stack](#technology-stack)
- [System Flow & ER Diagram](#system-flow--er-diagram)
- [Project Structure](#project-structure)
- [How to Run (Eclipse Setup)](#how-to-run-eclipse-setup)
- [Live Demonstration](#live-demonstration)
- [Team Members](#team-members)
- [References](#references)

---

<a name="introduction"></a>
## ✅ Introduction

Co-Ordinaid is developed as part of an Advanced Java Programming academic project for managing end-to-end volunteer operations. It provides intuitive modules for:
- Registering NGOs and volunteers
- Assigning tasks
- Logging work hours (timesheets)
- Managing volunteer skills

---

<a name="features"></a>
## 💡 Features

- Volunteer and NGO registration
- Assignments linked to both
- Timesheet logging and editing
- Skill management for volunteers
- Role-based form validation
- MySQL database integration
- Clean, mobile-responsive UI

---

<a name="technology-stack"></a>
## 🧰 Technology Stack

| Layer        | Technology Used                          |
|--------------|-------------------------------------------|
| Frontend     | HTML, CSS, Bootstrap 4, Thymeleaf         |
| Backend      | Java, Spring Boot, Spring MVC             |
| Data Access  | Spring JDBC (JdbcTemplate)                |
| Database     | MySQL                                     |
| IDE          | Eclipse IDE                               |
| Build Tool   | Maven                                     |

---

<a name="system-flow--er-diagram"></a>
## 🧭 System Flow & ER Diagram

### 📊 Flowchart:
[Flowchart](demo/live.mp4)

### 📐 ER Diagram:
[ER Diagram](demo/er-diagram.png)
- **Many-to-Many**: Volunteer ⬌ Nonprofit
- **One-to-Many**: Nonprofit ⬌ Assignment ⬌ Timesheet
- **One-to-Many**: Volunteer ⬌ Skills


---

<a name="project-structure"></a>
## 📁 Project Structure

```
Volunteer-Management-System/
│
├── src/
│   ├── main/
│   │   ├── java/org/vms/volunteer/         # Java packages: controller, dao, service, dto, mapper
│   │   ├── resources/
│   │   │   ├── static/                     # Static resources like CSS, images
│   │   │   ├── templates/                  # Thymeleaf HTML pages
│   │   │   ├── application.properties
│   │   │   ├── schema.sql, data.sql       # DB setup scripts
│   └── test/                              # Unit tests
├── pom.xml                                # Maven config
└── README.md
```

---

<a name="how-to-run-eclipse-setup"></a>
## 🛠️ How to Run (Eclipse Setup)

### ⚙️ Prerequisites:
- JDK 11+
- Eclipse IDE with Maven support
- MySQL Server running (port 3306)
- MySQL DB name: `volunteer_db`

### 📦 Steps:

1. **Clone or unzip the project** into your workspace.
2. Open Eclipse → `File > Import > Existing Maven Project` → Select the unzipped folder.
3. In MySQL Workbench or CLI, run:
   ```sql
   CREATE DATABASE volunteer_db;
   USE volunteer_db;
   SOURCE schema.sql;
   SOURCE data.sql;
   ```
4. Update `application.properties` (if needed):
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/volunteer_db
   spring.datasource.username=root
   spring.datasource.password=your_password
   ```
5. Run the project:
   - Right-click `VolunteerManagementSystemApplication.java` > `Run As > Java Application`
6. Visit:  
   `http://localhost:8080/` in your browser

---

<a name="live-demonstration"></a>
## 📸 Live Demonstration

[Video Demonstration](demo/live.mp4)


---

<a name="team-members"></a>
## 👨‍💻 Team Members

| Name            | Role                 | 
|-----------------|----------------------|
| Ankit Raj       | Team Lead & Docs     | 
| Nishu Kaushik   | Frontend Developer   | 
| Shweta Verma    | Backend Developer    |
| Aditi Yadav     | Database Management  | 

---

<a name="references"></a>
## 🔗 References

- [Spring Boot Docs](https://spring.io/projects/spring-boot)
- [Thymeleaf Docs](https://www.thymeleaf.org/)
- [MySQL Docs](https://dev.mysql.com/doc/)
- [Baeldung Java Guides](https://www.baeldung.com/)
- [W3Schools](https://www.w3schools.com/)
