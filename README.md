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



Infrastructure and environments:
 
To meet the client requirements we chose the following AWS infrastructure:
 
An architecture design based on an infrastructure as a code solution created by AWS CloudFormation using YAML.
  
This includes the following AWS Services:
    
    
 

 
 Client is currently hosting the following services on several virtual machines :
 
 * a customer facing web application on their on-premise environment based on a NodeJS application behind an NGINX reverse proxy.
 * the customer uses a MongoDB cluster for storing data as well as an FTP server for document storage. 
 * the customer maintains a cron server, mostly Bash and Python scripts, relevant to a small amount of jobs that need to be executed a few times per day (no more than once per hour).
 * the customer has 3 environments, namely Test, Acceptance and Production.

    
      
Goals:

The solution needs to be: 
- (must) scalable and flexible.
- (must) utilize managed services as much as possible.
- (nice to have) modernized during this migration in terms of infrastructure technologies used.



Topics to consider:
  
- The Learning Coach is making one change to the above assignment: to use a DynamoDB table instead of an ElasticSearch cluster.
- For AWS, write your IaC using: AWS CDK (preferred), or alternatively with AWS CloudFormation.
- Cost optimization should be applied when necessary, even if a few application related modifications are necessary. Environment isolation is important, but some shared services would be acceptable if they result in major cost reduction.



Approach:

# Activity log 

Activities:
 * Week 1 : 35 hours research
 * Week 2 : 20 hours research and 20 hours testing templates in CloudFormation
 * Week 3 : 10 hours testing final template in Cloudformation and 25 hours GitHub documentation

26th of July:
- The project details were made clear and our team started with doing research. Our first week mostly consisted of research and experimenting.

2nd of August:
- We made a draft of the services we wanted to use for the infrastructure and put them in a template.

3rd of August:
- We experimented more with the services and researched the synergy between them. 

4th of August:
- We tried deploying some of the services in AWS to see if we would run into errors.

6th of August:
- We made a definitive version of the template we created earlier in the week, and put the AWS services in we thought would perform best with each other.
 
 
         
         
References:

https://acloudguru.com/blog/business/what-is-cloud-migration

https://www.slideteam.net/powerpoint/Cloud-Migration

https://aws.amazon.com/architecture/icons/
 
https://aws.amazon.com/cloudformation/
____________________________________________________________________________________________________


