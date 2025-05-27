![Python, PostgreSQL on Google Cloud Platform Logo](_docs/python-postgresql-ai-google-cloud-platform-logo.png) 

This project shows how you can use **PostgreSQL** in
**Python** on the **Google Cloud Platform** and **locally**.

In this repository we have three projects:

- **🔐 Encrypt and Decrypt PDF Function** with Buckets.
- **🧑‍💻 Python User System Flask App (Backend) with PostgreSQL** lets users register and login to a backend.
- **🤖 Mental Health Check-In Assistant with AI** 
- **🧬 Lifestyle-Based Health Risk Scoring System Machine Learning** 

---

Table of contents:

1. [🎯 Applications](#-1-applications)
2. [💻 Software Needed](#-2-software-needed)
3. [🔗 Links](#-3-links)
4. [📜 License](#-4-license)


---


## 🎯 1 Applications

### 🔐 [Encrypt and Decrypt PDFs Function](encrypt-and-decrypt-pdfs)

* **Runs on:** Google Cloud Run Functions
* **GCP Services:**
  * Secret Manager 
 
* **Description:**
  PDF documents are stored in a Google Cloud Bucket named **originals**. 
  The documents there are encrypted into a directory named **encrypted**.
  When they are decrypted they are stored in a directory named **decrypted**.
  

### 🧑‍💻 [Python User System Flask App (Backend) with PostgreSQL](user-system)

* **Runs on:** Google Cloud Run
* **GCP Services:**
  * Cloud SQL (PostgreSQL)
  * Secret Manager

* **Description:**
  A basic user management system that handles sign-up, login, password hashing, 
  and user sessions using Flask and PostgreSQL. 
  
  Secret Manager securely stores database credentials, 
  and the service is deployed on Cloud Run with auto-scaling. 

  The project introduces secure cloud architecture, relational database access, 
  and containerized deployment.
  


### 🤖 [Mental Health Check-In Assistant with AI](mental-health-check-in-assistant-with-ai)

* Runs on: Google Cloud Run
* GCP Services: 
  * Vertex AI (LLM: PaLM/Gemini)
  * Secret Manager
  * Firestore (for storing journal entries)
  
* Description:
  Many people struggle to reflect on their mental health or spot patterns. 
  This app helps users write a daily mood journal and receive an AI-generated reflection or suggestion, 
  like “You seem anxious lately. Would taking a walk or journaling more help?”

  How it works:
    * User submits a short daily entry (text: how they feel, what happened).
    * Python backend sends this to Vertex AI via prompt, asking for:
      * Mood summary
      * Emotional trends
      * A gentle reflection or suggestion

    * Stores the entry + AI feedback in Firestore.

### 🧬 [Lifestyle-Based Health Risk Scoring System Machine Learning](lifestyle-based-health-risk-scoring-system-ml)

* Runs on: Google Cloud Run
* GCP Services:
  * Cloud Storage (for uploading or accessing test documents/data)
  * Firestore
  * Secret Manager 
  * Trained Scikit-learn model or TensorFlow Lite model

* Description:
  Many people get blood tests and have health habits (like smoking, exercise, etc.), 
  but don’t know how all their lifestyle and environmental factors add up to influence their overall health risk. 
  This app takes structured input and outputs a personalized health risk score.


  How it works:
    * User fills in a form (or uploads a JSON) with:
      * Blood test results (e.g. cholesterol, liver enzymes)
      * Lifestyle: exercise frequency, smoking, stress levels, diet
      * Exposures: radiation, environmental toxins, steroids, pharma
      * Nutrition: vitamins, minerals, amino acids
      * Subjective metrics: peace of mind, etc.

    * App runs a custom trained ML model to:
      * Predict a general health risk score (e.g., 0–100)
      * Optionally suggest which categories are most contributing to risk (feature importance)

    * Results stored in Firestore and shown via API.

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

[Python, Next.js, PostgreSQL and DevSecOps on Google Cloud Platform with Projects from Real Industry](https://github.com/ditlef9/python-nextjs-postgresql-devsecops-gcp) –  
Create six applications with this repository.
There is also an 
[Udemy Course](https://www.udemy.com/course/python-nextjs-postgresql-and-devsecops-on-google-cloud/?referralCode=FC37116C22B35FA1A907).


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

