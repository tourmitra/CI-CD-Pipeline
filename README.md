# CI/CD Pipeline Automation System

## Project Overview
An automated CI/CD pipeline that builds, tests, and deploys a Python Flask web application whenever code is pushed to GitHub. The pipeline eliminates manual deployment steps by automatically triggering on every Git push.

## Tech Stack
| Tool | Purpose |
|------|---------|
| Python + Flask | Web application |
| Docker | Containerization |
| Jenkins | CI/CD automation |
| GitHub | Source code & webhooks |
| Microsoft Azure | Cloud hosting |

## How It Works
1. Developer pushes code to GitHub
2. GitHub Webhook notifies Jenkins
3. Jenkins pulls the latest code
4. Docker builds a new image
5. App is tested and deployed automatically

## Pipeline Stages
- **Clone** — Pulls latest code from GitHub
- **Build** — Builds Docker image
- **Test** — Runs tests
- **Deploy** — Runs the container on port 5000

## Deployment
- **Live App:** [\[LINK\]](http://40.81.18.32:5000/)
- **GitHub:** https://github.com/tourmitra/CI-CD-Pipeline.git

