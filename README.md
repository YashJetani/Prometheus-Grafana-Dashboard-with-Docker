**# 📝 Django Notes App** 

A simple 2-tier Notes Application built with **Django** as the backend and deployed using **Docker & Docker Compose**.  
The project is fully automated with **Jenkins CI/CD pipeline** and monitored using **Prometheus, Grafana, and cAdvisor**.  

-----

**## 📌 Features**
- Create, update, and manage personal notes.
- Containerized using **Docker** for portability.
- Automated builds and deployments using **Jenkins CI/CD**.
- Real-time monitoring of containers with **Prometheus** using **cAdvisor**.
- Real-time visualization with **Grafana**.

-----

**## 🛠️ Tech Stack**
- **Backend**: Django (Python)  
- **Database**: SQLite3   
- **Containerization**: Docker, Docker Compose  
- **CI/CD**: Jenkins  
- **Monitoring**: Prometheus, Grafana, cAdvisor  

-----

** 📝 How To Execute**
**Step-1**
- Install **Java**
- Command :
-     sudo apt update
-     sudo apt install fontconfig openjdk-21-jre
-     java -version
- You can see O/P like this : openjdk version "21.0.3" 2024-04-16
                              OpenJDK Runtime Environment (build 21.0.3+11-Debian-2)
                              OpenJDK 64-Bit Server VM (build 21.0.3+11-Debian-2, mixed mode, sharing) 

**Step-2**
- Install **Jenkins**
- Command :
-     sudo wget -O /etc/apt/keyrings/jenkins-keyring.asc \
      https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key
-     echo "deb [signed-by=/etc/apt/keyrings/jenkins-keyring.asc]" \
      https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
      /etc/apt/sources.list.d/jenkins.list > /dev/null
-     sudo apt-get update
-     sudo apt-get install jenkins

**Step-3**
- Activate the **Jenkins** service
- Command :
-      sudo systemctl enable jenkins # for enable jenkins service
-      sudo systemctl start jenkins  # for stare jenkins service
-      sudo systemctl status jenkins # for the check cureent status of Jenkins.
