![Python, PostgreSQL on Google Cloud Platform Logo](_docs/python-postgresql-google-cloud-platform-logo.png) 

This project shows how you can use **PostgreSQL** in
**Python** on the **Google Cloud Platform** and **locally**.

This boilerplate provides a clean, minimal setup to jumpstart development using:

- **Python (FastAPI / Flask)** for backend logic
- **PostgreSQL** as the primary relational database
- **Google Cloud Platform (GCP)** for cloud deployment (Cloud Run, Cloud SQL and Secret Manager)

---

Table of contents:

1. [🎯 Applications](#-4-links)
2. [💻 Software Needed](#%EF%B8%8F-1--software-needed)
3. [🔗 Links](#-4-links)
4. [📜 License](#-5-license)


---


## 🎯 1 Applications

### 🔐 [Encrypt and Decrypt PDF Function](encrypt-and-decrypt-pdf-function)

* **Runs on:** Google Cloud Run Functions
* **GCP Services:**
  * Runs on: Cloud Run Function
  * Secrets: Secret Manager 
 
* **Description:**
  PDF documents are stored in a Google Cloud Bucket named **originals**. 
  The documents there are encrypted into a directory named **encrypted**.
  When they are decrypted they are stored in a directory named **decrypted**.
  

### 🧑‍💻 [Python User System Flask App (Backend) with PostgreSQL](user-system)

* **Runs on:** Google Cloud Run
* **GCP Services:**
  * Runs on: Cloud Run Functions
  * Database: Cloud SQL (PostgreSQL)
  * Secrets: Secret Manager

* **Description:**
  A basic user management system that handles sign-up, login, password hashing, 
  and user sessions using Flask and PostgreSQL. 
  
  Secret Manager securely stores database credentials, 
  and the service is deployed on Cloud Run with auto-scaling. 

  The project introduces secure cloud architecture, relational database access, 
  and containerized deployment.
  


### 🤖 [Dream Analyzer with AI](dream-analyzer-with-ai)

* Runs on: Google Cloud Run
* GCP Services: 
  * AI: Vertex AI (text analysis & summarization)
  * Runs on: Cloud Run 
  * Database: Cloud SQL (PostgreSQL)
  * Secrets: Secret Manager
  
* Description:
  A creative app where users input of dreams, and receive an AI-generated analysis including emotional tone, 
symbolic interpretation, and possible real-life correlations. 

Vertex AI processes and interprets dream text. 

The app demonstrates LLM integration, natural language processing, and secure deployment of an AI-powered API.

---

## 💻 2 Software Needed

Please install the following software:

* [Python](https://www.python.org/downloads) – The core programming language used in this project. 

* [PyCharm](https://www.jetbrains.com/pycharm/download) – A powerful IDE for Python development. 
It provides features like smart code completion, debugging, and project management.

* [PostgreSQL](https://www.postgresql.org/download) – The relational database used to store and manage data.
Note: On **Mac and Linux**, you also need to install pgAdmin, a GUI for managing your PostgreSQL databases.
(*pgAdmin is already included in the Windows PostgreSQL installer.*)

* [Git](https://git-scm.com/downloads) – A version control system used to manage and collaborate on your codebase. 
Essential for cloning the repo and contributing to the project.


---



## 🔗 3 Links

[Google Cloud Platform Docs](https://cloud.google.com/docs) –  
Official documentation for Google Cloud Platform. Learn how to deploy, secure, and manage applications using GCP services like Cloud Run, IAM, Cloud Functions, and more.

[Python Official Docs](https://docs.python.org/3/) –  
Comprehensive documentation for the Python programming language. Covers standard libraries, syntax, tutorials, and advanced programming techniques.

[PostgreSQL Documentation](https://www.postgresql.org/docs/) –  
Official reference for PostgreSQL, a powerful open-source relational database system. Learn about SQL syntax, configuration, security, and database management.

[GitHub Actions Docs](https://docs.github.com/en/actions) –  
Documentation for GitHub Actions, GitHub’s built-in CI/CD system. Learn how to automate workflows, set up pipelines, and integrate DevSecOps practices in your projects.


---

## 📜 4 License


This project is licensed under the
[Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/).

**⚠️ Warning: Educational Material Only**

This repository contains projects and resources created for educational purposes.

**This code is not intended for production use** and is provided **"as is"**. 
Use it at your own risk. No warranties or guarantees are provided, either express or implied. 

This material is **for students** enrolled in the course and is not meant to be used as part of any commercial product or service. 
Do not use the code as part of any production environment without thorough testing, modification, and security review.

