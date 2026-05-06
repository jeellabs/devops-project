DevOps Project: Flask App with Docker, Nginx, MySQL & CI/CD

📌 Project Overview

This project demonstrates a complete **DevOps workflow** by building and deploying a containerized web application using modern tools and practices.

The application is a simple **Flask web app**, containerized with Docker, served via Nginx, connected to a MySQL database, and deployed on AWS EC2 with a CI/CD pipeline using GitHub Actions.

---

Architecture

User → Nginx → Flask App → MySQL Database
                 ↑
              Docker
                 ↑
        GitHub Actions → AWS EC2


---

Tech Stack

* **Backend:** Python (Flask)
* **Database:** MySQL
* **Containerization:** Docker
* **Reverse Proxy:** Nginx
* **Cloud:** AWS EC2
* **CI/CD:** GitHub Actions
* **Version Control:** Git & GitHub

---

Project Structure


devops-project/
│── app.py
│── requirements.txt
│── Dockerfile
│── docker-compose.yml
│── nginx.conf
│── README.md


---

Setup & Installation

Clone the repository

bash
git clone https://github.com/jeellabs/devops-project.git
cd devops-project


---

Run using Docker Compose

bash
docker-compose up --build


---

Access the application

Open your browser:


http://localhost


---

Docker Details

* Flask app runs inside a container
* MySQL runs as a separate container
* Nginx acts as a reverse proxy
* All services are managed via Docker Compose

---

Deployment (AWS EC2)

1. Launch EC2 instance (Ubuntu)
2. Install Docker & Docker Compose
3. Clone this repository
4. Run:

bash
docker-compose up -d --build


5. Access using:


http://<EC2-PUBLIC-IP>


---

CI/CD Pipeline (GitHub Actions)

* Trigger: Push to `main` branch
* Workflow:

  * Connect to EC2 via SSH
  * Pull latest code
  * Rebuild containers
  * Restart application

---

Features

* Containerized multi-service application
* Reverse proxy with Nginx
* Database integration with MySQL
* Cloud deployment on AWS
* Automated deployment using CI/CD

---

Learning Outcomes

* Hands-on experience with Docker & Docker Compose
* Understanding of reverse proxy (Nginx)
* Cloud deployment using AWS EC2
* CI/CD pipeline implementation
* Real-world DevOps workflow

---

🚀 Future Improvements

* Add HTTPS (SSL using Let's Encrypt)
* Add domain name
* Implement logging & monitoring
* Use Kubernetes for orchestration
* Add load balancer

---

Author

**Jeel**
Aspiring DevOps Engineer 🚀

---

Contribute / Support

If you like this project, feel free to ⭐ the repository and share!

