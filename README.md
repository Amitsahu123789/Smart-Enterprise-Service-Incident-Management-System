# 🛡️ Smart Enterprise Service & Incident Management System

A full-stack enterprise incident management platform designed to help organizations **report, investigate, prioritize, track, and resolve security and operational incidents** through a centralized system.

The application provides a modern dashboard for incident monitoring, role-based access control, investigation workflows, audit logging, evidence management, notifications, reporting, and analytics.

> **Note:** This project is based on an open-source MIT-licensed project and has been customized for learning, development, and portfolio purposes. The original license and required attribution are retained.

---

## 🚀 Key Features

### 🔐 Authentication & Role-Based Access Control

- User registration and login
- Authentication and authorization
- Role-based access control
- Analyst and administrator roles
- User management dashboard
- First-user administrator setup
- Login using username or email

### 🚨 Incident Management

- Create and report incidents
- Incident categorization
- Severity and priority management
- Risk score tracking
- Incident assignment
- Incident status management
- Complete incident lifecycle tracking

### 🔎 Investigation Workspace

- Incident overview
- Risk assessment
- Investigation checklist
- Investigation timeline
- Comments and collaboration
- Evidence file management
- Incident assignment
- Investigation status tracking

### 📊 Dashboard & Analytics

- Incident statistics
- Open and critical incident monitoring
- Severity breakdown
- Incident lifecycle analytics
- Assigned incident tracking
- Reported incident tracking
- High-risk incident filtering
- Interactive dashboard

### 📄 Reports & Data Export

- Executive incident reports
- PDF report generation
- CSV data export
- Filtered incident exports
- Risk and incident summaries

### 📝 Audit & Notifications

- Incident activity tracking
- Audit logs
- User activity information
- Incident status history
- In-app notifications
- Unread notification counter

### 🤖 AI-Labelled Client Helpers

The application includes client-side intelligent helpers for:

- Incident category suggestions
- Severity suggestions
- Priority recommendations
- Risk score suggestions
- Investigation assistance
- Executive summary generation

> These helpers currently use deterministic client-side rules and do **not** call an external AI/LLM API.

---

# 🏗️ System Architecture

```text
                    ┌─────────────────────┐
                    │      React UI       │
                    │    React 19         │
                    └──────────┬──────────┘
                               │
                               │ REST APIs
                               ▼
                    ┌─────────────────────┐
                    │   Spring Boot API   │
                    │      Backend        │
                    └──────────┬──────────┘
                               │
                ┌──────────────┼──────────────┐
                │              │              │
                ▼              ▼              ▼
          PostgreSQL         Redis        File Storage
          Database           Cache        / Evidence
```

---

# 🛠️ Technology Stack

## Frontend

- React
- JavaScript
- HTML5
- CSS3
- REST API integration
- Responsive UI

## Backend

- Java
- Spring Boot
- Spring MVC
- Spring Data JPA
- Spring Security
- RESTful APIs

## Database & Infrastructure

- PostgreSQL
- Redis
- Docker
- Docker Compose

## Development Tools

- Git
- GitHub
- Maven
- VS Code / IntelliJ IDEA
- Postman

---

# 📂 Project Structure

```text
Smart-Enterprise-Service-Incident-Management-System/
│
├── backend/
│   ├── src/
│   ├── pom.xml
│   └── ...
│
├── frontend/
│   ├── src/
│   ├── package.json
│   └── ...
│
├── .github/
├── Dockerfile
├── docker-compose.yml
├── render.yaml
├── vercel.json
├── LICENSE
├── README.md
├── SECURITY.md
└── CONTRIBUTING.md
```

---

# 🔄 Incident Lifecycle

```text
OPEN
  │
  ▼
INVESTIGATING
  │
  ▼
WAITING FOR EVIDENCE
  │
  ▼
RESOLVED
  │
  ▼
CLOSED
```

The lifecycle allows security/support teams to track an incident from initial reporting through investigation and final resolution.

---

# ⚙️ Installation & Setup

## Prerequisites

Make sure you have the following installed:

