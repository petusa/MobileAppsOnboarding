# MobileAppsOnboarding
Guidelines with some boilerplate about how to distribute your Android and iOS mobile apps outside the stores (GooglePlay, AppStore).

Using this repository's boilerplate HTML files with the right application [configuration values](#configuration-file-appjs), you can host and share your own one pagers anywhere as static pages and share only a single link which opens up as needed on the respective Desktop/Android/iOS patforms.

The sample below shows the case when you host these pages from localhost (of course you'd better host if publicly, it is only for demo purpose): 

![Desktop page for platform specific download/install link and QR code](https://github.com/petusa/MobileAppsOnboarding/blob/master/screenshots/desktop.png)
![Android download and direct download page for HockecyApp hosted version](https://github.com/petusa/MobileAppsOnboarding/blob/master/screenshots/android_hockeyapplinks.png)
![iPhone signup page for TestFlight app](https://github.com/petusa/MobileAppsOnboarding/blob/master/screenshots/iphone_fastlaneboarding.png)

## Prerequisite

- [Android pre-requisite](instructions/android.md)
- [iOS pre-requisite](instructions/android.md)


## How to use

1. clone this repository
2. set values properly in app.js, see [configuration values](#configuration-file-appjs)
3. host the HTML files + app.js from the same folder anywhere you want (from Gtihub CDN, Google CDN, own webserver, corporeate website, etc...)
4. share the link of the index.html file with anyone who you would like to test your application


## Configuration file: app.js

