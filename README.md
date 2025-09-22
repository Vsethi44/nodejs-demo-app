# Node.js Demo App – CI/CD Pipeline with GitHub Actions

## Project Overview
This project demonstrates **CI/CD automation for a Node.js app** using **GitHub Actions** and **DockerHub**.  
- **Objective:** Automate build and deployment of a Node.js app using Docker.  
- **Tools:** GitHub, GitHub Actions, Node.js, Docker, DockerHub  

---

## Step 1: Repository Setup
1. Created local folder `nodejs-demo-app`.  
2. Created a GitHub repo with the same name.  
3. Connected local folder to GitHub and pushed initial commit 

**Screenshot:**  
![Confirmation of initial code push on GitHub](./screenshots/Repo_Push.png)

---

## Step 2: Create Dockerfile
1. Created `Dockerfile` in project root (capital D, no extension).  
2. Added Docker instructions to build the Node.js app image.  

**Screenshot:**  
![Dockerfile content](./screenshots/Dockerfile.png)

---

## Step 3: Add package.json
1. Initialized Node.js project:  

'npm init -y'

2. Pushed package.json to GitHub repo.

Screenshot:

![Content of package.json](./screenshots/PackageJSON.png) 

## Step 4: Prepare GitHub Actions Workflow

1. Created .github/workflows/main.yml.

2. Defined workflow jobs:

- npm install

- Docker image build

- DockerHub push

Screenshot:

![main.yml content](./screenshots/Workflow_File.png)

## Step 5: Configure GitHub Secrets

1. Added the following secrets in GitHub repo → Settings → Secrets → Actions:

DOCKERHUB_USERNAME → DockerHub username

DOCKERHUB_TOKEN → DockerHub access token

## Step 6: Run Workflow

1. Pushed local changes or manually triggered workflow.

2. GitHub Actions ran the workflow successfully.

Screenshots:

![GitHub Actions workflow logs](./screenshots/Workflow_Run.png)

![Docker image on DockerHub](./screenshots/DockerHub_Image.png)

## Step 7: Submission
Task complete! ✅

GitHub repo link: https://github.com/Vsethi44/nodejs-demo-app

DockerHub image: https://hub.docker.com/repository/docker/vsethi786/nodejs-demo-app/general