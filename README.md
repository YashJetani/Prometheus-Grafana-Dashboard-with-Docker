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
-      sudo systemctl enable jenkins 
-      sudo systemctl start jenkins  
-      sudo systemctl status jenkins

**Step-4**
- Access the Jenkins service on your Browser.
-     http://<YOUR_IP>:8080
- Then, Login using the password and install suggested pluging.
- Set your DockerHub credentails as a Globle credentails.
- Create a pipeline and configure it for Git SCM.
- Then, Run ** Build **.

**Step-5**
- Access all the service on Browser.
- Notes App : http://<YOUR_IP>:8000
- Grafana : http://<YOUR_IP>:3000  # If not working try port : 3001
- Prometheus: http://<YOUR_IP>:9090
- cAdvisor: http://<YOUR_IP>:8080  # If not working try port : 8081

-----

** 📊 Images of Grafana Dashboard :
<img width="960" height="416" alt="img4" src="https://github.com/user-attachments/assets/f1801e4d-2254-4ec3-8712-4be4c81e6209" />
<img width="944" height="417" alt="img5" src="https://github.com/user-attachments/assets/7f1ac2f2-ce1a-4009-adb6-079549b68ea2" />
<img width="944" height="410" alt="img6" src="https://github.com/user-attachments/assets/98121523-475c-44b6-a128-9f0119a99f80" />


- If you want to create Dashboard like this you can use official website of Grafana-templates.
- **Link** : https://grafana.com/grafana/dashboards/
