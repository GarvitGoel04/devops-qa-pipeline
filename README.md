# DevOps API Testing CI/CD Pipeline 🚀

This project demonstrates a complete CI/CD pipeline using **Jenkins**, **Docker**, and **Newman** for automated API testing with **Postman**. It runs your tests and generates an HTML report every time you push code.

---

## 🔧 Tech Stack

- **Docker** – Containerization of the API and Test Runner
- **Jenkins** – Automates the CI/CD process
- **Postman + Newman** – API tests and CLI execution
- **GitHub** – Version control and pipeline trigger
- **HTMLExtra Reporter** – Generates rich HTML reports

---

## 📁 Project Structure

devops-qa-pipeline/
├── api/ # Express.js sample API (Dockerized)
├── newman/
│ ├── postman_collection.json
│ └── jenkinsfile # Jenkins pipeline definition
├── reports/ # HTML reports saved here
├── Dockerfile # For Newman test runner
└── README.md # Project description

yaml
Copy
Edit
