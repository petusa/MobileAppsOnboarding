## How to use TestFlight and Fastlane/boarding to publish your IPA file

This description assumes that you have already an application version uploaded to [iTunesConnect](https://itunesconnect.apple.com/), and available for external testing via the [TestFlight application](https://developer.apple.com/testflight/), so it went already through Apple's beta app review.

Since the TestFlight external testing approach needs manual one-by-one invitations by the iTunesConnect app manager (there is also a bulk upload approach, though), a better and quicker way for distributing your iPhone/iPad applications to a limited group of people (either be it in your organization, or outside), is using [Fastlane/boarding](https://github.com/fastlane/boarding)'s signup application.

Their approach can be used for testing, beta signup, or internal delivery purposes, in a neat and convenient automatic way, instead of manually adding one by one each and every potential testers.

1. Please follow their [instructions](https://github.com/fastlane/boarding) to deploy your iPhone app's automatic signup app to e.g. Heroku, 
2. after that provide the deployer Heroku app's link for the [configuration](../README.md#configuration-file-appjs), to use these with the boilerplpates HTML pages with [Petusa/MobileAppsOnboarding](https://github.com/petusa/MobileAppsOnboarding).
