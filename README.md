# FireSmartLamp-Android
Android app for controlling a Smart Lamp. It's the Android client of this Smart Lamp project https://github.com/andriyadi/FireSmartLamp.
Make sure to deploy that Smart Lamp project successfully first before using this app.

##Run the app
If you already deployed that Smart Lamp project, you should already have Firebase app. Make note of Firebase app name (or project id).

Then in `DeviceActivity.java` file, on line 50, change `[YOUR_OWN_FIREBASE_APP]` to your Firebase app name/project id retrieved above.

If the app run successfully, you'll have something like this:

![Screen](https://github.com/andriyadi/FireSmartLamp-Android/blob/master/ScreenCap.png)

Notice that the app will first try to retrieve latest device object from Firebase and apply `parameters` object values to related controls (buttons and progress bar).
By that, if for example, the smart lamp is currently ON, the switch button will be ON as well. Then tap on it once will make the lamp OFF.

Sliding progress bar at the bottom is supposed to change the actual brightness/dim level of the lamp. But the implementation of dimming is not yet done on the Smart Lamp side. Maybe you wanna do it? Please do :)

That's it. Enjoy.

