
Day-9 | AWS S3 Buckets Deep Dive | 2 Demo Projects with Code
============================================================



Q1) What is Amazon S3?

A1) Simple Storage Service is a scalable and secure cloud storage service provided by Amazon Web Services (AWS). It allows you to store and retrieve any amount of data from anywhere on the web.



Q2) What are S3 buckets?

A2) S3 buckets are containers for storing objects (files) in Amazon S3. Each bucket has a unique name globally across all of AWS. You can think of an S3 bucket as a top-level folder that holds your data.



Q3) Why use S3 buckets?

A3) S3 buckets provide a reliable and highly scalable storage solution for various use cases. They are commonly used for backup and restore, data archiving, content storage for websites, and as a data source for big data analytics.







# Key benefits of S3 buckets - 
================================


S3 buckets offer several advantages, including:

1) Durability and availability: S3 provides high durability and availability for your data.

2) Scalability: You can store and retrieve any amount of data without worrying about capacity constraints.

3) Security: S3 offers multiple security features such as encryption, access control, and audit logging.

4) Performance: S3 is designed to deliver high performance for data retrieval and storage operations.

5) Cost-effective: S3 offers cost-effective storage options and pricing models based on your usage patterns.







# Creating and Configuring S3 Buckets - 
========================================


To create an S3 bucket, you can use the AWS Management Console, AWS CLI (Command Line Interface), or AWS SDKs (Software Development Kits). You need to specify a globally unique bucket name and select the region where you want to create the bucket.

Choosing a bucket name and region

The bucket name must be unique across all existing bucket names in Amazon S3. It should follow DNS naming conventions, be 3-63 characters long, and contain only lowercase letters, numbers, periods, and hyphens. The region selection affects data latency and compliance with specific regulations.


Bucket properties and configurations


Versioning: Versioning allows you to keep multiple versions of an object in the bucket. It helps protect against accidental deletions or overwrites.


Bucket-Level Permissions and Policies - Bucket-level permissions and policies define who can access and perform actions on the bucket. You can grant permissions using IAM (Identity and Access Management) policies, which allow fine-grained control over user access to the bucket and its objects.







# Uploading and Managing Objects in S3 Buckets - 
=================================================


1) Uploading Objects to S3 Buckets - You can upload objects to an S3 bucket using various methods, including the AWS Management Console, AWS CLI, SDKs, and direct HTTP uploads. Each object is assigned a unique key (name) within the bucket to retrieve it later.



2) Object Metadata and Properties - Object metadata contains additional information abouteach object in an S3 bucket. It includes attributes like content type, cache control, encryption settings, and custom metadata. These properties help in managing and organizing objects within the bucket.



3) File Formats and Object Encryption - S3 supports various file formats, including text files, images, videos, and more. You can encrypt objects stored in S3 using server-side encryption (SSE). SSE options include SSE-S3 (Amazon-managed keys), SSE-KMS (AWS Key Management Service), and SSE-C (customer-provided keys).



4) Lifecycle Management - Lifecycle management allows you to define rules for transitioning objects between different storage classes or deleting them automatically based on predefined criteria. For example, you can move infrequently accessed data to a lower-cost storage class after a specified time or delete objects after a certain retention period.



5) Multipart Uploads - Multipart uploads provide a mechanism for uploading large objects in parts, which improves performance and resiliency. You can upload each part in parallel and then combine them to create the complete object. Multipart uploads also enable resumable uploads in case of failures.



6) Managing Large Datasets With S3 Batch Operations - S3 Batch Operations is a feature that allows you to perform bulk operations on large numbers of objects in an S3 bucket. It provides an efficient way to automate tasks such as copying objects, tagging, and restoring archived data.







# Advanced S3 Bucket Features - 
===================================


1) S3 Storage Classes - S3 offers multiple storage classes, each designed for different use cases and performance requirements.

AWS Documentation for AWS Storage Classes - https://aws.amazon.com/s3/storage-classes/




2) S3 Replication - S3 replication enables automatic and asynchronous replication of objects between S3 buckets in different regions or within the same region. Cross-Region Replication (CRR) provides disaster recovery and compliance benefits, while Same-Region Replication (SRR) can be used for data resilience and low-latency access.




3) S3 Event Notifications and Triggers - S3 event notifications allow you to configure actions when specific events occur in an S3 bucket. For example, you can trigger AWS Lambda functions, send messages to Amazon Simple Queue Service (SQS), or invoke other services using Amazon SNS when an object is created or deleted.




4) S3 Batch Operations - S3 Batch Operations allow you to perform large-scale batch operations on objects, such as copying, tagging, or deleting, across multiple buckets. It simplifies managing large datasets and automates tasks that would otherwise be time-consuming.








# Security and Compliance in S3 Buckets -
==========================================


1) S3 Bucket Security Considerations - Ensure that S3 bucket policies, access control, and encryption settings are appropriately configured. Regularly monitor and audit access logs for unauthorized activities.



2) Data Encryption At Rest and In Transit - Encrypt data at rest using server-side encryption options provided by S3. Additionally, enable encryption in transit by using SSL/TLS for data transfers.



