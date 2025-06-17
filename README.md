# 🚀 DevOps API Testing CI/CD Pipeline Project

This is a complete **CI/CD pipeline project** using **Docker**, **Jenkins**, **Postman**, and **Newman** to run automated API tests and generate rich HTML reports — perfect for showcasing DevOps + QA skills in interviews and resumes.

---

## 🧠 What This Project Does

- 🐳 Dockerized Node.js sample API (Express)
- 📮 Postman Collection for API test cases
- ⚙️ Jenkins pipeline triggers on GitHub push
- ✅ Runs tests via Newman (CLI runner for Postman)
- 🧾 Auto-generates timestamped HTML test reports
- 📁 Reports stored inside a `/reports/` folder for review

---

## 🧰 Tools Used

- **Postman**: For writing API tests
- **Newman**: To run Postman tests from CLI
- **Docker**: For containerizing API and test runner
- **Jenkins**: To automate pipeline (CI/CD)
- **GitHub**: To trigger pipeline on code push

---

## ⚙️ CI/CD Flow Explained

> 🔁 This is what makes the project CI/CD:

1. You push changes to GitHub (`git push`)
2. Jenkins is automatically triggered
3. Jenkins pulls the code and runs the `jenkinsfile` pipeline
4. It builds the Newman Docker image
5. Runs API tests using the latest Postman collection
6. HTML report is generated with timestamp
7. Report is saved into `reports/` folder automatically

✅ *This entire process happens without manual intervention — that’s Continuous Integration & Delivery!*

---

## 🧪 Example Technologies in Action

- Your API is running on Docker container at port `3000`
- Postman tests hit the API endpoints and validate responses
- Newman runs inside Docker and produces HTML reports
- Jenkinsfile defines the pipeline — it's clean, version-controlled and replicable

---
## 📦 Project Structure (for understanding only)

api/ → Express API (Dockerized)
newman/ → postman_collection.json + Jenkinsfile
reports/ → Stores auto-generated HTML reports
Dockerfile → For Newman test runner image

yaml
Copy
Edit

---

## 🖥️ How to Run Locally

- Start Jenkins (in Docker):
docker run -d -p 8080:8080 -p 50000:50000 ^
-v jenkins_home:/var/jenkins_home ^
-v //var/run/docker.sock:/var/run/docker.sock ^
--name jenkins-devops jenkins/jenkins:lts

yaml
Copy
Edit

- Open Jenkins in browser: `http://localhost:8080`
- Create new pipeline and point it to GitHub repo
- Use the `jenkinsfile` from `/newman/` directory
- Trigger a build — Jenkins will run tests and save reports

---

## 📄 Sample Output

- ✅ Console logs with test summary
- 📁 `/reports/report-TIMESTAMP.html` generated every run
- 🔥 View reports directly in browser

---

## 💼 Why This is Resume-Worthy

- Shows you know CI/CD pipelines
- Covers automation, containers, API testing
- Demonstrates real-world team skills (versioning, reporting)
- Highly customizable for future enhancement

---

## 🙋 About Me

**Garvit Goel**  
DevOps | SRE | QA Automation  
📧 garvitgoel04@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/garvit-goel/)  

---

## 📌 Tags

`CI/CD` · `DevOps` · `Postman` · `Jenkins` · `Docker` · `Newman` · `Automation` · `HTML Reports``Pipeline` · `QA` · `SRE` · `Resume Project`
