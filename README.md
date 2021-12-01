# spring-gumball ci/cd example
## CI Workflow
* Using the default yml is not suffient enough and gave errors so I had to change the gradle-publish.yml to the content provided
* CI Workflow deployed on Github
![CI Workflow Github](images/ciworkflow.png)
## CD Workflow
* Service account with admin and storage rights created
![Service account](images/serviceaccount.png)
* Service account key created as JSON, download and set secrets in Github repo's setting
![Service account keys](images/serviceaccountkey.png)
* Create new workflow for GKE, the workflow runs will be triggered by releases
![Latest release](images/release.png)
![GKE Deployment&Service](images/gkedeploymentservice.png)
![GKE service and pod running](images/servicepodrunning.png)
* Manually create Ingress in GKE
![Load Balancer created](images/loadbalancer.png)
* The application powered up but when I try using it by inserting a coin it shows a WhiteLabel error
![WhiteLabel error](images/error.png)