3) Access Logging and Monitoring - Enable access logging to capture detailed records of requests made to your S3 bucket. Monitor access logs and configure alerts to detect any suspicious activities or unauthorized access attempts.









# S3 Bucket Management and Administration - 
=============================================




1) S3 Bucket Policies - Create and manage bucket policies to control access to your S3 buckets. Bucket policies are written in JSON and define permissions for various actions and resources.



2) S3 Access Control and IAM Roles - Use IAM roles and policies to manage access to S3 buckets. IAM roles provide temporary credentials and fine-grained access control to AWS resources.



3) S3 APIs and SDKs - Interact with S3 programmatically using AWS SDKs or APIs. These provide libraries and methods for performing various operations on S3 buckets and objects.



4) Monitoring and Logging with CloudWatch - Utilize Amazon CloudWatch to monitor S3 metrics, set up alarms for specific events, and collect and analyze logs for troubleshooting and performance optimization.



5) S3 Management Tools - AWS provides multiple management tools, such as the AWS Management Console, AWS CLI, and third-party tools, to manage S3 buckets efficiently and perform operations like uploads, downloads, and bucket configurations.










# Troubleshooting and Error Handling - 
========================================



1) Common S3 Error Messages and Their Resolutions - Understand common S3 error messages like access denied, bucket not found, and exceeded bucket quota. Troubleshoot and resolve these errors by checking permissions, bucket configurations, and network connectivity.



2) Debugging S3 Bucket Access Issues - Investigate and resolve issues related to access permissions, IAM roles, and bucket policies. Use tools like AWS CloudTrail and S3 access logs to identify and troubleshoot access problems.



3) Data Consistency and Durability Considerations - Ensure data consistency and durability by understanding S3's data replication and storage mechanisms. Verify that data is correctly uploaded, retrieve objects using proper methods, and address any data integrity issues.



4) Recovering Deleted Objects - If an object is accidentally deleted, you can often recover it using versioning or S3 event notifications. Additionally, consider enabling Cross-Region Replication (CRR) for disaster recovery scenarios.











----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


CA 



What is Amazon S3 - Amazon Simple Storage Servie S3 is an object storage service that offers Industry-Leading Scalability , Data Availability , Security and Performance.

What is Data Durability - Data durability refers to the guarantee that once data is written to a storage system, it will remain intact and accessible even in the face of failures, crashes, or power outages. In essence, it ensures that the data is reliably persisted over time. Durability is often achieved through techniques like replication, where data is stored in multiple locations, and by using mechanisms like checksums to detect and correct errors.


What is Data Availability - Data availability refers to the accessibility of data when it is requested. It ensures that the data is accessible and retrievable by users or applications whenever they need it. High data availability means that the system is up and running, and users can access their data without significant downtime or disruptions. This is often achieved through redundancy, load balancing, failover mechanisms, and quick recovery from failures.


Conclusion - In summary, data durability focuses on the long-term persistence and integrity of data, ensuring it's not lost or corrupted over time. Data availability, on the other hand, focuses on the real-time accessibility of data, ensuring it can be accessed by users or applications whenever needed, even in the face of failures.



---------------------------------------------------------------------------------------------------------------------------------------------------------------------



Features of Amazon Simple Storage Service (S3)  [SSL DAV SME LCD]

1. Security

2. Scalability

3. Lifecycle Management

4. Durability

5. Availability

6. Versioning

7. Storage Classes

8. Multipart Upload

9. Event Notifications

10. Logging & Monitoring

11. Cross region Replication

12. Data Transfer Acceleration



---------------------------------------------------------------------------------------------------------------------------------------------------------------------



Features Of Amazon S3 --> 

1) Storage Classes Amazon S3 offers a range of storage classes designed for different use cases.

A) You can store mission-critical production data in S3 Standard for frequent access.
B) Save costs by storing infrequently access data in S3 Standard-IA or One Zone-IA
C) Archive data at the lowest costs  in S3 Glacier Instant Retrieval , S3 Glacier Flexible Retrieval , S3 Glacier Deep Archive.


2) Storage Management S3 has storage management features that you can use to manage costs , meet regulatory requirements , reduce latency and save multiple distinct copies of your data for compliance requirements
A) S3 LifeCycle
B) S3 Object Lock
C) S3 Replication
D) S3 Batch Operations


3) Access Management and Security - Amazon S3 provides features for auditing and managing access to your buckets and objects. By default, S3 buckets and the objects in them are private. You have access only to the S3 resources that you create.
A) S3 Block Public Access 
B) AWS Identity and Access Management (IAM)
C) Bucket Policies 
D) Amazon S3 Access Points
E) Access Control Lists (ACLs)
F) S3 Object Ownership
G) IAM Access Analyzer for S3


4) Data Processing - To transform data and trigger workflows to automate a variety of other processing activities at scale, you can use the following features.
A) S3 Object Lambda
B) Event Notifications


