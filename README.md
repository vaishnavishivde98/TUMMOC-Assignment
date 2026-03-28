################################################
TUMMOC-Assignment for DevOps Engineer
################################################


## Project Overview

This project demonstrates a **basic DevOps pipeline** for a Python application using:

* Python (Hello World app)
* Docker (containerization)
* Jenkins (CI/CD automation)

The goal is to show how a simple application can be **automatically built, tested, and deployed**.


## Application Details

A simple Python script:
```
print("Hello, DevOps with Jenkins!")
```

✔ Used to validate the CI/CD pipeline.

## CI/CD Pipeline (Jenkins)

The pipeline is defined in the `Jenkinsfile` and includes:

### 🔹 Stages

1. **Checkout**

   * Pulls the latest code from the GitHub repository

2. **Run App**

   * Executes the Python script to verify it works

3. **Build Docker Image**

   * Creates a Docker image using the Dockerfile

4. **Run Container**

   * Runs the application inside a Docker container



##  Docker Setup

### 🔸 Build Docker Image

```
docker build -t python-app .
```

### 🔸 Run Container

```
docker run python-app
```


## 🔧 Jenkins Setup

1. Install Jenkins (locally or using Docker)

2. Install required plugins:

   * Git Plugin
   * Pipeline Plugin
   * Docker Pipeline Plugin

3. Create a **Pipeline Job**

4. Connect your GitHub repository

5. Click **Build Now**



## Project Structure
TUMMOC-Assignment/
│
├── app/
│   ├── app.py
│   └── requirements.txt
│
├── Dockerfile
├── Jenkinsfile
└── README.md


## Output

```
Hello, DevOps with Jenkins!
```

