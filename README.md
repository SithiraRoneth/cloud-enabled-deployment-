# ☁️ Cloud Enabled Deployment In Action with GCP

This repository demonstrates a **cloud-enabled microservices architecture** deployed on **Google Cloud Platform (GCP)**.  


## 📦 Project Structure

- `course-service` → Spring Boot + MySQL (Cloud SQL)  
- `student-service` → Spring Boot + MongoDB  
- `media-service` → Spring Boot + Local file storage (can be extended to Cloud Storage)  
- `frontend-app` → React + TypeScript  

---

## 🔧 Backend Services

### 1. course-service
- **Entity:** `Course(id, name, duration)`
- **Endpoints:**
  - `GET /courses`
  - `GET /courses/{id}`
  - `POST /courses`
  - `DELETE /courses/{id}`
- **Port:** `8081`  
- **Database:** Google Cloud SQL (MySQL)  

**Config Example (`application-gcp.properties`):**
```properties
spring.datasource.url=jdbc:mysql://<CLOUD_SQL_IP>:3306/course_db
spring.datasource.username=<USERNAME>
spring.datasource.password=<PASSWORD>

```

## 🔧 How to Use This Repository ### 

- Clone the repository bash git
  ``` clone https://github.com/SithiraRoneth/cloud-enabled-deployment-.git ```
- cd cloud-gcp-deployment

---

## 📽️ Configured Video
- watch here : https://drive.google.com/file/d/1Z8vIKPWhjkIzzBOeMvkzp7sb54GAncPs/view?usp=drive_link

---
