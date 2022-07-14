# sklearn-app [![Python application test with Github Actions](https://github.com/Jantzilla/sklearn-app/actions/workflows/python-app.yml/badge.svg)](https://github.com/Jantzilla/sklearn-app/actions/workflows/python-app.yml)

This project is a machine learning microservice API built using Flask, Kaggle and Sklearn.

## Project Plan

* [Trello board](https://...) for the project
* A ![spreadsheet](/...) that includes the original and final project plan

## Instructions

To run the project, first start by opening the Azure Cloud Shell, cloning the code repository and navigating to it's main directory. This can be done by running the following commands:

`git clone https://github.com/Jantzilla/sklearn-app.git`

`cd sklearn-app`

### Project cloned into Azure Cloud Shell
![cloned project](/screenshots/ssh-git-clone.png)

After that you should setup, install, test, and lint the project by running `make all`

### Passing tests that are displayed after running the `make all` command from the `Makefile`
![make all command](/screenshots/make-all.png)

Once you've done this you can optionally choose to enter the virtual environment created in the previous `make all` step by using the following command:

`source ~/.sklearn-app/bin/activate`

Finally, you can start the project by running the command: `python app.py`

Now that your project is running, you will need to open a separate Azure Cloud Shell session at which point you will be able to run the prediction script! 

Do this by running  `./make_prediction.sh`

### Output of a test run
![test run](/screenshots/test-run.png)

## Enhancements

You can improve this project by adding CI/CD (Continuous Integration/Continuous Deployment) integration, deploying to Azure App Services, running load test, and examining the apps log output. I've included some images of these project enhancements below.

### Architectural Diagram (Shows the entire Azure DevOps integration)
![Azure App Service](/udacity-architecture-diagram.png)

### Project running on Azure App Service
![Azure App Service](/screenshots/azure-app-services.png)

### Successful deploy of the project in Azure Pipelines.  [Note the official documentation should be referred to and double checked as you setup CI/CD](https://docs.microsoft.com/en-us/azure/devops/pipelines/ecosystems/python-webapp?view=azure-devops).
![Deploy](/screenshots/azure-deploy.png)

### Running Azure App Service from Azure Pipelines automatic deployment
![Running App](/screenshots/running-azure-app.png)

### Successful prediction from deployed flask app in Azure Cloud Shell.
![Prediction](/screenshots/azure-app-services-prediction.png)

### Output of streamed log files from deployed application
![Logs](/screenshots/app-logs.png)

### Locust Console Configuration
![Locust Console](/screenshots/locust-console-start.png)

### Running Locust Load Test
![Locust Test](/screenshots/locust-load-test.png)

## Demo

I've also provided a short demo of how the application would look after implementing the entire DevOps workflow which can be viewed at the following [link](https://youtu.be/lzZCmYEWvMw)


