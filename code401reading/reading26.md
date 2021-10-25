# Android Fundamentals
[Notes were taken from this site](https://developer.android.com/guide/components/funda)

- Android apps can be written using Kotlin, Java, C++.
- *Android Package* = .apk file, contains the content that an Android app needs at runtime.
- *Androi App Bundle* = .aab file, contains the contents that an Android app does not need at runtime.
- >Each Android app lives in its own security sandbox, protected by the following Android security features:
  > - The Android operating system is a multi-user Linux system in which each app is a different user.
  > - By default, the system assigns each app a unique Linux user ID (the ID is used only by the system and is unknown to the app). The system sets permissions for all the files in an app so that only the user ID assigned to that app can access them.
  > - Each process has its own virtual machine (VM), so an app's code runs in isolation from other apps.
  > - By default, every app runs in its own Linux process. The Android system starts the process when any of the app's components need to be executed, and then shuts down the process when it's no longer needed or when the system must recover memory for other apps.
- The Android system implements the *principle of least privilege*. That is, each app, by default, has access only to the components that it requires to do its work and no more.
- 4 different types of app components:
  - Activities - interacting with the user, e.g. an email app.
  - Services - general-purpose for running in the background, e.g. a music player.
  - Broadcast Receivers - enables the system to deliver events to the app outside of a regular user flow, e.g. an alarm.
  - Content Providers - manages a shared set of app data to store somewhere, e.g. an contact list/address book.
- Your app must have a manifest file, `AndroidManifest.xml`, at the root of your project directory. This file lets the system know what components exist in your app.
- Declaring Components example:

```Java
<?xml version="1.0" encoding="utf-8"?>
<manifest ... >
    <application android:icon="@drawable/app_icon.png" ... >
        <activity android:name="com.example.project.ExampleActivity"
                  android:label="@string/example_label" ... >
        </activity>
        ...
    </application>
</manifest>
```

- Declaring Component Capabilities example:
```Java
<manifest ... >
    ...
    <application ... >
        <activity android:name="com.example.project.ComposeEmailActivity">
            <intent-filter>
                <action android:name="android.intent.action.SEND" />
                <data android:type="*/*" />
                <category android:name="android.intent.category.DEFAULT" />
            </intent-filter>
        </activity>
    </application>
</manifest>
```
- Declaring App Requirements
- App Resources

[Back to HOME](../README.md)