# MobileAppsOnboarding
Guidelines with some boilerplate about how to distribute your Android and iOS mobile apps outside the stores (GooglePlay, AppStore).

Using this repository's boilerplate HTML files with the right application [configuration values](#configuration-file-appjs), you can host and share your own one pager installers anywhere as static pages and share only a single link which opens up as needed on the respective Desktop/Android/iOS patforms.

---

The sample below shows the case when you host these pages from localhost (of course you'd better host if publicly, it is only for demo purpose): 

![Desktop page for platform specific download/install link and QR code](https://github.com/petusa/MobileAppsOnboarding/blob/master/screenshots/desktop.png)

This is what your mobile browser will show, when you open/scan this link from your Android or iPhone:

![Android download and direct download page for HockecyApp hosted version](https://github.com/petusa/MobileAppsOnboarding/blob/master/screenshots/android_hockeyapplinks.png)

![iPhone signup page for TestFlight app](https://github.com/petusa/MobileAppsOnboarding/blob/master/screenshots/iphone_fastlaneboarding.png)

## Prerequisite

I our case, we simply use now [HockeyApp](https://www.hockeyapp.net/) for hosting our Android app's APK file, with direct download possibility:

- [Android pre-requisite](instructions/android.md)

We use [iTunesConnect](https://itunesconnect.apple.com/) with [TestFlight application](https://developer.apple.com/testflight/) to host and distribute the properly signed iPhone IPA file. We also use the [Fastlane/boarding](https://github.com/fastlane/boarding) automatic signup approach for easier TestFlight onboarding:

- [iOS pre-requisite](instructions/iphone.md)

Of ourse there might be different distribution and App hosting approaches, too.

## How to use

1. clone this repository
2. set values properly in app.js, see [configuration values](#configuration-file-appjs)
3. host the HTML files + app.js from the same folder anywhere you want (from Gtihub CDN, Google CDN, own webserver, corporeate website, etc...)
4. share the link of the index.html file with anyone who you would like to test your application


## Configuration file: app.js

**Values:**
- `name` Set this to your application name
- `image_url` Set this to your application image (can be either Android/iOS application icon's full URL from e.g. TestFlight/HockeyApp)
- `description` Set a description for your application
- `android_hockey_app_url` Set this to your app's Hockey hosted Android public page link, seen here ([Android pre-requisite](instructions/android.md))
- `android_hockey_app_download_url` Set this to your app's Hockey hosted Android public page download link, seen here ([Android pre-requisite](instructions/android.md))
- `ios_auto_boarding_url` Set this to the iPhone version, TestFlight app's automatic signup page link, seen here ([Android pre-requisite](instructions/iphone.md))
