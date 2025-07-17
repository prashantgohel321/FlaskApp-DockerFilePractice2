# 🚀 Deploy Flask App on AWS EC2 using Docker

A complete step-by-step tutorial on how to deploy a **Python Flask App** on an **AWS EC2 instance** using **Docker**, aimed at beginners in DevOps and Cloud Computing.

🎥 **Watch the Full Video Tutorial Here:**  
[Watch on YouTube](https://youtu.be/jl9v_HVhD4Y?si=P65ejtOE0v59uUoe)

---

## 📌 What You'll Learn

- Launch and configure an AWS EC2 instance
- Connect to EC2 using SSH in WSL (Ubuntu on Windows)
- Install Docker on EC2 instance
- Clone a simple Flask app with `app.py`, `run.py`, and `req.txt`
- Write a custom `Dockerfile`
- Build and run a Docker image
- Expose the Flask app on the browser using public IP

---

## 🛠️ Technologies Used

- AWS EC2 (Ubuntu)
- Docker & Dockerfile
- Python 3.7
- Flask
- Git
- WSL (Ubuntu on Windows)

---

## 🧾 Dockerfile Used

```Dockerfile
FROM python:3.7
WORKDIR /app
COPY . .
RUN pip install -r req.txt
ENTRYPOINT ["python"]
CMD ["run.py"]
```

## 🧪 Key Commands
```bash
sudo apt update
sudo apt install docker.io
git clone <your-flask-repo-url>
docker build -t flask-app .
docker run -d -p 80:80 flask-app
```

## 🌐 Demo
Once deployed, access your app using:
```bash
http://<your-ec2-public-ip>
```

## 🔗 Useful Links
- [Youtube Video](https://youtu.be/jl9v_HVhD4Y?si=P65ejtOE0v59uUoe)
- [Linkedin](https://www.linkedin.com/in/prashantgohel1706/) | [dev.to](https://dev.to/prashant_gohel_321) | [Youtube Channel](https://www.youtube.com/@DevOpsWithUs)
