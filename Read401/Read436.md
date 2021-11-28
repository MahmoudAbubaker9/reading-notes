# Cognito

* The Amplify Auth category provides an interface for authenticating a user.

* Cognito lets you add user sign-up, sign-in, and access control to your web and mobile apps quickly and easily.

## Configure Auth Category

**To start provisioning auth resources in the backend, go to your project directory and execute the command:**

1. ###  `amplify add auth`

- Enter the following when prompted:

```bash
$ Do you want to use the default authentication and security configuration?
    `Default configuration`
$ How do you want users to be able to sign in?
    `Username`
$ Do you want to configure advanced settings?
    `No, I am done.`
```

- To push your changes to the cloud, execute the command:

2. ### `amplify push`


### Install Amplify Libraries

- Add the following dependency to your app‘s `build.gradle` along with others you added above in Prerequisites and click “Sync Now” when prompted:

```java
dependencies {
    implementation 'com.amplifyframework:aws-auth-cognito:1.17.4'
}
```

### Initialize Amplify Auth

- Add the Auth plugin before calling  **Amplify.configure**

```java
// Add this line, to include the Auth plugin.
Amplify.addPlugin(new AWSCognitoAuthPlugin());
Amplify.configure(getApplicationContext());
```

### Check the current auth session

- We can now check the current auth session.

- For testing purposes, you can run this from your MainActivity’s `onCreate` method.

```java
Amplify.Auth.fetchAuthSession(
    result -> Log.i("AmplifyQuickstart", result.toString()),
    error -> Log.e("AmplifyQuickstart", error.toString())
);
```

### Sign in

- The Auth category can be used to register a user, confirm attributes like email/phone, and sign in with optional multi-factor authentication. It is set up to use Amazon Cognito User Pools which manages the users and their properties.

### Reset password

* In order to reset your password, use the resetPassword api - this will send a code to the user attribute configured to receive such a reset code (e.g. email or SMS):
* To complete the password reset process, invoke the confirmResetPassword api with the code you were sent and the new password you want.

### Sign out

* Invoke the signOut api to sign out a user from the Auth category. You can only have one user signed in at a given time.
* Calling signOut without any options will just delete the local cache and keychain of the user. If you would like to sign out of all devices, invoke the signOut api with advanced options.

**************
**Additional resources**

[Amplify and Cognito](https://docs.amplify.aws/lib/auth/getting-started/)

**************