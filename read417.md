# AWS: S3 and Lambda

## Review, Research, and Discussion 👍

* Describe “The Cloud” 

 **The cloud refers to software and services that run on the Internet, instead of locally on your computer. Most cloud services can be accessed through a Web browser like Firefox or Google Chrome, and some companies offer dedicated mobile apps.**

* What is a container (as it relates to computers and servers)?

**Containers are a form of operating system virtualization. A single container might be used to run anything from a small microservice or software process to a larger application. Inside a container are all the necessary executables, binary code, libraries, and configuration files.**

* What is auto-scaling?

 **Autoscaling is a cloud computing feature that enables organizations to scale cloud services such as server capacities or virtual machines up or down automatically, based on defined situations such as traffic ir utilization levels.**

* What is bandwidth?

**The maximum amount of data transmitted over an internet connection in a given amount of time. Bandwidth is often mistaken for internet speed when it's actually the volume of information that can be sent over a connection in a measured amount of time – calculated in megabits per second (Mbps).**

* How do cloud providers compute service costs?

**When setting price, cloud providers determine the expense to maintaining the network. They start by calculating costs for network hardware, network infrastructure maintenance, and labor. These expenses are added together and then divided by the number of rack units a business will need for its IaaS cloud.**

--------------------------------------------------------------------------


### Document the following Vocabulary Terms 📑
|||
|-----|-----|
|Server Instances|a collection of SQL Server databases which are run by a solitary SQL Server service or instance. The details of each server instance can be viewed on the service console which can be web-based or command-line based.|
|Containers| is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another. A Docker container image is a lightweight, standalone, executable package of software that includes everything needed to run an application: code, runtime, system tools, system libraries and settings.|
|Cloud Services|are infrastructure, platforms, or software that are hosted by third-party providers and made available to users through the internet. |
|Cloud Architecture|the technology components that are combined to build a cloud, where resources are pooled through virtualization technology and shared across a network. ... A front-end platform (the client or device used to access the cloud) One or more back-end platforms (servers and storage)|
|AWS|(Amazon Web Services) is a comprehensive, evolving cloud computing platform provided by Amazon that includes a mixture of infrastructure as a service (IaaS), platform as a service (PaaS) and packaged software as a service (SaaS) offerings.|
|EC2/Beanstalk vs Heroku|Heroku and AWS Elastic Beanstalk, solutions (production configurations) is that they have comparable features and pricing. ... On the other hand, Heroku is generally simpler to get up and running as AWS has a fairly steep initial learning curve.|

----------------------------------------------

## Preview 📙

Which 3 things had you heard about previously and now have better clarity on?
Socket,
events,
WRRC
Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
AWS,
Tree data structure,
UDP

What are you most excited about trying to implement or see how it works?
AWS & react.js


----------------------------------------------

## Preparation Materials 📚

**Amazon S3** 

* Object storage built to retrieve any amount of data from anywhere

* Amazon Simple Storage Service (Amazon S3) is an object storage service offering industry-leading scalability, data availability, security, and performance. Customers of all sizes and industries can store and protect any amount of data for virtually any use case, such as data lakes, cloud-native applications, and mobile apps. With cost-effective storage classes and easy-to-use management features, you can optimize costs, organize data, and configure fine-tuned access controls to meet specific business, organizational, and compliance requirements. [TO KNOW MORE](https://aws.amazon.com/s3/)


**What is AWS Lambda?**

* AWS Lambda is a serverless computing service provided by Amazon Web Services (AWS). Users of AWS Lambda create functions, self-contained applications written in one of the supported languages and runtimes, and upload them to AWS Lambda, which executes those functions in an efficient and flexible manner.

* Each Lambda function runs in its own container. When a function is created, Lambda packages it into a new container and then executes that container on a multi-tenant cluster of machines managed by AWS. Before the functions start running, each function’s container is allocated its necessary RAM and CPU capacity. Once the functions finish running, the RAM allocated at the beginning is multiplied by the amount of time the function spent running. The customers then get charged based on the allocated memory and the amount of run time the function took to complete. [TO KNOW MORE](https://www.serverless.com/aws-lambda)

**Content Delivery Network (CDN)**

* A Content Delivery Network (CDN) is a geographically distributed group of servers that work together to provide fast delivery of Internet content. A CDN allows for the fast transfer of data needed for loading Internet content including HTML pages, javascript files, stylesheets, images, and videos.

 #### &copy; Dima Alabsi; 2021