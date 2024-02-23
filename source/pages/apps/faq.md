---
layout: ~/layouts/MarkdownLayout.astro
title: Frequently Asked Questions
---

# Frequently Asked Questions

*See the page of each app for app-specific FAQs.*

### How can I report a bug or suggest a feature?

Tap the feedback button in the app or the support link on the app's page. I prioritize bug fixes and consider feature suggestions that align with the app's vision and user demand.

### How can I get a refund?

For apps purchased on the Apple App Store, you can [request a refund](https://support.apple.com/en-us/HT204084). However, I would appreciate if you [reached out](/feedback) first. I may be able to resolve any problems you are having.

### Do your apps collect any personal data?

My apps prioritize user privacy and do not collect any personal data.

### Are your apps native?

Yes, all my apps are native. They are built using Swift and SwiftUI and are designed to provide the best performance and integration with the operating systems. I put a lot of effort into adhering to Apple's [Human Interface Guidelines](https://developer.apple.com/design/human-interface-guidelines).

### Why are most of your apps free?

I love making apps and I want them to be available to as many people as possible. I don't care much about money and I earn enough on my paid apps.

### What's your policy on ads in your apps?

I hate ads. None of my apps have ads.

### How can I support your work?

Rate and review my apps on the App Store. Your ratings and reviews greatly aid in increasing the apps' visibility and discoverability, helping more users find them.

### Who makes your app icons?

I make them myself in Sketch, sometimes using AI as a starting point.

### How do you prioritize bug fixes?

User-reported bugs are prioritized based on their impact on the app's functionality and the number of users affected. My goal is to fix **all** bugs.

### What's the best way to learn about new apps?

Subscribe to my [“new apps” RSS feed](/rss-apps.xml) and follow me on [Twitter](https://twitter.com/sindresorhus) and [Mastodon](https://mastodon.social/@sindresorhus).

### Do you actively maintain all your apps?

Yes, I actively maintain all my apps to ensure they remain awesome and bug free. Every year, I make sure they take advantage of Apple's latest technologies.

### The app hasn't been updated in a while, is it still maintained?

Yes, if an app has not been updated for months, it's still actively maintained. A lack of recent updates indicates that the app has reached a mature and stable state.

### Why do you only support the latest macOS/iOS version?

I make apps for fun and supporting older operating system versions is simply no fun. It adds a lot of overhead with having to test each update on the older versions, work around bugs Apple will never fix, etc. As a compromise, I provide older versions of my apps for older operating system versions.

### How can I export, import, sync, or back up the settings in a Mac app?

[See this guide.](https://github.com/sindresorhus/guides/blob/main/backup-app-settings.md)

### Can I contribute localizations to your apps?

No, I don't plan to localize my apps. Localization adds complexity and maintenance demands that detract from my focus on app quality and performance.

### You are doing a lot of open source, why are only some of your apps open source? {#why-not-oss}

I open source [some of my apps](https://github.com/search?q=user%3Asindresorhus+language%3Aswift+topic%3Aapp+archived%3Afalse), but not all, for a few key reasons. First, I use specialized tools (internal framework) to speed up app development, which are not suitable for sharing. Additionally, past experiences with open sourcing apps have led to clones of my apps appearing on the App Store, which is problematic. Also, community contributions, though well-intentioned, often don't match the high quality standards I set for my apps. As a compromise, I tend to open source the [reusable building blocks](https://github.com/search?q=user%3Asindresorhus+topic%3Aswift-package+archived%3Afalse), allowing community involvement while maintaining the quality and uniqueness of my apps.

### I'm having a problem with your app {#app-problem}

Here are some things you could try:

- Restart your device.
- Ensure you are on the latest version of the app.
- Ensure you are on the latest operating system version.
- Check the FAQ on the app's page in case it's already answered there.
- If the app requires an internet connection, make sure you are online. Try disabling any VPN.
- macOS: Close all other apps (including menu bar items) to make sure the problem is not caused by another app.
- macOS: [Reset permissions.](#mac-reset-permissions)
- [Reset the app.](#reset-app)

If you have tried all of this, [contact me](/feedback).

### How can I send you debug info for one of your Mac apps? {#mac-debug-info}

Make sure the app is not running (you can force-quit it from the Activity Monitor app) and then press <kbd>Shift</kbd>+<kbd>Control</kbd>+<kbd>Option</kbd> while launching the app.

### How can I delete all settings and data to start over in one of your apps? {#reset-app}

iOS: Open the Settings app, go to “General › iPhone/iPad Storage”, tap the app in the list, tap “Delete App”, then go to the App Store and install the app again.

macOS: Make sure the app is not running (you can force-quit it from the Activity Monitor app) and then press <kbd>Shift</kbd>+<kbd>Control</kbd>+<kbd>Option</kbd>+<kbd>Command</kbd> while launching the app.

### How can I reset all permissions for your Mac app? {#mac-reset-permissions}

*(This is only necessary if the app asked for any permissions the first time you launched it)*

First, quit the app.

Copy the following, open the Terminal app, paste it into the Terminal window, replace `<app-name>` with the name of the app, and then press the <kbd>Return</kbd> key:

```sh
osascript -e 'id of app "<app-name>"'
```

Example:

```sh
osascript -e 'id of app "Dato"'
```

You now have the app's identifier.

Next, copy the following, and paste it into the Terminal window, replace `<app-identifier>` with the app's identifier, and then press the <kbd>Return</kbd> key:

```sh
tccutil reset All <app-identifier>
```

Example:

```sh
tccutil reset All com.sindresorhus.Dato
```

You can now launch the app again.

### How can I send you a crash report for one of your Mac apps? {#crash-report}

- Open Finder
- Select `Go to Folder…` from the `Go` menu
- Enter: `~/Library/Logs/DiagnosticReports`
- In the resulting list, select all files that starts with the app name, ZIP them, and [send me](/feedback)

### Can you support non-Apple platforms?

No, my expertise is exclusively in macOS, iOS, watchOS, and visionOS. Focus is key to high-quality apps.

### Can I hire you to build me an app?

I am not available for hire.

### Can I acquire your app?

No. I make apps because I enjoy it. Your money is of no interest to me.

### My question is not answered here

[Ask me.](/contact)

*You could also try to [ask my AI bot](https://chat.openai.com/g/g-df0ZoBF9N-sindregpt).*
