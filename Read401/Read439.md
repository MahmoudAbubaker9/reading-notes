# Amplify and Kinesis

* Amazon Kinesis makes it easy to collect, process, and analyze real-time, streaming data so you can get timely insights and react quickly to new information.

## Getting started

- The **Analytics category** -> used to collect analytics data for your App.
- The Analytics category comes with built-in support for **Amazon Pinpoint** and **Amazon Kinesis** (Kinesis only available in the Amplify JavaScript library).

## Set up Analytics backend

1. `amplify add analytics`

```
? Select an Analytics provider (Use arrow keys)
    `Amazon Pinpoint`
? Provide your pinpoint resource name:
    `yourPinpointResourceName`
? Apps need authorization to send analytics events. Do you want to allow guests and unauthenticated users to send analytics events? (we recommend you allow this when getting started)
    `Yes`
```

2. `amplify push`

## Install Amplify Libraries

- Inside `build.gradle (Module: app)`:

```
dependencies {
    // Add these lines in `dependencies`
    implementation 'com.amplifyframework:aws-analytics-pinpoint:1.24.0'
    implementation 'com.amplifyframework:aws-auth-cognito:1.24.0'
}
```

## Initialize Amplify Analytics

- How the class should look like :

```
public class MyAmplifyApp extends Application {
    @Override
    public void onCreate() {
        super.onCreate();

        try {
            // Add these lines to add the AWSCognitoAuthPlugin and AWSPinpointAnalyticsPlugin plugins
            Amplify.addPlugin(new AWSCognitoAuthPlugin());
            Amplify.addPlugin(new AWSPinpointAnalyticsPlugin(this));
            Amplify.configure(getApplicationContext());

            Log.i("MyAmplifyApp", "Initialized Amplify");
        } catch (AmplifyException error) {
            Log.e("MyAmplifyApp", "Could not initialize Amplify", error);
        }
    }
}
```

### Benefits of Kinesis

* **Real-time:** Amazon Kinesis enables you to ingest, buffer, and process streaming data in real-time, so you can derive insights in seconds or minutes instead of hours or days.

* **Fully managed:** Amazon Kinesis is fully managed and runs your streaming applications without requiring you to manage any infrastructure.

* **Scalable:** Amazon Kinesis can handle any amount of streaming data and process data from hundreds of thousands of sources with very low latencies.


