# 🚀 Deploying Portfolio Website using GitHub Actions & AWS

## 📌 Project Overview
This project demonstrates how to deploy a static portfolio website to AWS S3 using a fully automated CI/CD pipeline with GitHub Actions.

Whenever code is pushed to the `main` branch, the workflow automatically uploads the latest files to an S3 bucket.

---

## 🛠️ Tech Stack
- GitHub Actions (CI/CD)
- AWS S3 (Static Website Hosting)
- AWS IAM (Secure Access)
- YAML (Workflow Configuration)

---

## ⚙️ CI/CD Workflow
1. Code pushed to GitHub repository
2. GitHub Actions workflow is triggered
3. AWS credentials are configured securely
4. Website files are synced to S3 bucket
5. Portfolio is updated live 🚀

---

## 📂 Project Structure

---

## 🔐 GitHub Secrets Used
- `AWS_ACCESS_KEY_ID`
- `AWS_SECRET_ACCESS_KEY`

---

## 🪣 AWS S3 Configuration
- Bucket Name: `awsmz-portfolio-web`
- Static Website Hosting: Enabled
- Public Access: Configured

---

## 🚀 Deployment Command
```bash
aws s3 sync . s3://awsmz-portfolio-web --delete
