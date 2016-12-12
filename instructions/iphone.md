## How to use TestFlight and Fastlane/boarding to publish your IPA file

This description assumes that you have already an application version uploaded to [iTunesConnect](https://itunesconnect.apple.com/), and available for external testing via the [TestFlight application](https://developer.apple.com/testflight/), so it went already throught Apple's beta app review.

Since the TestFlight external testing approach needs manual one-by-one invitations by the iTunesConnect app manager (there is also a bulk upload approach, though), a better and quicker way for distributing your iPhone/iPad applications to a limited group of people (either be it in your organization, or outside), is using [Fastlane/boarding](https://github.com/fastlane/boarding)'s signup application.

Their approach can be used for testing, beta signup, or internal delivery purposes, in a neat and convenient way.

Please follow their [instructions](https://github.com/fastlane/boarding), and upload your iPhone app's automatic signup app to e.g. Heroku, and provide it's link for the [configuration](../README.me#configuration-file-appjs).



