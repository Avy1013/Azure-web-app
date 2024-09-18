# Flask Application Deployment on Azure Web Apps with CI/CD

## Overview
This project is a simple Flask application deployed on **Azure Web Apps** using **GitHub Actions** for Continuous Integration and Continuous Deployment (CI/CD). The app has a single endpoint that returns "Hello, Azure Web Apps!" when accessed.

## Prerequisites
- [Azure account](https://azure.microsoft.com/en-us/free/)
- [GitHub account](https://github.com/)
- [Python 3.x](https://www.python.org/downloads/)
- Basic knowledge of Flask and Azure Web Apps

## Deployment Methods

1. **Manual Azure Web App creation with CI/CD deployment**


---

### 1. Manual Azure Web App Creation with CI/CD

#### Steps:
1. **Create an Azure Web App via the Azure Portal**
   - Ensure **Basic Authentication** is enabled so you can download the `publish_profile`.
   
2. **Push your Flask app to GitHub** 
   - Ensure the code is hosted in a GitHub repository.

3. **Generate `requirements.txt`**
   - Use `pip freeze` in your virtual environment to create the `requirements.txt` file:
     ```bash
     pip freeze > requirements.txt
     ```

4. **Set up the CI/CD pipeline**
   - Write a GitHub Actions YAML file that:
     1. Builds and installs the necessary requirements.
     2. Deploys the app to the Azure Web App using the `publish_profile`.
     3. Make Sure that publish_profile is in the secrets.

5. **Run the GitHub Actions workflow**
   - Trigger the workflow by pushing your code to the main branch.

---


