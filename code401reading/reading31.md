# Espresso
[Notes taken from this site](https://developer.android.com/training/testing/espresso)

- Espresso can be used to write tests for Android UI
- Example code:

```Java
@Test
public void greeterSaysHello() {
    onView(withId(R.id.name_field)).perform(typeText("Steve"));
    onView(withId(R.id.greet_button)).perform(click());
    onView(withText("Hello Steve!")).check(matches(isDisplayed()));
}
```

## Packages

- `espresso-core` - Contains core and basic `View` matchers, actions, and assertions. See Basics and Recipes.
- `espresso-web` - Contains resources for `WebView` support.
- `espresso-idling-resource` - Espresso's mechanism for synchronization with background jobs.
- `espresso-contrib` - External contributions that contain `DatePicker`, `RecyclerView` and `Drawer` actions, accessibility checks, and `CountingIdlingResource`.
- `espresso-intents` - Extension to validate and stub intents for hermetic testing.
- `espresso-remote` - Location of Espresso's multi-process functionality.

## Creating UI Tests with Espresso Test Recorder
[Notes taken from this site](https://developer.android.com/studio/test/espresso-test-recorder)

- Espresso Test Recorder lets you recorder your interactions with your app without having to write any code.
- Before using Espresso Test Recorder, make sure to turn off animations.
- Espresso tests consist of two primary components: UI interactions and assertions on View elements.
- > To start recording a test with Espresso Test Recorder, proceed as follows:
  > 1. Click **Run** > **Record Espresso Test**.
  > 2. In the **Select Deployment Target** window, choose the device on which you want to record the test. If necessary, create a new Android Virtual Device. Click **OK**.
  > 3. Espresso Test Recorder triggers a build of your project, and the app must install and launch before Espresso Test Recorder allows you to interact with it. The **Record Your Test** window appears after the app launches, and since you have not interacted with the device yet, the main panel reads "No events recorded yet." Interact with your device to start logging events such as "tap" and "type" actions.
- Add assertations to verify UI elements.
- Save your recording.
- >Once you finish interacting with your app and adding assertions, use the following steps to save your recording and generate the Espresso test:
  > 1. Click **Complete Recording**. The **Pick a test class name for your test** window appears.
  > 2. Espresso Test Recorder gives your test a unique name within its package based on the name of the launched activity. Use the **Test class name** text field if you want to change the suggested name. Click **Save**.
  > 3. The file automatically opens after Espresso Test Recorder generates it, and Android Studio shows the test class as selected in the **Project** window of the IDE.

[Back to HOME](../README.md)