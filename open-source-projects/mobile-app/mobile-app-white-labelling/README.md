# Mobile App White Labelling

In this guide, we will cover how to rebrand Rocket.Chat Mobile Apps to suit your styling.

Here we will show you how to customize:

* The App Icons
* Splash Screens
* App Name
* Colors

## Important

* This document is updated after every release, so we can guarantee it's stable for production
  * `develop` branch might be different from this
* Keep in mind that you will need an **intermediate** knowledge of Android/iOS development and basic Javascript knowledge
* Our repo contains targets/build flavors to build both our Experimental and Official apps
  * Both apps are equal but released at a different pace in the stores
  * If you see an Experimental folder, don't be scared of breaking anything. It's just a folder containing the assets for the non-official app

## Repo

* Make sure you have both iOS and Google developer accounts and the respective development environments working
  * You can follow this guide: [https://reactnative.dev/docs/getting-started](https://reactnative.dev/docs/getting-started)
* Clone [https://github.com/RocketChat/Rocket.Chat.ReactNative](https://github.com/RocketChat/Rocket.Chat.ReactNative)
* Checkout `single-server` branch (git clone -b single-server [https://github.com/RocketChat/Rocket.Chat.ReactNative](https://github.com/RocketChat/Rocket.Chat.ReactNative))

## General

* Create an account on [https://www.bugsnag.com/](https://www.bugsnag.com/)
* Set `server`, `appGroup` and `appStoreId` on [app.json](https://github.com/RocketChat/Rocket.Chat.ReactNative/blob/single-server/app.json#L5)
  * `appGroup` must be the same App Group created for the iOS app
* Change app colors on [colors.ts](https://github.com/RocketChat/Rocket.Chat.ReactNative/blob/develop/app/lib/constants/colors.ts)

## Firebase

### Creating a new project on Google Cloud Platform

* Visit [https://console.cloud.google.com/home/dashboard](https://console.cloud.google.com/home/dashboard)
* By the text Google Cloud Platform there is a dropdown, open and then “Create project”
* In the dialog give a project a name then hit “Create”
* Wait until the creating process, you can follow in notifications by your avatar
* You will be redirected to the project page after creation

### Creating a new Firebase project

* Visit [https://console.firebase.google.com/](https://console.firebase.google.com/)
* Click on “Add Project”
* Enter the project name you created in the previous step
* Follow the wizard until the Firebase project is created
* We’re going to create the apps later on the tutorial page

{% content-ref url="ios-app-white-labelling.md" %}
[ios-app-white-labelling.md](ios-app-white-labelling.md)
{% endcontent-ref %}

{% content-ref url="android-app-white-labelling.md" %}
[android-app-white-labelling.md](android-app-white-labelling.md)
{% endcontent-ref %}

{% content-ref url="configuring-push-notifications.md" %}
[configuring-push-notifications.md](configuring-push-notifications.md)
{% endcontent-ref %}
