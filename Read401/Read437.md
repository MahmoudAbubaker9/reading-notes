# Amazon S3

### What is Amazon S3?

Amazon Simple Storage Service (Amazon S3) is an object storage service offering industry-leading scalability, data availability, security, and performance.


### Advantages of using Amazon S3

* Creating buckets
* Storing data
* Downloading data
* Permissions
* Standard interfaces

### Amazon S3 features

* Storage classes
* Bucket policies
* AWS Identity and Access Management
* Access control lists
* Versioning
* Operations

### Amazon S3 concepts
* Buckets: is a container for objects stored in Amazon S3. Every object is contained in a bucket.

* Objects:Objects are the fundamental entities stored in Amazon S3. Objects consist of object data and metadata.

* Keys:A key is the unique identifier for an object within a bucket. Every object in a bucket has exactly one key.

* Regions:You can choose the geographical AWS Region where Amazon S3 will store the buckets that you create.

### The REST interface
* Using REST, you use standard HTTP requests to create, fetch, and delete buckets and objects.
* You can use any toolkit that supports HTTP to use the REST API.
* In some areas, we have added functionality to HTTP. In these cases, we have done our best to add the new functionality in a way that matched the style of standard HTTP usage.

# Install Amplify dependencies

* Expand Gradle Scripts, open build.gradle (Module: app).

* Add these libraries into the dependencies block:

```java
dependencies {
    implementation 'com.amplifyframework:aws-storage-s3:1.17.4'
    implementation 'com.amplifyframework:aws-auth-cognito:1.17.4'
}
```

# Initialize Amplify Storage

* To initialize the Amplify Auth and Storage categories you call `Amplify.addPlugin()` method for each category. To complete initialization call `Amplify.configure()`.

* Add the following code to your `onCreate()` method in your application class:

```java
Amplify.addPlugin(new AWSCognitoAuthPlugin());
Amplify.addPlugin(new AWSS3StoragePlugin());
```

**************
**Additional resources**

[Introduction to Amazon S3](https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html)

[S3 with Amplify](https://docs.amplify.aws/lib/storage/getting-started/)

**************