# Espresso

Espresso is a testing framework for Android to make it easy to write reliable user interface tests

## Synchronization capabilities

**the following synchronization conditions are met:**

1. The message queue is empty.
2. There are no instances of AsyncTask currently executing a task.
3. All developer-defined idling resources are idle.

## Packages

* `espresso-core` Contains core and basic View matchers, actions, and assertions. See Basics and Recipes.
* `espresso-web` Contains resources for WebView support.
* `espresso-idling-resource` Espresso's mechanism for synchronization with background jobs.
* `espresso-contrib` External contributions that contain DatePicker, RecyclerView and Drawer actions, accessibility checks, and CountingIdlingResource.
* `espresso-intents` Extension to validate and stub intents for hermetic testing.
* `espresso-remote` Location of Espresso's multi-process functionality.

## Ridiculous superpower: the Espresso Test Recorder

* The Espresso Test Recorder tool lets you create UI tests for your app without writing any test code.

* By recording a test scenario, you can record your interactions with a device and add assertions to verify UI elements in particular snapshots of your app.

* Espresso Test Recorder then takes the saved recording and automatically generates a corresponding UI test that you can run to test your app.

* **note** : Before using Espresso Test Recorder, make sure you turn off animations on your test device to prevent unexpected results.


## Record an Espresso test

1. **Espresso tests consist of two primary components**

1. UI interactions and assertions on View elements
2. UI interactions include tap and type actions that a person may use to interact with your app

2. **Record an Espresso test**

```
1. Click Run > Record Espresso Test.

2. In the Select Deployment Target window, choose the device on which you want to record the test.

3. Recorded interactions will appear in the main panel in the Record Your Test window, When you run the test, the Espresso test will try executing these actions in the same order.

```

3. **Add assertions to verify UI elements**

```
1. Click Add Assertion.
2. To select a View element on which to create an assertion, click on the element in the screenshot or use the first drop-down menu in the Edit assertion box at the bottom of the window.
3. Select the assertion you want to use from the second drop-down menu in the Edit assertion box.
4. Click Save and Add Another to create another assertion or click Save Assertion to close the assertion panels.
```

4. **Save a recording**
```
1. Click Complete Recording.
2. Use the Test class name text field if you want to change the suggested name. Click Save.
3. Android Studio shows the test class as selected in the Project window of the IDE.
```


**************
**Additional resources**

[Espresso Testing](https://developer.android.com/training/testing/espresso)

[Ridiculous superpower: the Espresso Test Recorder](https://developer.android.com/studio/test/espresso-test-recorder)
**************