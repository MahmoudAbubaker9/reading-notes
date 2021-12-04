# Intent Filters

* Intent filter is a property that used in your app to allow other apps use a feature of your app and It is added in the manifest file if you want to use it


# Allowing Other Apps to Start Your Activity

* To allow other apps to start your activity in this way, you need to add an `<intent-filter>` element in your manifest file for the corresponding `<activity>` element.

* When your app is installed on a device, the system identifies your intent filters and adds the information to an internal catalog of intents supported by all installed apps. When an app calls `startActivity()` or `startActivityForResult()`, with an implicit intent, the system finds which activity (or activities) can respond to the intent.


* The system may send a given Intent to an activity if that activity has an intent filter fulfills the following criteria of the Intent object:

1. Action : Usually one of the platform-defined values such as ACTION_SEND or ACTION_VIEW.
2. Data : A description of the data associated with the intent.
3. Category : usually related to the user gesture or location from which it's started ,all implicit intents are defined with CATEGORY_DEFAULT by default.

## Handle the Intent in Your Activity

```java
@Override
protected void onCreate(Bundle savedInstanceState) {
    super.onCreate(savedInstanceState);

    setContentView(R.layout.main);

    // Get the intent that started this activity
    Intent intent = getIntent();
    Uri data = intent.getData();

    // Figure out what to do based on the intent type
    if (intent.getType().indexOf("image/") != -1) {
        // Handle intents with image data ...
    } else if (intent.getType().equals("text/plain")) {
        // Handle intents with text ...
    }
}

```

## Return a Result

```java
// Create intent to deliver some kind of result data
Intent result = new Intent("com.example.RESULT_ACTION", Uri.parse("content://result_uri"));
setResult(Activity.RESULT_OK, result);
finish();
```