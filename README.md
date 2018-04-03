# cordova-plugin-local-notifications


<p align="left"><b><a href="">SAMPLE APP</a> :point_right:</b></p>

<br>

<p align="center">
    <a href="https://www.npmjs.com/package/cordova-plugin-local-notification">
        <img src="https://badge.fury.io/js/cordova-plugin-local-notification.svg" alt="npm version" />
    </a>
    <a href="https://opensource.org/licenses/Apache-2.0">
        <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg" alt="License" />
    </a>
</p>

<br>

> A notification is a message you display to the user outside of your app's normal UI. When you tell the system to issue a notification, it first appears as an icon in the notification area. To see the details of the notification, the user opens the notification drawer. Both the notification area and the notification drawer are system-controlled areas that the user can view at any time.

<br>

### Notification components

- Header area
- Content area
- Action area

### How notifications may be noticed

- Showing a status bar icon
- Appearing on the lock screen
- Playing a sound or vibrating
- Peeking onto the current screen
- Blinking the device's LED

### Supported platforms

- Android 4.4+
- iOS 10+
- Windows 10

<br>
<br>

## Important Notice

Please make sure that you always read the tagged README for the version you're using. 

See the _0.8_ branch if you cannot upgrade. Further development for `v0.9-beta` will happen here. The `0.9-dev` and `ios10` branches are obsolate and will be removed soon.

Please report bugs or missing features!


## Basics

The plugin is same as native plugin and use native object for it is `this.localNotifications` and is accessible after *deviceready* has been fired.
<br>

### Repeating

Repeat relative from now:

I am just updated plugin for repeat notification for every second, minute, hour, day, week, month, and year is extend with repeat parameter. you can use repeat parameter as per example you can set your notification.   

```js
this.localNotifications.schedule({
  id: 1,
  text: 'Single ILocalNotification',
  every: 'day',
  repeat: 2
});
```

## Installation

The plugin can be installed via [Ionic-CLI][CLI] and is publicly available on [NPM][CLI].

Execute from the projects root folder:

    $ ionic cordova plugin add cordova-plugin-local-notification

and install npm plugin :

    $ npm install --save @ionic-native/local-notifications

© 2018 [Karmdip-MI][company]

[cordova]: https://ionicframework.com/
[CLI]: https://ionicframework.com/docs/native/local-notifications/
[company]: mindinventory.com
