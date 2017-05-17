# TODO #

## Lesson 1 ##

### 1. Welcome to Developing Android Apps ###

* [Android Sample Code](http://developer.android.com/samples/index.html?utm_source=udacity&utm_medium=mooc&utm_term=android&utm_content=L1_Welcome_Samples&utm_campaign=training\)
* [Android Developer Site](http://developer.android.com/?utm_source=udacity&utm_medium=mooc&utm_term=android&utm_content=L1_Welcome_DAC&utm_campaign=training\)
* [Android Developers on Google+](http://plus.google.com/+AndroidDevelopers/)
* [Android Developers on Twitter](http://www.twitter.com/AndroidDev/)
* [Android Questions on Stack Overflow](http://stackoverflow.com/questions/tagged/android/)

### 2. Introducing Your Instructors ###

You don't have to take Katherine's word for it - you can see some of her impressive coding abilities in action by downloading [Google Keep](https://play.google.com/store/apps/details?id=com.google.android.keep) from Google Play. It's got 4.5 stars and over 10 million downloads, so you know she's legit.

Reto really has been around since the very early days of Android, writing this [historical getting started guide](http://blogoscoped.com/archive/2007-11-19-n27.html) a week after the first beta Android SDK was released.

### 7. The Code And Videos ###

#### The Directory Structure of Android Studio ####

More in-depth information can be found [here](https://developer.android.com/tools/projects/index.html).

#### The GitHub Codebase ####

If you’re not comfortable with GitHub or Git you can learn more about both [here](https://www.udacity.com/course/ud775).

### 8. Starter Code ###

Since you haven't learned about [Activities](http://developer.android.com/guide/components/activities.html) or [Fragments](http://developer.android.com/guide/components/fragments.html), it's okay if you're not familiar with some of the concepts discussed.

### 9. Create a New Android Studio Project ###

Find the Android Studio Installation and Setup Guides for Windows and Mac in our [How to Install Android Studio mini-course](https://www.udacity.com/course/ud808).

Don't forget you can check out [Android Studio installation instructions on the developer site](http://developer.android.com/sdk/installing/studio.html) and the [Android Studio known issues](http://tools.android.com/knownissues) if you're having trouble translating what's in the video to what's in your IDE.

### 10. Select A Minimum And Target SDK ###

The graph shown in this video is already out of date - check out the [Android Platform Version Distribution dashboard](http://developer.android.com/about/dashboards/index.html?utm_source=udacity&utm_medium=mooc&utm_term=android&utm_content=platform_distribution&utm_campaign=training) to get the latest distributions.

Learn more about the specific features released in each version of Android by reviewing the [Android version history](http://en.wikipedia.org/wiki/Android_version_history).

### 11. Select a Target SDK ###

In order to provide a great experience for as many users as possible, use the [Support Library](http://developer.android.com/tools/support-library/features.html?utm_source=udacity&utm_medium=mooc&utm_term=android&utm_content=support_library&utm_campaign=training) to use features from newer platform releases on devices running older versions and review the [Android Platform Version Distribution dashboard](http://developer.android.com/about/dashboards/index.html?utm_source=udacity&utm_medium=mooc&utm_term=android&utm_content=platform_distribution&utm_campaign=training) to get the latest platform distribution numbers.

### 12. Finish Creating a New Project ###

Here are two links to Google documentation on creating Fragments: one is titled [Creating Fragments](https://developer.android.com/training/basics/fragments/creating.html) and the other is just titled [Fragments](https://developer.android.com/guide/components/fragments.html).

### 13. Launch Sunshine And Create An AVD ###

The Android Developer site has more details for [Managing Virtual Devices](http://developer.android.com/tools/devices/index.html?utm_source=udacity&utm_medium=mooc&utm_term=android&utm_content=managing_avd&utm_campaign=training) and using the [Android Debug Monitor](http://developer.android.com/tools/debugging/ddms.html?&utm_content=ddms&utm_campaign=training) to control emulators.

### 14. Android Software Stack And Gradle ###

[Gradle](http://gradle.org/) is a sophisticated build system that lets you use a simple, declarative DSL to configure the build process of your app. For more info, check out Udacity's [Gradle for Android and Java course](https://classroom.udacity.com/courses/ud867/lessons/3968239469/concepts/42836685960923)!

You can find out [more about the Android build system here](http://tools.android.com/tech-docs/new-build-system), or by watching Xavier Ducrohet [describe the new Android SDK build system](https://www.youtube.com/watch?v=LCJAgPkpmR0) at Google I/O 2013.

If you're a hardcore command-line guru, be sure to read up on the [Android Debug Bridge (ADB)](http://developer.android.com/tools/help/adb.html?utm_source=udacity&utm_medium=mooc&utm_term=android&utm_content=adb&utm_campaign=training) and other [command line tools](http://developer.android.com/tools/index.html?utm_source=udacity&utm_medium=mooc&utm_term=android&utm_content=tools&utm_campaign=training). You can also find out more about the Android Virtual Machines [ART](https://source.android.com/devices/tech/dalvik/art.html) and [DART](http://source.android.com/devices/tech/dalvik/) to see how the Android Runtime works under the covers.

You may need to run chmod +x on gradlew before you can run it. See this [link](https://developer.android.com/sdk/installing/studio-build.html#buildCmd) for more detailed instructions.

### 15. Setup Your Device ###

Setting up USB debugging on some operating systems can be a little more complicated than Katherine demonstrated - check out this guide on [Using Hardware Devices](http://developer.android.com/tools/device.html#setting-up?utm_source=udacity&utm_medium=mooc&utm_term=android&utm_content=dev_mode&utm_campaign=training) for debugging to learn more if you run into trouble.

### 16. Launching On A Device ###

#### Command Line Tool Commands ####

The usage of these commands is entirely optional. The result is that same as clicking the Run button in Android Studio.

* chmod +x gradlew - This command only needs to be run once and is used to give gradlew the correct execute permissions.
* ./gradlew assembleDebug - This command will compile the code.
* adb install -r app/build/outputs/apk/app-debug-unaligned.apk - This command will install the APK. With the -r flag it will overwrite any prior installed versions. Note if you have more than one device, you will need to use the -s flag right after adb to specify the serial number of the intended device.
* adb shell am start -n com.example.android.sunshine.app/com.example.android.sunshine.app.MainActivity - This command will actually run the app.

If you're all about the command-line, check out these links to find out more about using the [Android Debug Bridge (ADB)](http://developer.android.com/tools/help/adb.html?utm_source=udacity&utm_medium=mooc&utm_term=android&utm_content=adb&utm_campaign=training) and [building with Gradle](http://developer.android.com/sdk/installing/studio-build.html?utm_source=udacity&utm_medium=mooc&utm_term=android&utm_content=studio_gradle&utm_campaign=training).

### 19. Create A User Interface ###

The [Activity](http://developer.android.com/guide/components/activities.html) class that Dan's extending with MainActivity is the screen, or window, that's used to display a visual user interface to our users.

### 20. UI Element Quiz ###

As Dan says, the Visual Layout Editor is a powerful tool for creating layouts. You can find out more tips on using it in this guide to [using the Layout Editor](https://developer.android.com/sdk/installing/studio-layout.html?utm_source=udacity&utm_medium=mooc&utm_term=android&utm_content=l1_visual_layout_editor&utm_campaign=training).

### 24. Responsive Design Thinking ###

To learn more about Responsive Design in Android, check out some of Google's Android Design Advocates as they discuss various elements of Android Design in this episode of [Android Design in Action](https://www.youtube.com/watch?v=zHirwKGEfoE?utm_source=udacity&utm_medium=mooc&utm_term=android&utm_content=l1_ADIA&utm_campaign=training).

You can find lots more Android design tips from the full [Android Design in Action playlist](https://www.youtube.com/playlist?list=PLWz5rJ2EKKc8j2B95zGMb8muZvrIy-wcF&utm_source=udacity&utm_medium=mooc&utm_term=android&utm_content=l1_ADIA_playlist&utm_campaign=training).

### 25. Layout Managers ###

* [Linear Layout](http://developer.android.com/guide/topics/ui/layout/linear.html?utm_source=udacity&utm_medium=mooc&utm_term=android&utm_content=l1_linear&utm_campaign=training)
* [Relative Layout](http://developer.android.com/guide/topics/ui/layout/relative.html?utm_source=udacity&utm_medium=mooc&utm_term=android&utm_content=l1_relative&utm_campaign=training)

As Dan mentioned, each of these Layout Managers extends the [View Group](http://developer.android.com/reference/android/view/ViewGroup.html?utm_source=udacity&utm_medium=mooc&utm_term=android&utm_content=l1_viewgroup&utm_campaign=training) class.

### 26. ScrollViews Vs ListViews ###

* [Scroll View](http://developer.android.com/reference/android/widget/ScrollView.html?utm_source=udacity&utm_medium=mooc&utm_term=android&utm_content=l1_scrollview&utm_campaign=training)
* [ListView](http://developer.android.com/guide/topics/ui/layout/listview.html?utm_source=udacity&utm_medium=mooc&utm_term=android&utm_content=l1_listview&utm_campaign=training)

We'll explore the ListView in more detail throughout the course, but if you really want to understand some of what's possible with this control, you should watch [The World of ListView](https://www.youtube.com/watch?v=wDBM6wVEO70?utm_source=udacity&utm_medium=mooc&utm_term=android&utm_content=l1_listview_youtube&utm_campaign=training) from Google I/O 2010.

### 28. Add ListView To Layout ###

These are the base [layout parameters](http://developer.android.com/reference/android/view/ViewGroup.LayoutParams.html?utm_source=udacity&utm_medium=mooc&utm_term=android&utm_content=l1_layoutparams&utm_campaign=training), which should be applied to every View in your layouts.

### 30. Adapters ###

* [Adapters](http://developer.android.com/reference/android/widget/Adapter.html?utm_source=udacity&utm_medium=mooc&utm_term=android&utm_content=l1_adapters&utm_campaign=training)
* [AdapterViews](http://developer.android.com/guide/topics/ui/declaring-layout.html#AdapterViews)

We'll learn more about [building layouts with an adapter](http://developer.android.com/guide/topics/ui/declaring-layout.html#AdapterViews?utm_source=udacity&utm_medium=mooc&utm_term=android&utm_content=l1_adapterview&utm_campaign=training) as we continue creating Sunshine.

### 31. Initialize The Adapter ###

Katherine is using an [ArrayAdapter](http://developer.android.com/reference/android/widget/ArrayAdapter.html?utm_source=udacity&utm_medium=mooc&utm_term=android&utm_content=l1_array_adapter&utm_campaign=training).

You can see an [example of an ArrayAdapter](http://developer.android.com/guide/topics/ui/declaring-layout.html#FillingTheLayout) in the Android documentation.

This is the first time you've encountered the magic R files. It's not really magic. Check out this [guide](http://developer.android.com/guide/topics/resources/accessing-resources.html) for more info!

### 32. Finding Views FindViewById() ###

Because we're creating all our layouts in XML, it's important to understand how you can get a reference to those Views within your code. That means you'll be making a lot of calls to [findViewById](http://developer.android.com/reference/android/view/View.html#findViewById(int)?utm_source=udacity&utm_medium=mooc&utm_term=android&utm_content=l1_findviewbyid&utm_campaign=training).

## Lesson 2 ##

### 2. Review Data Provided By Open Weather Map ###

* [API key](https://home.openweathermap.org/api_keys) - Sign In
* [API calls examples](http://openweathermap.org/current)

### 4. Find The Query We Want ###

Katherine's solution: [http://api.openweathermap.org/data/2.5/forecast/daily?q=94043&mode=json&units=metric&cnt=7](http://api.openweathermap.org/data/2.5/forecast/daily?q=94043&mode=json&units=metric&cnt=7)

### 6. HTTP Requests ###

[Connecting to the Network training guide](http://developer.android.com/training/basics/network-ops/connecting.html)

Check out this [blog post](http://android-developers.blogspot.com/2011/09/androids-http-clients.html) on the Android HTTP clients!

### 7. Logcat ###

You can use Monitor or, if you're a command line guru, [ADB logcat](http://developer.android.com/tools/help/adb.html?utm_source=udacity&utm_medium=mooc&utm_term=android&utm_content=adb&utm_campaign=training) to view logs.

[Reading and Writing Logs](http://developer.android.com/tools/debugging/debugging-log.html)

### 9. OpenWeatherMap API Keys ###

To learn more about permissions and privacy, check out [this documentation](https://developer.android.com/preview/features/runtime-permissions.html).

### 11. Main Thread Vs Background Thread ###

Check out the Google Android guide on threading [here](http://developer.android.com/guide/components/processes-and-threads.html#Threads).

### 12. Which Thread For AsyncTask ###

Don't want to guess? Check the [AsyncTask documentation](http://developer.android.com/reference/android/os/AsyncTask.html)!

### 17. Menu Buttons ###

[Menu training guide](http://developer.android.com/guide/topics/ui/menus.html)

### 18. Refresh Button ###

[Declaring string resources](http://developer.android.com/guide/topics/resources/string-resource.html#String)

### 19. Refresh Button Behavior ###

* [Guide to Options Menu](http://developer.android.com/guide/topics/ui/menus.html#RespondingOptionsMenu)
* [Fragment.setHasOptionsMenu(boolean) method](http://developer.android.com/reference/android/app/Fragment.html#setHasOptionsMenu(boolean))

### 21. Permissions in Android Marshmallow ###

For more information on permissions, visit [this documentation](https://developer.android.com/preview/features/runtime-permissions.html).

### 22. Permissions In The Manifest ###

See the [security section](http://developer.android.com/guide/topics/security/permissions.html) of the Android Developers site.

### 23. Adding Internet Permission ###

Check the [Android documentation](http://developer.android.com/reference/android/Manifest.permission.html)!

### 24. Postal Code Param ###

[UriBuilder](http://developer.android.com/reference/android/net/Uri.Builder.html)

### 25. Identify Desired JSON Attributes ###

You can view the JSON in a more readable format by pasting it into the [JSON Formatter and Validator](http://jsonformatter.curiousconcept.com/).

### 26. Parse Out The Max Temp ###

[JSONObject in Android](http://developer.android.com/reference/org/json/JSONObject.html)

### 28. Update The Adapter ###

Hint: Make sure FetchWeatherTask is not defined as a static class. If you're wondering why, see this link on [nested classes in Java](http://docs.oracle.com/javase/tutorial/java/javaOO/nested.html).

### 29. Source Code For ArrayAdapter ###

[ArrayAdapter source code in Android framework](https://android.googlesource.com/platform/frameworks/base/+/master/core/java/android/widget/ArrayAdapter.java)

### 33. Review Material for Lesson 2 ###

If you’re unfamiliar with JSON, take a look at [this tutorial](http://www.w3schools.com/json/).

## Lesson 3 ##

### 4. List Item Click Listener ###

[ListView Documentation](http://developer.android.com/reference/android/widget/ListView.html)

### 5. ItemClickListener And Toast ###

[Toast documentation](http://developer.android.com/guide/topics/ui/notifiers/toasts.html#Basics)

### 6. Create New Activity ###

[More info on parent activity](http://developer.android.com/training/basics/firstapp/starting-activity.html#CreateActivity)
[http://developer.android.com/design/patterns/navigation.html](http://developer.android.com/design/patterns/navigation.html)

### 9. Intents As Envelopes ###

[Common Intents page](http://developer.android.com/guide/components/intents-common.html)

### 10. Launch Detail Activity ###

[Example of an explicit intent](http://developer.android.com/guide/components/intents-filters.html#ExampleExplicit)

### 13. Settings UX ###

Follow along with Katherine in [the documentation](https://developer.android.com/design/patterns/settings.html).

UX = User Experience

### 14. Preferences ###

[Settings Developer Guide](http://developer.android.com/guide/topics/ui/settings.html)
[SharedPreferences](http://developer.android.com/reference/android/content/SharedPreferences.html)

### 16. Launch SettingsActivity ###

The reason the action bar doesn't appear is that the current version of [appcompat](https://developer.android.com/tools/support-library/features.html#v7) - which is a library that provides backwards compatibility - styles our application. Appcompat only adds an action bar to activities that derive from [ActionBarActivity](https://developer.android.com/reference/android/support/v7/app/ActionBarActivity.html) and SettingsActivity does not subclass ActionBarActivity. SettingsActivity is a subclass of [PreferenceActivity](https://developer.android.com/reference/android/preference/PreferenceActivity.html).

So why are we using PreferenceActivity? It’s an easy way to get the preference UI working on Gingerbread devices.

Fear not though, in Lesson 5 when we discuss theming and styling, we will add an action bar to our activity.

### 17. Location Setting XML ###

Follow along with Katherine in the [settings documentation](https://developer.android.com/guide/topics/ui/settings.html#DefiningPrefs).

[Defining Preferences in XML](https://developer.android.com/guide/topics/ui/settings.html#DefiningPrefs)

### 21. Temperature Units Setting ###

[Preference Documentation](http://developer.android.com/reference/android/preference/Preference.html)
[Documentation on String Arrays](http://developer.android.com/guide/topics/resources/string-resource.html#StringArray)

### 24. Add Map Location Intent ###

See [Common Intents](https://developer.android.com/guide/components/intents-common.html) for examples of the map intent.

### 25. Intent Resolution ###

The activity within the Maps app included:

    <intent-filter>
      <action:name="android.intent.action.VIEW" />
      <data android:scheme="geo" />
    </intent-filter>

This could be used in own app: Android will check intent filters of every installed app for the appropriate scheme.

### 26. Share Intent ###

For more information on ShareActionProviders, see the documentation [here](http://developer.android.com/training/sharing/shareaction.html).
