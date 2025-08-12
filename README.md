
# Co-ordinaid

**Co-ordinaid** is a web-based platform designed to streamline the registration, organization, and management of volunteers for NGOs or events. It helps administrators track volunteer details, activities, and schedules while providing volunteers a platform to register, view tasks, and update their availability. Built using **Spring Boot** with **Thymeleaf** for the frontend and **MySQL** for the database, this project eliminates inefficiencies caused by manual or disconnected systems.

## ▶ Project Summary

**Objective:**  
To build a digital, cost-effective, and user-friendly solution for NGOs and event organizers to manage volunteers, track assignments, monitor timesheets, and utilize skill-based matching.

**Domain:** Web Application Development for Nonprofit Organizations  
**Technologies Used:**
- **Frontend:** HTML, CSS, JavaScript, Thymeleaf
- **Backend:** Java (Spring Boot, Controllers)
- **Database:** MySQL
- **Authentication:** Spring Security

## ➤ Features

- **Administrator login** with Spring Security for secure authentication
- **Volunteer registration** and task management
- **Real-time updates** on volunteer availability and assignments
- **Easy onboarding** and registration process for volunteers
- **Comprehensive tracking** of volunteer hours, skills, and assignments
- **User-friendly interface** ensuring quick adoption by administrators and volunteers

## ▪ Project Structure

```
Co-ordinaid/
│
├── src/                       # Spring Boot controllers and business logic
│   ├── controller/
│   │   ├── AdminController.java
│   │   ├── VolunteerController.java
│   └── model/
│       ├── Volunteer.java
│       └── Assignment.java
│
├── resources/                  # Thymeleaf templates and static resources
│   ├── templates/
│   │   ├── volunteer_dashboard.html
│   │   ├── admin_dashboard.html
│   ├── application.properties
│
├── Database/                  # MySQL schema
│   └── coordinaid.sql
│
└── README.md                  # This file
```

## → Setup Instructions

1. **Clone the repository:**
   ```bash
   git clone https://github.com/araj7491/Co-ordinaid.git
   ```

2. **Open in your Java IDE** (e.g., IntelliJ IDEA or Eclipse).

3. **Configure the MySQL database**:
   - Import the `coordinaid.sql` file into your MySQL server to create the required tables.
   - Update the `application.properties` file with your MySQL credentials:
     ```properties
     spring.datasource.url=jdbc:mysql://localhost:3306/coordinaid
     spring.datasource.username=root
     spring.datasource.password=your_password
     ```

4. **Run the Spring Boot application**.

5. **Access the application** by navigating to `http://localhost:8080/`.

## ◆ Roles

- **Administrator:** Can log in, manage volunteer tasks, and track volunteer details and availability.
- **Volunteer:** Can register, view available tasks, and update availability.


## ► Author

- **Ankit Raj**  


## ▸ References

- [Spring Boot Documentation](https://spring.io/projects/spring-boot)
- [Thymeleaf Documentation](https://www.thymeleaf.org)
- [MySQL Documentation](https://dev.mysql.com/doc/)
- [W3Schools](https://www.w3schools.com/)
- [Baeldung Spring Guides](https://www.baeldung.com/)


