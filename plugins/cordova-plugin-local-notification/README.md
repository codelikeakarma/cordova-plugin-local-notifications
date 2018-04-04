# cordova-plugin-local-notifications

> A notification is a message you display to the user outside of your app's normal UI. When you tell the system to issue a notification, it first appears as an icon in the notification area. To see the details of the notification, the user opens the notification drawer. Both the notification area and the notification drawer are system-controlled areas that the user can view at any time.

## Installation

The plugin can be installed via [Ionic-CLI][ionicPluginCLI] and is publicly available on [NPM][CLI].

Please replace your folder with this repository as per directory map.

Find the Native plugin of local notification form [here][CLI].

**Install ionic cordova plugin :**

    $ ionic cordova plugin add cordova-plugin-local-notification

**Install ionic native npm plugin :**

    $ npm install --save @ionic-native/local-notifications

## Notification components

- Header area
- Content area
- Action area

## How notifications may be noticed

- Showing a status bar icon
- Appearing on the lock screen
- Playing a sound or vibrating
- Peeking onto the current screen
- Blinking the device's LED

## Supported platforms

- Android 4.4+

## Important Notice

- Please make sure that you always read the tagged README for the version you're using.
- Please report bugs or missing features!
- It's only available for Android and soon update for iOS.

## Basics
- The plugin is same as native plugin and use native object for same i.e. `localNotifications` and is accessible after *deviceready* has been fired.

## Repeating Interval

Repeat relative from now:

It is using for The interval at which to reschedule the local notification. That can be a value of second, minute, hour, day, week, month or year.

Just you are adding a parameter to extend your interval time of your local notification.

```
interval: number // integer number only.
```

Below given an example for sending notification every 2 days. You may update the interval time as per your requirement.

```js
this.localNotifications.schedule({
  id: 1, // id of your notification
  title: 'Local Notification', // title of your notification.
  text: 'Repeat notification', // message of your notification.
  every: 'day', // it's every second, minute, hour, day, month and year parameter to repeat your notification.
  interval: 2 // it's for repeat your notification in timespan Ex. you are using 2 then it's triggerd your notification at every 2 days.
});
```

### Thanks for your support.



© 2018 [Mindinventory][company]

[cordova]: https://ionicframework.com/
[CLI]: https://ionicframework.com/docs/native/local-notifications/
[ionicPluginCLI]: https://ionicframework.com/docs/cli/cordova/plugin/
[company]: https://www.mindinventory.com/