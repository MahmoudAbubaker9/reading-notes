# Intents, Activities, and SharedPreferences

## Android Tasks and the Back Stack

A task is a collection of actions that users can perform when they try to do something in the app. The activities are organized in a stack, which is called the back stack.

### Lifecycle of a task and its back stack

1. The Home screen is the place where most tasks are started. When a user touches an icon for an app or a shortcut, that app's task appears in the foreground.

2. When an existing activity starts another, the new one is pushed on top of the stack. The old one is stopped, and the system retains the current UI state. The back stack is only used once, and only after the user has left it.

![backstack](https://developer.android.com/images/fundamentals/diagram_backstack.png)

The stack's activities are only revealed once the user has returned to the Home screen. If they are no longer needed, then the task no longer remains.

### Back press behavior for root launcher activities

* activities are activities that declare an Intent with both ACTION_MAIN and CATEGORY_LAUNCHER. are the root activities that are used to launch an app from the launcher.

* When a user presses or gestures Back from a root launcher activity, the system handles the event differently depending on the version of Android that the device is running.

**System behavior on Android 11 and lower**

The system finishes the activity.

**System behavior on Android 12 and higher** 

* The system stops working on an activity and its task when it gets too heavy. This behavior works similarly when navigating out of an app by using the Home button or a gesture.

* If you need to provide a custom back navigation method, then the AndroidX Activity APIs are the best solution. They automatically defer to the system's behavior if no components are intercepting the system's Back Press.

* If your app doesn't support onBackPressed(), call through to super.onbackPressed() instead of finishing the activity. This method returns a consistent UI experience for all app users.

### Background and foreground tasks

A task is a unit that can move from the background to the foreground when a user launches a new task. It can then return to the center when the user stops the task and proceeds to another one.


### Multiple activity instances

The back stack never gets rearranged, as if the user can start a specific activity from multiple locations. This means that if one activity is instantiated multiple times, it might get pushed to the top of the stack.

### Manage tasks

The way Android handles tasks and the back stack is by placing all the activities in succession in the same task, and in a last in, top-out stack. This method works great for most apps. However, it can also work for apps that want to implement certain behaviors.

In this regard, these are the principal <activity> attributes that you can use:

* taskAffinity
* launchMode
* allowTaskReparenting
* clearTaskOnLaunch
* alwaysRetainTaskState
* finishOnTaskLaunch

And these are the principal intent flags that you can use:

* FLAG_ACTIVITY_NEW_TASK
* FLAG_ACTIVITY_CLEAR_TOP
* FLAG_ACTIVITY_SINGLE_TOP

### Defining launch modes

1. Using the manifest file

When you declare an activity in your manifest file, you can specify how the activity should associate with tasks when it starts.

2. Using Intent flags

When you call startActivity(), you can include a flag in the Intent that declares how (or whether) the new activity should associate with the current task.


## Save key-value data 

If you have a few key-values that you would like to save, then the SharedPreferences API is for you. It simplifies the work of creating key-value pairs by pointing to a file that contains them.

You can create a new shared preference file or access an existing one by calling one of these methods:


1. getSharedPreferences() — if you need multiple shared preference files identified by name, which you specify with the first parameter. You can call this from any Context in your app.

2. getPreferences() — If an Activity has multiple shared preference files, this method will retrieve one of them. You do not need to supply a name.



**************
[Tasks and the back stack - source site](https://developer.android.com/guide/components/activities/tasks-and-back-stack)

[Save key-value data - source site](https://developer.android.com/training/data-storage/shared-preferences)

**************
