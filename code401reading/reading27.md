# Intents, Activities, SharedPreferences

## Tasks
[Notes/Images taken from this site](https://developer.android.com/guide/components/activities/tasks-and-back-stack)

- >A *task* is a collection of activities that users interact with when trying to do something in your app
- >These activities are arranged in a stack—the *back stack*—in the order in which each activity is opened.

![BackStack](https://developer.android.com/images/fundamentals/diagram_backstack.png)

- >A task is a cohesive unit that can move to the background when a user begins a new task or goes to the Home screen. While in the background, all the activities in the task are stopped, but the back stack for the task remains intact

## Key-Value Data
[Notes taken from this site](https://developer.android.com/training/data-storage/shared-preferences)

- > A `SharedPreferences` object points to a file containing key-value pairs and provides simple methods to read and write them.
- > `getSharedPreferences()` — Use this if you need multiple shared preference files identified by name, which you specify with the first parameter. You can call this from any `Context` in your app.
- `getPreferences()` — Use this from an `Activity` if you need to use only one shared preference file for the activity. Because this retrieves a default shared preference file that belongs to the activity, you don't need to supply a name.
- Example:

```Java
Context context = getActivity();
SharedPreferences sharedPref = context.getSharedPreferences(
        getString(R.string.preference_file_key), Context.MODE_PRIVATE);
```

- To write to a shared preferences file, create a `SharedPreferences.Editor` by calling `edit()` on your `SharedPreferences`.

- Example:

```Java
SharedPreferences sharedPref = getActivity().getPreferences(Context.MODE_PRIVATE);
SharedPreferences.Editor editor = sharedPref.edit();
editor.putInt(getString(R.string.saved_high_score_key), newHighScore);
editor.apply();
```

[Back to HOME](../README.md)