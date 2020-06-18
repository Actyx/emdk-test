# Multitasking test with EMDK library on the Zebra TC8000

When the EMDK library is not used the activity that is started with the action button will spawn a new task which is accessible in the task switcher. This is enabled by the `android:documentLaunchMode="intoExisting"` property. With the EMDK the activity will be opened in the current task.

Remove the `<uses-library>` tag in `AndroidManifest.xml` to make it work again. On all other devices/emulators tested it works without modification.