- Java JDK 17+
- Maven
- Node.js
- npm
- PostgreSQL
- Redis
- Git

Check your installations:

```bash
java -version
mvn -version
node -v
npm -v
git --version
```

---

# 📥 Clone the Repository

```bash
git clone https://github.com/Amitsahu123789/Smart-Enterprise-Service-Incident-Management-System.git
```

Move into the project:

```bash
cd Smart-Enterprise-Service-Incident-Management-System
```

---

# 🔧 Backend Setup

Move to the backend directory:

```bash
cd backend
```

Configure the database and application properties according to your local environment.

Then install/build the project:

```bash
mvn clean install
```

Run the Spring Boot application:

```bash
mvn spring-boot:run
```

The backend API will normally be available at:

```text
http://localhost:8080
```

---

# 🎨 Frontend Setup

Open another terminal and navigate to:

```bash
cd frontend
```

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm run dev
```

The frontend will normally be available at:

```text
http://localhost:5173
```

---

# 🐳 Docker Setup

If Docker is configured for the project, you can start the required services using:

```bash
docker compose up --build
```

To stop the services:

```bash
docker compose down
```

---

# 🔑 Main Functional Modules

| Module | Description |
|---|---|
| Authentication | User registration and login |
| RBAC | Role-based authorization |
| Incident Management | Create and manage incidents |
| Investigation | Investigate and track incidents |
| Evidence | Upload and manage investigation evidence |
| Dashboard | Monitor incidents and statistics |
| Audit Logs | Track system activities |
| Notifications | Display incident-related notifications |
| Reports | Generate incident reports |
| Export | Export incident information to CSV |

---

# 🎯 Project Objectives

The main objectives of this project are:

- Build a practical enterprise-level full-stack application.
- Implement RESTful APIs using Spring Boot.
- Develop a responsive React frontend.
- Implement authentication and role-based authorization.
- Manage enterprise incident workflows.
- Integrate relational databases with a Spring Boot backend.
- Implement caching using Redis.
- Provide analytics and reporting functionality.
- Practice real-world software development architecture.

---

# 📚 What I Learned

Through this project, I gained practical exposure to:

- Java backend development
- Spring Boot application development
- REST API development
- Spring Security
- JPA/Hibernate
- PostgreSQL database integration
- Redis caching
- React application development
- Frontend-backend integration
- Authentication and authorization
- CRUD operations
- Enterprise application architecture
- Git and GitHub
- Docker-based development

---

# 🔮 Future Enhancements

Potential improvements include:

- JWT refresh-token architecture
- Real-time notifications using WebSockets
- Advanced SLA management
- Email notifications
- AI-powered incident classification
- Automated incident assignment
- Advanced security analytics
- Production cloud deployment
- Kubernetes deployment
- Comprehensive automated testing
- CI/CD pipeline
- Advanced monitoring and observability

---

# 📸 Screenshots

Add screenshots of the following modules to make the repository more professional:

- Login page
- Dashboard
- Incident creation
- Incident investigation
- Admin user management
- Analytics dashboard
- Incident details
- Reports

Example:

```markdown
## 📸 Screenshots

### Dashboard
![Dashboard](screenshots/dashboard.png)

### Incident Management
![Incident Management](screenshots/incidents.png)

### Investigation Workspace
![Investigation](screenshots/investigation.png)
```

---

# 👨‍💻 Developer

**Amit Sahu**

B.Tech Computer Science & Engineering  
Indore, Madhya Pradesh

### Profiles

- GitHub: https://github.com/Amitsahu123789
- LinkedIn: https://www.linkedin.com/in/amit-sahu-bb399927a
- LeetCode: https://leetcode.com/u/Amit_78/

---

# 📄 License

This project is distributed under the **MIT License**.

Please see the [`LICENSE`](LICENSE) file for complete license information.

This repository retains the applicable open-source license and attribution from the original project on which this work is based.

---

# ⭐ Acknowledgement

This project is based on an open-source **Threat Incident Management / SOC platform** and has been used as a foundation for learning, customization, and portfolio development.

Thanks to the original open-source contributors for making the project available under the MIT License.
