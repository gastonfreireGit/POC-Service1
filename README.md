## Azure Pipeline CI/CD

### How to Configure:

* Install AWS Tools for Azure DevOps: In this step, we will install AWS Tools for Azure DevOps on to your account. This will allow us to leverage the powerful features the add-on provides to created CICD tasks on AWS.

Navigate to [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=AmazonWebServices.aws-vsts-tools) and click on Get it free button as shown in the image below
![image](https://user-images.githubusercontent.com/97241135/158191350-6e6373d9-302d-49ea-8930-b9237b033b70.png)

* Setup AWS Connection with Azure DevOps: In this step, we will create a service connection to AWS on Azure DevOps. This will allow us to easily execute AWS specific tasks by simply selecting the service connection within the task itself 

Under Project Settings > Service connections, click on New Service connections and select AWS from that list.
<img src="https://user-images.githubusercontent.com/97241135/158192857-1ea9ad24-2ad6-403a-9bdd-4573deeb9e12.png" width="380">

![image](https://user-images.githubusercontent.com/97241135/158192604-18270c39-8932-42f7-9f20-b67d7f828cae.png)
