# Android Fundamentals

Android apps can be written in various languages, such as Java, Kotlin, and C++. The Android SDK tools help developers create apps that run smoothly on Android devices.

* An Android package (.apk) is a directory containing the contents of an Android app, which are required to run.

* An Android App Bundle (.aab) is an archive file that contains the contents of a project, without requiring any additional metadata to be installed on Android devices.

### Each Android app lives in its own security sandbox, protected by the following Android security features:

1. The Android operating system is a multi-user Linux system in which each app is a different user.


2. The system assigns each app a unique user ID. The user ID is used only by that system and is not known to the app.

3. Each process has its own virtual machine (VM)

**The Android system has a principle that gives each app the least privilege to access the components that it needs to do its work. This ensures that the system is secure.**

* It's possible to share a Linux user ID with two apps. They can then access each other's files and run in the same Linux process.

* A permissions request is a request to access a specific device's data. The user must explicitly grant the app permission to access the data.

### App components

There are four different types of app components :

1. Activities : An activity is the entry point for interacting with the user. It represents a single screen with a user interface.

2. Services : keeping an app running in the background for all kinds of reasons

3. Broadcast receivers : component deliver events to the app outside of a regular user flow and allowing the app to respond to system-wide broadcast announcements.

4. Content providers : manage data that you can store

```
There are separate methods for activating each type of component:

You can start an activity or give it something new to do by passing an Intent to startActivity() or startActivityForResult() (when you want the activity to return a result).
With Android 5.0 (API level 21) and later, you can use the JobScheduler class to schedule actions. For earlier Android versions, you can start a service (or give new instructions to an ongoing service) by passing an Intent to startService(). You can bind to the service by passing an Intent to bindService().
You can initiate a broadcast by passing an Intent to methods such as sendBroadcast(), sendOrderedBroadcast(), or sendStickyBroadcast().
You can perform a query to a content provider by calling query() on a ContentResolver.
```

### The manifest file

AndroidManifest.xml is a file that has the configuration of the app such as:
User permissions.
The API Level required by the app.
Hardware and software features.
API libraries the app needs to be linked to API.

[resources](https://developer.android.com/guide/components/fundamentals)


