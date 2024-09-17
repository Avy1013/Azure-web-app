# Flask Application Deployment on Azure Web Apps with CI/CD

## Overview
This project is a simple Flask application deployed on **Azure Web Apps** using **GitHub Actions** for Continuous Integration and Continuous Deployment (CI/CD). The app has a single endpoint that returns "Hello, Azure Web Apps!" when accessed.

# Prerequisites
- Azure account
- GitHub account
- Python 3.x
- Basic knowledge of Flask and Azure Web Apps

## Includes two ways to deploy -
1. Manually create azure web app and then use ci/cd to deploy
2. Uses azure cli automates everything in one click uses with ci/cd

## Steps for 1st ---
1. Create a Azure app through azure portal 
> enable basic authencation to make sure you can download publish_profile
2. Push your simple flask app to github
3. use pip freeze in your enviroment to have requirement.txt
4. Write ci/cd yml 
    Includes following steps
    1. building and installing requirments
    2. deploying the app on webapp
5. run the Job
