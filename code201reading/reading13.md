# Reading Notes 13 - Local Storage

## Local Storage
- Native applications can use a registry, INI files, XML files, or databases for local storage.
- Web applications can use cookies but it does have some downsides:
  - Cookies are in every HTTP request, causing slowdown.
  - Can send unencrypted data.
  - limited to about 4KB of data.
- Various solutions to local storage have been used in the past (DHTML/userData, Flash cookies, Gears, etc)

## HTML Storage
- Stores named key/value pairs locally within the browser.
- Unlike cookies, this data is never sent to a remote web server unless manually told to do so.
- Most modern browsers support HTML5 Storage.
- Access HTML5 Storage through the ***localStorage*** object in JavaScript.
- Named key = string.
- data value = any data type supported by JavaScript (Boolean, Number, String, etc).
- Howeever the data is stored as a string. Use `parseInt()` or `parseFloat()`.
- You treat `localStorage` as an object using the square bracket syntax.
- default storage limit of 5 megabytes.

[Back to HOME](../README.md)