# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.


- Analyze costs: 
With created VM with Standard B1s - basic size  we will spend $4.09/month while we can create App service with free tier for deploy our application. 

- Scalability:
We can easily scale of VM such as CPU, RAM, storage when the application grows while App service can we only support to maximum of 14GB of memory and 4 vCPU cores per instance

- Availability:
Both of VM and App Service ensue high availability. VM provide 2 two options when it comes to scaling—Virtual Machine Scale Sets and Load Balancers . App service support both Linux and Windows environments but limited set of programming languages

- Workflow: 
With VM we need prepare and configuration everything for deploy applications like runtime, enviroment, open port, SSL, firewall, connect to domain, IIS,... while with App service we only focus to deployment and easily to configuration and Azure supports automated deployment directly from serveral resource like Azure Repos, GitHub, Bitbucket, Local git.

- So in this project App service is a good choise because this is a small application and we can config and deploy quickly to app service from Github and easily authenticate users with Active Directory

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 
-
If in the future the application grows, more data, develops more features and need seperate application to pices as well as security requirements, we need to move the application to the VM to scale up as well as full control database (security), backup....

- URL: https://chaothu.azurewebsites.net
