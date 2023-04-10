# Mobile App FAQs

<details>

<summary>Why am I not receiving push notifications on mobile apps?</summary>

First, please make sure you understand our Push Notification workflow, and the app should be receiving a push notification. If you're using [Rocket.Chat SaaS](https://docs.rocket.chat/rocket.chat-saas/cloud-account), make sure you have enough Push Notification quota. If you're self-hosted, make sure your gateway is properly configured.

</details>

<details>

<summary><strong>Will</strong> <strong>Rocket.Chat</strong> <strong>push notification gateway work on my Whitelabel app?</strong></summary>

No, Rocket.Chat gateway works only for Rocket.Chat apps on the stores. You'll need to [configure push notification](mobile-app-white-labelling/configuring-push-notifications.md) on your server.

</details>

<details>

<summary>Do I need previous knowledge to build a white-label app?</summary>

Yes, you'll need intermediate iOS and Android experience to be able to build and upload your apps to the stores.

</details>

<details>

<summary>Why is Bugsnag required to build my white-label app?</summary>

Every app should contain some level of error tracking so you can find issues happening and fix them.\
If you find any bugs on your app built from the source, you can contribute back to the community or open a new issue on our [Github Repository](https://github.com/RocketChat/Rocket.Chat.ReactNative/), and we can fix them on an upcoming version of the app.\
A bug might be caused during the white-label process, so it's important to be aware. If you know the risks and still want to remove Bugsnag from your app, you can follow their [installation guide](https://docs.bugsnag.com/platforms/react-native/react-native/#installation-and-configuration), but undo everything. Additionally, if you think we should remove the Bugsnag dependency from our project, let us know by [filing an issue](https://github.com/RocketChat/Rocket.Chat.ReactNative/issues/new), and we're happy to discuss it with you further!

</details>

<details>

<summary>The "single-server" branch is outdated. When is it going to be updated?</summary>

We always keep the white-label up-to-date to the [Rocket.Chat](http://rocket.chat) apps on App Store and Google Play. Once a new version is released, we update it to match the new content.

</details>
