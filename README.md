# classconnect
# 🎓 ClassConnect - Course Registration System

## 📘 Overview
**ClassConnect** is a full-stack web-based application designed to simplify the process of course registration and management for students.  
It allows students to browse available courses, enroll in their preferred ones, and view their enrollment details through a clean and intuitive interface.

---

## 🧩 Features
- 🧑‍🎓 **Student Course Registration** — Students can easily register for available courses.
- 📚 **View Available Courses** — Lists all active courses from the backend database.
- 📝 **Enrollment Management** — Students can see their registered courses.
- ⚙️ **Spring Boot REST APIs** — Backend powered by RESTful endpoints.
- 💾 **MySQL Integration** — All course and enrollment data are stored in a MySQL database.
- 🌐 **CORS Enabled** — Secure communication between frontend and backend.

---

## 🛠️ Tech Stack
### **Frontend**
- HTML5  
- CSS3  
- JavaScript (Vanilla)

### **Backend**
- Java 17+  
- Spring Boot (RESTful APIs)
- Spring Data JPA
- Maven Build Tool

### **Database**
- MySQL

---

## 📁 Project Structure

```
classconnect-main/
│
├── Class_connect_Backendcode/
│   └── Course-Registration-System/
│       ├── src/
│       │   ├── main/java/com/example/Course/Registration/System/
│       │   │   ├── controller/ → Contains REST API controllers
│       │   │   ├── model/ → Entity classes for Course & CourseRegistry
│       │   │   ├── repository/ → JPA repositories
│       │   │   └── services/ → Business logic
│       │   └── resources/
│       │       └── application.properties → Database & server configuration
│       ├── pom.xml → Maven dependencies
│
└── Frond_end_code/
    ├── index.html → Home page
    ├── availcourses.html → Available courses listing
    ├── enrolled.html → Enrolled courses page
    ├── register.html → Course registration form
    └── myscript.js → Frontend logic & API calls
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone or Extract the Repository
```bash
git clone https://github.com/yourusername/classconnect.git
cd classconnect-main
```

### 2️⃣ Setup the Backend (Spring Boot)
- Open the project in **IntelliJ IDEA** or **Eclipse**.
- Update your MySQL credentials in  
  `Class_connect_Backendcode/Course-Registration-System/src/main/resources/application.properties`
  ```properties
  spring.datasource.url=jdbc:mysql://localhost:3306/classconnect
  spring.datasource.username=root
  spring.datasource.password=yourpassword
  spring.jpa.hibernate.ddl-auto=update
  ```
- Build and run:
  ```bash
  mvn spring-boot:run
  ```
- Backend will run at:  
  👉 `http://localhost:8080`

### 3️⃣ Setup the Frontend
- Open the folder:  
  `classconnect-main/Frond_end_code/`
- Open `index.html` in your browser.
- Ensure the backend (`localhost:8080`) is running to allow API calls.

---

## 🔗 API Endpoints
| HTTP Method | Endpoint | Description |
|--------------|-----------|-------------|
| GET | `/courses` | Get list of all available courses |
| POST | `/courses/register` | Register a new course |
| GET | `/enrollments` | Get enrolled courses for a student |

---

## 🧑‍💻 Author
**Developed by:** Surendhar  
**Role:** Junior Full Stack Web Developer  
**Technologies:** Java, Spring Boot, MySQL, HTML, CSS, JavaScript  

---

## 📜 License
This project is open-source and available under the [MIT License](LICENSE).

---

## 🖼️ Screenshots (Optional)
_Add screenshots of your UI here for better presentation._

---

## 💡 Future Enhancements
- Add user authentication (login/signup).  
- Add admin dashboard for course management.  
- Enhance UI with React or Angular.  
- Integrate email notifications for enrollments.
