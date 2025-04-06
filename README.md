Automatic Deployment with Cloud Build (CI/CD)

This project is configured for automated deployment to Google Cloud Run using Cloud Build. It includes a secure, production-ready CI/CD pipeline and demonstrates best practices for managing cloud infrastructure, secrets, and service deployment.

Deployment Overview

Each time changes are pushed to the main branch, Cloud Build is triggered to:

Build the Docker image for the Django application.

Push the image to Google Container Registry.

Deploy the image to Cloud Run (staging environment).

Inject necessary environment variables and secrets securely from Secret Manager.

Secure Secret Management

Sensitive credentials like Google Cloud Storage keys are securely stored in Secret Manager and accessed during deployment without being hardcoded in the codebase.

The project uses:

GOOGLE_APPLICATION_CREDENTIALS_JSON secret for authenticating service accounts.

IAM bindings to restrict access to only Cloud Build and Cloud Run services.

TECH STACK

Python (Django)

MySQL (Cloud SQL)

Google Cloud Run

Google Cloud Build (CI/CD)

Docker

Secret Manager

Highlights

Fully automated deployment to Cloud Run.

CI/CD with Cloud Build, reducing manual steps.

Secure environment using Google Secret Manager.

Cloud SQL integration with private connections.

Cloud Storage for media/static file hosting.

Environment

This deployment currently targets the staging environment and can be easily extended to production with minor changes.

Why this matters

Setting up a secure, cloud-native CI/CD pipeline is critical for professional software development. This configuration demonstrates an understanding of:

Cloud infrastructure

CI/CD automation

Secure key management

Scalable deployment practices

This project is part of a personal portfolio showcasing cloud engineering and backend development skills.

For questions or collaboration inquiries, feel free to connect on LinkedIn.
