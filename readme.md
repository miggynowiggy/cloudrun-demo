# Introduction to GCP

This is a sample repository that you can refer to when building projects that needs to be deployed to Google Cloud Run. The sample project used in this repository is directly copied from the sample app from the FAST API documentation. [LINK](https://fastapi.tiangolo.com/tutorial/sql-databases/#__tabbed_8_3)

---

This repository also contains a github action that automatically builds the docker image and deploy it Google Cloud Run on new commits, just visit `./github/workflow/deploy_changes.yml`

___

## Tech Stack:
- Python 3.10
- FAST API
- PostgreSQL 14
- SQLAlchemy (for ORM)
- Docker

---

## Google Cloud Technologies Used:
- Google Cloud Run
- Google Cloud SQL

---

## How to use the repository locally
1. Install Docker Desktop on your computer. Instruction might vary depending on your OS.

2. Run the app in dev mode (with hot-reload)
  `docker compose up -d

1. Enjoy!

___

## Deploying changes to Google App Engine using the gcloud CLI
1. run `gcloud auth login` and select the appropriate account
2. run `gcloud config set project <your-project-id>` to set the default project details in gcloud cli
3. run `gcloud app deploy app.yaml` and confirm the deployment
4. Wait till it says success
