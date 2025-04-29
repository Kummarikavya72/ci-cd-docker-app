# ci-cd-docker-app
project
Code is pushed to GitHub main branch.
2. GitHub Actions triggers the workflow.
3. Docker image is built and pushed to DockerHub.
4. Docker container is pulled and run on EC2 instance.

---

## 🔒 GitHub Secrets Configured
- `DOCKER_USERNAME` → DockerHub username
- `DOCKER_PASSWORD` → DockerHub password/access token

---
 Steps to Run Locally
bash
 Clone the repository
git clone https://github.com/kummarikavya/ci-cd-docker-app.git
cd ci-cd-docker-app

Build Docker image
docker build -t kummarikavya/ci-cd-app:latest .

 Run the container
docker run -d -p 3000:3000 kummarikavya/ci-cd-app:latest
Access the app at:
http://localhost:3000

git hub actions pipeline success build ![image](https://github.com/user-attachments/assets/72abeaa4-ac35-4647-a449-f16c34d8670a)

output of linux ![image](https://github.com/user-attachments/assets/154536b3-730d-4e37-956a-d7ff4f9f3288)
docker image ![image](https://github.com/user-attachments/assets/bab02341-dbf5-45b1-bdbf-19e2c4605c3a)
docker build ![image](https://github.com/user-attachments/assets/2b9259f8-a634-489f-9126-e7f2ed993b99)
