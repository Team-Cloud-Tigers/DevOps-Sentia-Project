# DevOps-Sentia-Project

GitHub page of Team Cloud-Tigers

In this Repository we will upload the deliverables needed for the Sentia cloud migration project. The following will be uploaded:

- An architectual design for all the components and all the environments.
- An IaC project for deploying an MVP demo.
- A simple time log of the activities we have performed.
- A document of assumptions and decisions we have made.

You can find the scenario of the assignment in the following link:

https://github.com/sentialabs/public-cloud-recruitment/blob/master/ASSIGNEMENT.md

# Architecture Overview

![image](https://user-images.githubusercontent.com/84905032/129204815-92e61b59-f806-4381-b123-106a5a9c8306.png)


# Infrastructure

To meet the customers' requirements the following AWS Infrastructure was made:
 
An architecture design based on an infrastructure as a code solution created by AWS CloudFormation using YAML.
   
This includes the following AWS Services or components:
 
 * CloudFormation: CloudFormation was chosen after testing Cloud Development Kit the customers' choice. This is because of the current knowledge about how to use CDK. 
AWS CloudFormation is a service that gives developers and businesses an easy way to create a collection of related AWS and third-party resources, and provision and manage them in an orderly and predictable fashion.

 * VPC: Virtual Private Cloud is a service that lets you launch AWS resources in a logically isolated virtual network that you define.
 
 * Public Subnets: The public subnet is a subnet that's associated with a route table that has a route to an internet gateway. This connects the VPC to the internet and to other AWS services.

 * Private Subnet: Instances in the private subnet are back-end servers that don't need to accept incoming traffic from the internet and therefore do not have public IP addresses.
 
 * Internet Gateway: An internet gateway serves two purposes: to provide a target in your VPC route tables for internet-routable traffic, and to perform network address translation (NAT) for instances that have been assigned public IPv4 addresses.
 
 * 2 EC2: An Amazon EC2 instance is a virtual server in Amazon's Elastic Compute Cloud (EC2) for running applications on the Amazon Web Services (AWS) infrastructure.
 
 * EC2 VPN client: A VPN client is a software based technology that establishes a secure connection between the user and a VPN server.
 
 * Elastic Beanstalk: Upload your code and Elastic Beanstalk automatically handles the deployment, from capacity provisioning, load balancing, auto-scaling to application health monitoring. At the same time, you retain full control over the AWS resources powering your application and can access the underlying resources at any time.
 
 * 2 DynamoDB: Amazon DynamoDB is a fully managed NoSQL database service that provides fast and predictable performance with seamless scalability.
 
 * Elastic Loadbalancer: Instead of a NGINX reverse proxy to deploy a NodeJS application an Elastic Load Balancer on EC2 instances was chosen. Elastic Load Balancing automatically distributes incoming application traffic across multiple targets, such as Amazon EC2 instances, containers, IP addresses, Lambda functions, and virtual appliances.
 
  * CloudWatch: CloudWatch collects monitoring and operational data in the form of logs, metrics, and events, and visualizes it using automated dashboards so you can get a unified view of your AWS resources, applications, and services that run in AWS and on-premises.
  
 * QuickSight Dashboard: The customer needs to have access via a publically accessibly dashboard within their headquarters. Amazon QuickSight connects to your data in the cloud and combines data from many different sources. In a single data dashboard, QuickSight can include AWS data, third-party data, big data, spreadsheet data, SaaS data, B2B data, and more. 
 
 * S3: Amazon Simple Storage Service is an object storage service that offers industry-leading scalability, data availability, security, and performance.
 
 * SFTP Server: For the customers to login to access their documents.
An SSH File Transfer Protocol (SFTP) server is an endpoint that is associated with a receiver or a destination during a message exchange. An SFTP server uses the SFTP transport protocol, which is an extension of the Secure Shell (SSH) cryptographic protocol.

 
 
 
  
 
 
 
 
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
  
- The Product Owner made one change to the above assignment: use a DynamoDB table instead of an ElasticSearch cluster.
- For AWS, write your IaC using: AWS CDK (preferred), or alternatively with AWS CloudFormation.
- Cost optimization should be applied when necessary, even if a few application related modifications are necessary. Environment isolation is important, but some shared services would be acceptable if they result in major cost reduction.


Company policies:
- Teams must work using the scrum methodology, including all the rituals and meetings.
- For new teams, one developer is chosen as scrum master. This is a double role, so they are developer and scrum master at the same time. They remain scrum master for the entire duration of the project. A scrum master gets a 50% pay raise (for a total of €0 x 150% = €0).
- Your Learning Coach is the product owner. 
- Resources must be tagged properly with the following tags(keys ,value); Project(k), devops(v) and TEAM(k), your team name here(v). 
Resources that are not properly tagged might randomly get deleted. The Cloud Team is not responsible for any lost data when you do not comply with these rules.

Approach:
 
Team worked together on research,testing and reviewing the project.

Assumptions and discussions were handled and made in a respectful and relaxed environment within the team.

        
         
# References:

https://acloudguru.com/blog/business/what-is-cloud-migration

https://www.slideteam.net/powerpoint/Cloud-Migration

https://aws.amazon.com/architecture/icons/
 
https://aws.amazon.com/cloudformation/
____________________________________________________________________________________________________


