# JOB-APP

A simple **Spring Boot + JSP** job portal web application.  
Users can browse predefined job postings and create new ones through a clean, responsive interface.

---

## 🚀 Features
- 📋 **View a list of 20 predefined job postings**
- ➕ **Add new job postings** via a form
- 📱 **Responsive design** with Bootstrap 5.3
- 💾 **In-memory storage** — no database setup required

---

## 📂 Project Structure

| File / Folder         | Description |
|-----------------------|-------------|
| `JobAppApplication.java` | Entry point for Spring Boot, starts the server |
| `JobController.java`     | Handles routes: `/`, `/home`, `/addjob`, `/viewalljobs`, `/handleForm` |
| `JobService.java`        | Business logic layer between controller and repository |
| `JobRepo.java`           | In-memory repository with methods to return/add job posts. Preloaded with 20 posts |
| `JobPost.java`           | Model for a job post (`postProfile`, `postDesc`, `reqExperience`, `postTechStack`) |
| `views/*.jsp`            | JSP templates for home, job listing, job form, and success page |
| `static/css/*.css`       | Stylesheets for the app |

---

## 🛠 Tech Stack
- **Java**: 17+
- **Spring Boot**: 3.x
- **JSP + JSTL** for templating
- **Bootstrap** 5.3.2 for styling
- **Maven** for build and dependency management
- **Data Storage**: In-memory `ArrayList` (no database)

---

## ▶ How to Run

### Prerequisites
- Java **17+**
- Maven **3.8+**

### Steps
```bash
# 1. Clone the repository
git clone <repo-url>
cd JOB-APP

# 2. Run with Maven
./mvnw spring-boot:run
````

Once running, open **[http://localhost:8080](http://localhost:8080)** in your browser.

---

## 🌐 Endpoints Overview

| Method | URL            | Description            |
| ------ | -------------- | ---------------------- |
| GET    | `/`            | Home page              |
| GET    | `/home`        | Home page (alias)      |
| GET    | `/addjob`      | Job creation form      |
| POST   | `/handleForm`  | Processes new job post |
| GET    | `/viewalljobs` | Lists all job posts    |

---

## 🔮 Future Improvements

* Add persistent database (e.g., MySQL or PostgreSQL)
* Implement search and filtering
* Add user authentication for posting jobs
* Create REST API version

---

## 📸 Screenshots

<img width="1914" height="944" alt="image" src="https://github.com/user-attachments/assets/ed02ae61-df92-4466-9c6f-d834716ce654" />
<img width="1911" height="936" alt="image" src="https://github.com/user-attachments/assets/76e30971-088f-4fd3-8399-8ac40287f839" />
<img width="1919" height="936" alt="image" src="https://github.com/user-attachments/assets/daab6322-5d17-4f0f-a682-086c072d09e4" />

---

## 👨‍💻 Author

**Mohd Saqib**
[GitHub](https://github.com/imsaqib04) | [LinkedIn](https://www.linkedin.com/in/imsaqib04) 

---

## 📜 License

This project is licensed under the **MIT License** — you are free to use, modify, and distribute it with attribution.

---
