# S3
[Notes taken from this site](https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html)

- Amazon Simple Storage Service (S3) can be used to store and protect data.
- Amazon S3 has different storage classes for different use cases/costs.
- Storage management:
  - >S3 Lifecycle - Configure a lifecycle policy to manage your objects and store them cost effectively throughout their lifecycle.
  - >S3 Object Lock - Prevent Amazon S3 objects from being deleted or overwritten for a fixed amount of time or indefinitely.
  - >S3 Replication - Replicate objects and their respective metadata and object tags to one or more destination buckets in the same or different AWS Regions for reduced latency, compliance, security, and other use cases.
  - >S3 Batch Operations - Manage billions of objects at scale with a single S3 API request or a few clicks in the Amazon S3 console. 
- Access Management:
  - >S3 Block Public Access
  - >AWS Identity and Access Management
  - >Bucket Policies - Use IAM-based policy language to configure resource-based permissions for your S3 buckets and the objects in them.
  - >Access Control Lists
  - >Access Analyzer for S3
- Data Processing:
  - >S3 Object Lambda - Add your own code to S3 GET requests to modify and process data as it is returned to an application.
  - >Event Notifications
Storage Logging and Monitoring
  - >Amazon CloudWatch metrics for Amazon S3


## Amplify Storage
[Notes taken from this site](https://docs.amplify.aws/lib/storage/getting-started/q/platform/android/)

Steps to add Amplify Storage:
1. Excute the following command in the project directory: `amplify add storage`
2. Enter the following when prompted:
```Java
? Please select from one of the below mentioned services:
    `Content (Images, audio, video, etc.)`
? You need to add auth (Amazon Cognito) to your project in order to add storage for user files. Do you want to add auth now?
    `Yes`
? Do you want to use the default authentication and security configuration?
    `Default configuration`
? How do you want users to be able to sign in?
    `Username`
? Do you want to configure advanced settings?
    `No, I am done.`
? Please provide a friendly name for your resource that will be used to label this category in the project:
    `S3friendlyName`
? Please provide bucket name:
    `storagebucketname`
? Who should have access:
    `Auth and guest users`
? What kind of access do you want for Authenticated users?
    `create/update, read, delete`
? What kind of access do you want for Guest users?
    `create/update, read, delete`
? Do you want to add a Lambda Trigger for your S3 Bucket?
    `No`
```
3. `amplify push`
4. Add dependencies:
```Java
dependencies {
    implementation 'com.amplifyframework:aws-storage-s3:1.28.3'
    implementation 'com.amplifyframework:aws-auth-cognito:1.28.3'
```
5. Initialize Amplify Auth & Storage in the `onCreate()` method:
```Java
Amplify.addPlugin(new AWSCognitoAuthPlugin());
Amplify.addPlugin(new AWSS3StoragePlugin());
```

[Back to HOME](../README.md)