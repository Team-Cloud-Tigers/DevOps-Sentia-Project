# DevOps-Sentia-Project

GitHub page of Team Cloud-Tigers

In this Repository we will upload the deliverables needed for the Sentia cloud migration project. The following will be uploaded:

- An architectual design for all the components and all the environments.
- An IaC project for deploying an MVP demo.
- A simple time log of the activities we have performed.
- A document of assumptions and decisions we have made.

You can find the scenario of the assignment in the link:

https://github.com/sentialabs/public-cloud-recruitment/blob/master/ASSIGNEMENT.md

# Architecture Overview

![template1-designer (3)](https://github.com/Team-Cloud-Tigers/DevOps-Sentia-Project/blob/70859aa28b3b0b10c407dc74f48201f5496d9c25/Diagram/FinalTmpltPRODUCTION.png)

# Topics

 * References
 
    Websites,videos

 * Infrastructure and environments
 
 To meet the client requirements we did 
 
 Client is currently hosting the following services on several virtual machines :
 
 * a customer facing web application on their on-premise environment based on a NodeJS application behind an NGINX reverse proxy.
 * the customer uses a MongoDB cluster for storing data as well as an FTP server for    document storage. 
 * the customer maintains a cron server, mostly Bash and Python scripts, relevant to a small amount of jobs that need to be executed a few times per day (no more than once per hour).
 * the customer has 3 environments, namely Test, Acceptance and Production.

     
 
 * Goals

Provide environment separation
Provide basic security sandbox per environment
Integration for human user management
Allow sharing resources across environments where required

 * Topics to consider

security
CI/CD
accounting

* Approach

# Activity log 

Click [here]:
 
 
         



