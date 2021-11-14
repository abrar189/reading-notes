# What is Amazon S3?

Amazon Simple Storage Service (Amazon S3) is an object storage service that offers industry-leading scalability, data availability, security, and performance. Customers of all sizes and industries can use Amazon S3 to store and protect any amount of data for a range of use cases, such as data lakes, websites, mobile applications, backup and restore, archive, enterprise applications, IoT devices, and big data analytics. Amazon S3 provides management features so that you can optimize, organize, and configure access to your data to meet your specific business, organizational, and compliance requirements.

## Amazon S3 features

- Storage classes
- Bucket policies
- AWS Identity and Access Management
- Access control lists
- Versioning
- Operations

## Advantages of using Amazon S3

- Creating buckets – Buckets are the fundamental containers in Amazon S3 for data storage.

- Storing data – Store an infinite amount of data in a bucket. Upload as many objects as you like into an Amazon S3 bucket.

- Downloading data – Download your data or enable others to do so. Download your data anytime you like, or allow others to do the same.

- Permissions – Grant or deny access to others who want to upload or download data into your Amazon S3 bucket.

- Standard interfaces – Use standards-based REST and SOAP interfaces designed to work with any internet-development toolkit.

## Amazon S3 concepts

**[Buckets]**
A bucket is a container for objects stored in Amazon S3. Every object is contained in a bucket. Buckets serve several purposes:

- They organize the Amazon S3 namespace at the highest level.

- They identify the account responsible for storage and data transfer charges.

- They play a role in access control.

- They serve as the unit of aggregation for usage reporting.

**[Objects]**

Objects are the fundamental entities stored in Amazon S3. An object is uniquely identified within a bucket by a key (name) and a version ID.

**[Keys]**

A key is the unique identifier for an object within a bucket. Every object in a bucket has exactly one key.

**[Regions]**

You can choose the geographical AWS Region where Amazon S3 will store the buckets that you create.

**[Amazon S3 data consistency model]**

Amazon S3 provides strong read-after-write consistency for PUTs and DELETEs of objects in your Amazon S3 bucket in all AWS Regions.

## Paying for Amazon S3

Amazon S3 charges you only for what you actually use, with no hidden fees and no overage charges. This gives developers a variable-cost service that can grow with their business while enjoying the cost advantages of the AWS infrastructure.

## PCI DSS compliance

Amazon S3 supports the processing, storage, and transmission of credit card data by a merchant or service provider, and has been validated as being compliant with Payment Card Industry (PCI) Data Security Standard (DSS).