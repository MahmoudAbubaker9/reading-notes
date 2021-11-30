# Notifications

### What is Amazon SNS?

* A managed service that provides message delivery from publishers to subscribers .
* Publishers communicate asynchronously with subscribers by sending messages to a topic, which is a logical access point and communication channel.
* Clients can subscribe to the SNS topic and receive published messages using a supported endpoint type.

## Features and capabilities

**Amazon SNS provides the following features and capabilities:**

* Reliably deliver messages with durability
Amazon SNS uses cross availability zone message storage to provide high message durability. Amazon SNS reliably delivers messages to valid AWS endpoints, such as Amazon SQS queues and AWS Lambda functions.

* Simplify your architecture with Message Filtering
Amazon SNS helps you simplify your pub/sub messaging architecture by offloading the message filtering logic from your subscriber systems, and message routing logic from your publisher systems.

* Automatically scale your workload
Amazon SNS leverages the proven AWS cloud to dynamically scale with your application. Amazon SNS is a fully managed service, taking care of the heavy lifting related to capacity planning, provisioning, monitoring, and patching.

* Keep messages private and secure
Amazon SNS topic owners can set topic policies that restrict who can publish and subscribe to a topic. Amazon SNS also ensures that data is encrypted in transit and at rest, and provides VPC endpoints for message privacy.

## Related services

**You can use the following services with Amazon SNS:**

* **Amazon SQS** offers a secure, durable, and available hosted queue that lets you integrate and decouple distributed software systems and components.

* **AWS Lambda** enables you to build applications that respond quickly to new information. Run your application code in Lambda functions on highly available compute infrastructure.

* **AWS Identity and Access Management (IAM)** helps you securely control access to AWS resources for your users. Use IAM to control who can use your Amazon SNS topics (authentication), what topics they can use, and how they can use them (authorization).

* **AWS CloudFormation** enables you to model and set up your AWS resources. Create a template that describes the AWS resources that you want, including Amazon SNS topics and subscriptions. AWS CloudFormation takes care of provisioning and configuring those resources for you.

### SNS with Amplify (and Firebase)
* Enable your users to receive mobile push messages sent from the Apple (APNs) and Google (FCM/GCM) platforms.
* The CLI deploys your push notification backend using Amazon Pinpoint
1.  add the SDK to your app.

```cd ./YOUR_PROJECT_FOLDER
amplify add notifications
```

2. Choose Firebase Cloud Messaging (FCM).
> FCM
3. Add the following dependencies and plugin to your app/build.gradle:

```dependencies {
    // Overrides an auth dependency to ensure correct behavior
    implementation 'com.google.android.gms:play-services-auth:19.2.0'

    // Import the BoM for the Firebase platform
    implementation platform('com.google.firebase:firebase-bom:28.2.1')
    implementation 'com.google.firebase:firebase-messaging'

    implementation 'com.amazonaws:aws-android-sdk-pinpoint:2.25.+'
    implementation ('com.amazonaws:aws-android-sdk-mobile-client:2.26.+@aar') { transitive = true }
}

apply plugin: 'com.google.gms.google-services'
```

4. Add the following to your project level build.gradle:

```
buildscript {
    dependencies {
        classpath 'com.google.gms:google-services:4.0.1'
    }
}

allprojects {
    repositories {
        google()
    }
}
```
5. added this tag to AndroidManifest.xml:

```<service
    android:name=".PushListenerService">
    <intent-filter>
        <action android:name="com.google.firebase.MESSAGING_EVENT"/>
    </intent-filter>
</service>
```



**************
**Additional resources**

[SNS: Getting Started](https://aws.amazon.com/sns/getting-started/)

[SNS with Amplify (and Firebase)](https://docs.amplify.aws/)

**************