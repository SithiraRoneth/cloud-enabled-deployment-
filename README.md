# ☁️ Cloud Enabled Deployment In Action with GCP

This repository demonstrates a **cloud-enabled microservices architecture** deployed on **Google Cloud Platform (GCP)**.  

It contains **four projects**:

- **course-service** → Spring Boot + MySQL (Cloud SQL)  
- **student-service** → Spring Boot + MongoDB/Firestore  
- **media-service** → Spring Boot + File Storage (Local / Cloud Storage)  
- **frontend-app** → React + TypeScript (Firebase Hosting / Cloud Run)  

---

## 📦 Project Structure

- course-service (Spring Boot + MySQL)
- student-service (Spring Boot + MongoDB)
- media-service (Spring Boot + Local file storage, can be extended to S3/MinIO)
- frontend-app (React + TypeScript)

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


---

## 🔧 How to Use This Repository

### 1. Clone the repository
```bash
git clone (https://github.com/SithiraRoneth/cloud-enabled-deployment-.git)
cd cloud-gcp-deployment

