#### A consulting firm repeatedly builds large architecture for their customers using AWS resources from several AWS services including IAM, Amazon EC2, Amazon RDS, DynamoDB and Amazon VPC. The consultants have architecture diagrams for each of their architectures, and are frustrated that they cannot automatically create their resources. Service that will immediately benefit to the organization is:
  * AWS Cloudformation. 
    * Cloudformation enables consultants to user their architecture diagrams to construct CloudFormation templates. 
    * Cloudformation is a service that helps you model and set up your Amazon Web Service resources so that you can spend less time managing those resources and more time focusing on your application that run on AWS. You can create a template that describes all the AWS resources that you want (like Amazon EC2 instance or Amazon RDS DB instances), and AWS CloudFormation takes care of provisioning and configuring those resources for you. 
    
#### An organization hosts a multi-language website on AWS, which is served using CloudFront. Language is specified in the HTTP request as shown below:
  * http://d11111f8.cloudfront.net/main.html?language=de
  * http://d11111f8.cloudfront.net/main.html?language=en
  * http://d11111f8.cloudfront.net/main.html?language=es
  
  **How should AWS Cloudfront be configured to deliver cache data in the correct language?**
   * Based on query string parameter
#### A Solution Architect is designing a shared service for hosting containers from several customers on Amazon ECS. These containers will use several AWS service. A container from one customer should not be able to access data from another customer. Which of the below solutions should the architect use to meet these requirements?
  * IAM roles for tasks
    * With IAM roles for Amazon ECS tasks, you can specify an IAM role to be used by the containers in a task. Applications are required to sign their AWS API requests with AWS credentials, and this feature provides a strategy to manage credentials for your application's use. This is similar to how Amazon EC2 instance profiles provide credentials to EC2 instances. 
  
#### There is a requirement to host a database on a EC2 Instance. It is also required that the EBS volume should support 12,000 IOPS. Which Amazon EBS volume type meets the performance requirement.
  * EBS Provisioned IOPS SSD
     * For high performance and high requirement as in this case, the ideal choice would be EBS Provisioned IOPS SSD. Suitable for large database workloads, such as MongoDB, Cassandra, Microsoft SQL Server, MySQL, PostgreSQL, Oracle. 
     * Genereal purpose SSD(gp2), on the other hand, is recommended for most wide variety of workloads, system boot volumes, virtual desktops, low-latency interactive apps, development and test environment. 

#### Development teams in your organization use S3 buckets to store log files for various applications hosted in AWS development environments. The developers intend to keep the logs for a month for troubleshooting purposes, and subsequently purge the logs. What feature will enable this requirement?
  * Configuring lifecycle rules on the S3 buckets. 
#### A legacy application need a proprietary file system. Which of the following can be used to store data accessibile by an EC2 instance?
  * AWS EFS
    * Amazon Elastic file system(EFS) provides simple, scalable file storage for use with Amazon EC2 instances in the AWS Cloud. Amazon EFS is easy to use and offers a simple interface that allows you to create and configure file systems quickly and easily. With Amazon EFS, storage capacity is elastic, growing and shrinking automatically as you add and remove files, so your application have the storarge they need, when they need it. 
    * When mounted on Amazon EC2 instances, an Amazon EFS file system provides a standard file system interface and file system access semantics, allowing you to seamlessly integrated EFS with your existing application and tools. Multiple Amazon EC2 instances can access an Amazon EFS file system at the same time.
#### What options can be used to host an application that uses NGINX and is scalable at any point in time?
  * AWS EC2
  * AWS Elastic Beanstalk
    * NGINX is an open source software for web serving, reverse proxying, caching, load balancing, etc. NGINX can be hosted in EC2 instance through a series of clear steps--Launch an EC2 instance through the console. SSH into the instance and use the command yum install -y nginx to install nginx. Also, make sure that it is configured to restart automatically after a reboot. 
    * It can also be installed with an ELastic Beanstalk service. To enable NGINX proxy server with your Tomcat application, you must add a configuration file to .ebeextentions in the application source bundle that you upload to Elastic Beanstalk. 
#### A million images are required to be uploaded to S3. What option ensures optimal performance in this case?
  * Use a hexadecimal hash for the prefix
    * One way to introduce randomeness to key names is to add a hash string as prefix to the key name. 
#### There is a requirement to get the IP addresses for resources accessed in a private subnet. Which of the following can be used  to fulfill this purporse?
  * VPC flow logs
    * VPC flow logs is a feature that enables you to capture your information about the IP traffic going to and from network interfaces in your VPC. 
#### A database is required for a Two-Tier application. The data would go through multiple schema changes. The database needs to be durable, and changes to the database should not result in database downtime. Which of the following is best option for downtime?
  * AWS Aurora
#### A Redshift cluster currently contains 60TB of data. There is a requirement that a disaster recovery site is put in place in a region located 600km away. Which of the following solutions would help ensure that this requirement is fulfilled?
  * Enable cross-region snapshots for the redshift cluster.
#### A company is using a Redshift cluster to store their data warehouse. There is a requirement from the internal IT Security team to encrypt data for the Redshift database. How can this be achieved?
  * Use AWS KMS Customer Default master key.