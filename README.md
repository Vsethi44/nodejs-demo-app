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
- ./screenshots/Repo_Push.png → Confirmation of initial code push on GitHub  

---

## Step 2: Create Dockerfile
1. Created `Dockerfile` in project root (capital D, no extension).  
2. Added Docker instructions to build the Node.js app image.  

**Screenshot:**  
- `Dockerfile.png` → Dockerfile content  

---

## Step 3: Add package.json
1. Initialized Node.js project:  
```powershell
npm init -y
Pushed package.json to GitHub repo.

Screenshot:

PackageJSON.png → Content of package.json

Step 4: Prepare GitHub Actions Workflow
Created .github/workflows/main.yml.

Defined workflow jobs:

npm install

Docker image build

DockerHub push

Screenshot:

Workflow_File.png → main.yml content

Step 5: Configure GitHub Secrets
Added the following secrets in GitHub repo → Settings → Secrets → Actions:

DOCKERHUB_USERNAME → DockerHub username

DOCKERHUB_TOKEN → DockerHub access token

Step 6: Run Workflow
Pushed local changes or manually triggered workflow.

GitHub Actions ran the workflow successfully.

Screenshots:

Workflow_Run.png → GitHub Actions workflow logs

DockerHub_Image.png → Docker image on DockerHub

Step 7: Submission
Task complete! ✅

GitHub repo link: https://github.com/Vsethi44/nodejs-demo-app

DockerHub image: vsethi786/nodejs-demo-app:latest