5) Storage Logging and Monitoring - Amazon S3 provides logging and monitoring tools that you can use to monitor and control how your Amazon S3 resources are being used.
 --> Automated monitoring tools
A) Amazon CloudWatch metrics for Amazon S3
B) AWS CloudTrail 

 --> Manual monitoring tools
A) Server access logging
B) AWS Trusted Advisor


6) Analytics and Insights - Amazon S3 offers features to help you gain visibility into your storage usage, which empowers you to better understand, analyze, and optimize your storage at scale.
A) Amazon S3 Storage Lens
B) Storage Class Analysis
C) S3 Inventory with Inventory Reports


7) Strong Consistency - Amazon S3 provides strong read-after-write consistency for PUT and DELETE requests of objects in your Amazon S3 bucket in all AWS Regions. This behavior applies to both writes of new objects as well as PUT requests that overwrite existing objects and DELETE requests. In addition, read operations on Amazon S3 Select, Amazon S3 access control lists (ACLs), Amazon S3 Object Tags, and object metadata (for example, the HEAD object) are strongly consistent.



--> How Amazon S3 works

Amazon S3 is an object storage service that stores data as objects within buckets. An object is a file and any metadata that describes the file. A bucket is a container for objects.

To store your data in Amazon S3, you first create a bucket and specify a bucket name and AWS Region. Then, you upload your data to that bucket as objects in Amazon S3. Each object has a key (or key name), which is the unique identifier for the object within the bucket.

S3 provides features that you can configure to support your specific use case. For example, you can use S3 Versioning to keep multiple versions of an object in the same bucket, which allows you to restore objects that are accidentally deleted or overwritten.

Buckets and the objects in them are private and can be accessed only if you explicitly grant access permissions. You can use bucket policies, AWS Identity and Access Management (IAM) policies, access control lists (ACLs), and S3 Access Points to manage access.




====================================================================================================================



We get a service in aws which has all the 4 basic pillar and it is known as EC2 

vcpu's works pn threads (VCPU)- Compute
Giga instance in bytes(Gib) - Memory
Elastic Network Interface (ENI) - Network
Solid State Drive /Hard Disk Drive - Storage {SSD me latency kam rhegi q ki electrons k thru kaam krta usme disk mhi rhti isliye abhi HDD ko SSD se replace kur diye}

Private Cloud :- The co will manage the datacenter. 

Public Cloud :- The cloud prov will be managing the datacenter.

Hybrid Cloud :- Co will hve their own datacenter but will use public cloud as well.


Block Type Storage :- It will chop the data in small blocks and then store it. (Replication use krega jis wajah se data loss nhi hoga)

Object Type Storage (S3 and Ozone) :- It will store the data as it is in ozone and S3.


High Availability - Cust/ clients/organisaton wants that data should be available in clicks and minutes.


1. Infinitely Scalable

2. Minimum Administration (Monitiring).

3. Service Level Agreement Guarantee.

4. High Level Automation

5. Security - Maximum

6. Make the data available globally in minutes.

7. Blocking the unwanted public access.

8. Cost Optimization

 --> Structured Data - Clearly-defined data models; easy to search (eg. Spreadsheet)
 
 --> Semi Structured Data - Loosely-coupled data models (eg. JSON, XML) 
 
 --> UnStructured Data - No defined data models; difficult to search (eg. Text doc ,Image file, Video and Audio Files)


Availability
Durability - 99999999999 (11'9s of durability means once in a million years data will be loss but if the data is loss then AWS will give us compensation)


Data LifeCycle Policy - The data lifecycle refers to the stages through which data typically progresses during its existence within an organization or system. The data lifecycle is crucial for organizations to effectively manage, analyze, and derive value from their data while also complying with legal and regulatory requirements. It helps ensure that data is accurate, secure, and used responsibly throughout its journey within the organization.

Data LifeCycle Stages - Data Creation -> Data Ingestion -> Data Storage -> Data Processing -> Data Analysis -> Data Visualisation -> Data Sharing -> Data Archiving -> Data Retention -> Data Deletion -> Data Backup and Recovery  -> Data Security -> Data Governance -> Data Transformation -> Data Retirement.




--> How to create a bucket

1. Bucket name should be globally unique and you should give abbreveation (for eg. it is for Production,Development,Testing)


2. Select the region (You will get low latency)


3. Object Ownership (Jo bhi file create kiye uska ownership dena h ya nhi 


4. Block Public Access - (Hamesha public access block hi rkhne ka)


5. Bucket Versioning - (Copy generate hoti hai but Production me nhi krne ka)


6. Tags - Bohot sare departments ki buckets rhti h toh usko jis dept ki bucket h us hisab se tag dene ka.


7. Encryption - For eg ABCD ko apun ne 6*/& isme encrypt kiye toh jo bhi file open krega usko 6*/& dikhega Jab tuk key nhi dege samne wale ko jab tuk wo data ko decrypt nhi kur payega


8. Object Lock - Jo bhi data bucket me dalege and agar bucket me object lock laga hua h toh koi bhi wo data ko na read kr payega na write kr payega na delete kr payega.
