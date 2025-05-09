

# 📝 To-Do Management App

A **To-Do List Management Application** built using **Spring Boot**, enabling users to manage their personal tasks efficiently. The app supports full CRUD operations, user-specific task handling, and integrates form validation and session management using Spring MVC and Spring Security.

---

## 🚀 Features

- ✅ User-specific task management using Spring Security
- 📋 Create, Read, Update, Delete (CRUD) functionalities
- 📅 Set deadlines for tasks with date validation
- 🛡️ Session-based authentication
- ✨ Simple and clean UI with Thymeleaf templates
- 🧪 Form validation with error feedback

---

## 🛠️ Technologies Used

- Java 17+
- Spring Boot
- Spring MVC
- Spring Security
- Jakarta Validation API
- Maven
- H2 (In-memory database for development)

---

## 📂 Project Structure

```
src
├── main
│   ├── java
│   │   └── com.in28minutes.springboot.myfirstwebapp
│   │       ├── todo
│   │       │   ├── TodoController.java
│   │       │   ├── TodoService.java
│   │       │   └── Todo.java
│   │       └── MyFirstWebAppApplication.java
│   └── resources
│       ├── templates
│       │   ├── listTodos.html
│       │   └── todo.html
│       └── application.properties
└── test
```

---

## 🧑‍💻 How It Works

### Authentication

- The app retrieves the currently logged-in user's username using Spring Security:
  ```java
  Authentication authentication = SecurityContextHolder.getContext().getAuthentication();
  String username = authentication.getName();
  ```

### CRUD Operations

- **List To-Dos** – Shows all tasks for the logged-in user
- **Add To-Do** – Create a new task with a deadline
- **Update To-Do** – Modify the description or date
- **Delete To-Do** – Remove a task by ID

---

## 🏃‍♂️ Getting Started

### Prerequisites

- Java 17 or above
- Maven

### Run the App

1. Clone the repo:

   ```bash
   git clone https://github.com/your-username/todo-springboot-app.git
   cd todo-springboot-app
   ```

2. Run using Maven:

   ```bash
   ./mvnw spring-boot:run
   ```

3. Open your browser:

   ```
   http://localhost:8080/list-todos
   ```

---

## 📌 Future Enhancements

- ✅ User login/registration system with password encryption
- 📱 RESTful APIs for frontend integration
- 📊 Task analytics dashboard
- ☁️ Persistent database (MySQL/PostgreSQL)

---

## 🤝 Contributing

Contributions are welcome! Feel free to fork this repo and open a pull request.
