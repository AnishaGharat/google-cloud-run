# google-cloud-app-engine
To deploy CI/CD on Cloud Run

---

### List of steps

The pipeline is deployed on _Google Cloud Run_ for deployment. CI/CD is 
The application uses the following resources on Google Cloud Platform:

The application uses the following resources on Google Cloud Platform:

1) Cloud Run

2) Cloud Build

3) Google Container Registry

5) Google Source Code Repositories   

6) Cloud Build Triggers

---

### Deployment

### Create the source code repository

`gcloud source repos create [REPOSITORY_NAME]`

### Create a Cloud Build Trigger to automate deployment on every build (Through the console)

### Clone the cloud repository on your local

`gcloud source repos clone [REPOSITORY_NAME] --project [PROJECT_ID]`

### Create a Cloud Build Trigger through the console 
    - In source repository configure the repository which is cloned to the local
    - In the configurations file, select the cloudbuild.yaml file
    - Select the branch to automate the deployment process on pushing to that branch

###  Push the code to the respective branch and the app engine service gets available

