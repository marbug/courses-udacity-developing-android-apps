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

### 27. Broadcast Intents ###

Examples: device is charging or that it's just finished rebooting.
To do that ourselves, we use the [SendBroadcast](https://developer.android.com/reference/android/content/Context.html) method.

### 28. Intent Filters ###

The receiver itself is pretty simple:

    public class MyReceiver extends BroadcastReceiver  {

      @Override
      public void onReceive(Context context, Intent intent) {
        // handle received intent
      }
    }

To have your receiver start listening for broadcasts, you need to register it either through an entry in your manifest like this:

    <receiver android:name=".MyReceiver">
      <intent-filter>
        <action android:name="com.myapp.NEW_LIFEFORM" />
      </intent-filter>
    </receiver>

or dynamically within other application component:

    IntentFilter intentFilter = new IntentFilter("com.myapp.NEW_LIFEFORM");

    registerReceiver(myReceiver, intentFilter);

The biggest difference between manifest and dynamic receivers is when they're triggered:

|                | Manifest | Dynamic |
| -------------- | -------- | ------- |
| App Running    |     +    |    +    |
| App Terminated |     +    |    -    |

[BroadcastReceiver](https://developer.android.com/reference/android/content/BroadcastReceiver.html)
[Monitoring Battery](https://developer.android.com/training/monitoring-device-state/battery-monitoring.html)

### 30. Android Distribution Platform ###

[Core App Quality Guidelines](http://developer.android.com/distribute/essentials/quality/core.html)

## Lesson 4 ##

### 1. Intro to Popular Movies App, Stage 1 ###

#### Project Overview ####

Most of us can relate to kicking back on the couch and enjoying a movie with friends and family. In this project, you’ll build an app to allow users to discover the most popular movies playing. We will split the development of this app in two stages. First, let's talk about stage 1. In this stage you’ll build the core experience of your movies app.

You app will:

* Present the user with a grid arrangement of movie posters upon launch.
* Allow your user to change sort order via a setting:

    * The sort order can be by most popular or by highest-rated

* Allow the user to tap on a movie poster and transition to a details screen with additional information such as:

    * original title
    * movie poster image thumbnail
    * A plot synopsis (called overview in the api)
    * user rating (called vote_average in the api)
    * release date

#### Why this Project? ####

To become an Android developer, you must know how to bring particular mobile experiences to life. Specifically, you need to know how to build clean and compelling user interfaces (UIs), fetch data from network services, and optimize the experience for various mobile devices. You will hone these fundamental skills in this project.

By building this app, you will demonstrate your understanding of the foundational elements of programming for Android. Your app will communicate with the Internet and provide a responsive and delightful user experience.

#### What Will I Learn After Stage 1? ####

* You will fetch data from the Internet with theMovieDB API.
* You will use adapters and custom list layouts to populate list views.
* You will incorporate libraries to simplify the amount of code you need to write

### 2. Popular Movies App, Stage 1 Instructions ###

#### How Will I Complete this Project? ####

To submit this project for feedback, check out the [Android Developer Nanodegree Program](https://www.udacity.com/nanodegrees-new-s/nd801).

#### Supporting Course Material ####

You should have the skills you need to complete this app after completing Lessons 1-3 of this course.

If you'd like to make your app's UI beautiful, we also suggest reviewing this material from Lesson 5, which goes into greater detail about how to make more detailed layouts.

#### Required Tasks ####

* Build a UI layout for multiple Activities.
* Launch these Activities via Intent.
* Fetch data from themovieDB API

#### Implementation Guide ####

For step-by-step support, we've provided details on how to approach each task in this [Implementation Guide](https://docs.google.com/document/d/1ZlN1fUsCSKuInLECcJkslIqvpKlP7jWL2TP9m6UiA6I/pub?embedded=true).

### 3. Popular Movies App Rubric ###

#### Project Rubric ####

Assess your project using this rubric.

Be sure to review the rubric thoroughly before you get started!

## Lesson 5 ##

### 3. The Android Activity Lifecycle ###

* onCreate
* [created]
* onStart
* [visible]
* onResume
* [active]
* onPause
* [focus is lost - paused] - could be moved to onResume
* onStop
* [stopped] - can be moved via onRestart to onStart
* onDestroy
* [destroyed] - can be moved to onCreate

You can find a diagram of the Android Activity Life Cycle [here](https://s3.amazonaws.com/content.udacity-data.com/course/ud853/Android_Activity_LifeCyle.png).

Read more about it on the [Android Developers site](http://developer.android.com/training/basics/activity-lifecycle/starting.html).

### 8. What To Do In OnPause/OnStop ###

Some examples of listeners or updates you should disconnect or stop when onPause or onStop are received:

* Sensor Listeners
* Location Updates
* Dynamic Broadcast Receivers
* Game Physics Engine

After onPause app is still visible, so do not stop drawing your UI.

### 12. Optional SQLite Tutorial ###

#### Optional SQLite Tutorial ####

Since Sunshine will be using a SQLite database to store weather data, you should have a basic understanding of SQLite and its commands before continuing this lesson. This is an optional exercise for anyone new to SQL databases or anyone in need of a refresher.

#### Introduction ####

SQLite is a relational database management system, which is an implementation of SQL (Structured Query Language). It comes packaged with the Android OS as a C++ library so that apps can have private databases. SQL can be used to create, search and maintain databases. In this tutorial, you will learn about the syntax and usage of SQL and see how to create and manage a small database on your computer. The commands you learn here are similar to the SQL commands you will write for your Sunshine app, in order to store and retrieve weather data from a SQLite database.

#### Get SQLite ####

1. Download the SQLite command line shell and install. You can follow [this tutorial](http://www.tutorialspoint.com/sqlite/sqlite_installation.htm) or go directly to [http://sqlite.org/download.html](http://sqlite.org/download.html)

2. Open terminal and navigate to a folder of your choice where you will save your database. Create a new database file called sunshine.db and start the SQLite shell (which will recognize your SQL commands) by typing:

    sqlite3 sunshine.db

3. For a list of all commands:

    .help

4. One of the commands is to list out all databases. It should display one database called main and the file location on your computer for sunshine.db.

    .databases

In an app, you can have multiple databases. Our Sunshine app will only have a single database, and that database can contain multiple tables.

#### Create A Database Table ####

1. A table is a collection of rows and columns like a spreadsheet. Use the [CREATE TABLE statement](http://www.tutorialspoint.com/sqlite/sqlite_create_table.htm) to create a new database table called “weather.” Each row will be one day’s worth of weather data. It should have 6 columns of data: ID, date, min temperature, max temperature, humidity, and pressure.

In the CREATE TABLE statement, each column definition is separated by commas, where you provide the column name and datatype for that column. We also specify that the column should be non-null. We specify the _id column to be the primary key and it’s an integer.

    CREATE TABLE weather( _id INTEGER PRIMARY KEY, date TEXT NOT NULL, min REAL NOT NULL, max REAL NOT NULL, humidity REAL NOT NULL, pressure REAL NOT NULL);

The list of possible [SQLite data types](http://www.sqlite.org/datatype3.html) is a useful resource, or you can see [this tutorial](http://www.tutorialspoint.com/sqlite/sqlite_data_types.htm).

Note: SQLite keywords, such as CREATE TABLE or PRIMARY KEY, are capitalized for ease of readability to distinguish them from the table and column names that we’ve selected, but you can lowercase the keywords if you want.

Note: This is not the full table you’ll be using in Sunshine, this is just a simpler version of the table.

2. Use this command to list out all tables. Ensure that the weather table was created.

    .tables

3. Use a [SELECT statement](http://www.tutorialspoint.com/sqlite/sqlite_select_query.htm) to return out all rows in the weather table. The * is a symbol that means “all of the columns”. At this time, nothing will be returned because the table is created, but there is no data in the table yet.

    SELECT * FROM weather;

4. At any point, you can find out the schema of how the tables were created in the database

    .schema

#### Insert rows ####

1. Use an [INSERT statement](http://www.tutorialspoint.com/sqlite/sqlite_insert_query.htm) to insert a new row of data into the weather table. The following INSERT statement inserts a row into the weather table for June 25th, 2014, which had a low of 16 degrees, a high of 20 degrees, 0 humidity and 1029 pressure. The _id of this row is 1.

    INSERT INTO weather VALUES(1,'20140625',16,20,0,1029);

2. Query for all rows in the weather table, and you should see the one row of data you just inserted.

    SELECT * FROM weather;

3. To have the column name be printed out as well (for easier readability as to what value corresponds to which column), turn the header on. Then do the query again.

    .header on
    SELECT * FROM weather;

4. Experiment by inserting another 3 rows of data into the weather table.

    INSERT INTO weather VALUES(2,'20140626',17,21,0,1031); INSERT INTO weather VALUES(3,'20140627',18,22,0,1055); INSERT INTO weather VALUES(4,'20140628',18,21,10,1070);

Query for all rows to verify they were inserted properly.

    SELECT * FROM weather;

#### Query rows ####

1. Practice doing queries where you provide a selection [WHERE clause](http://www.tutorialspoint.com/sqlite/sqlite_where_clause.htm) to narrow down the number of rows that are returned in the result. Always remember the semicolon at the end of a statement!

For all possible SQLite operators, see this [link](http://www.tutorialspoint.com/sqlite/sqlite_operators.htm).

This query returns rows from the weather table where the date column exactly equals the 20140626.

    SELECT * FROM weather WHERE date == 20140626;

2. This query returns rows from the weather table where the date column is between 20140625 and 20140628. However, all columns are not returned, we just return the 4 specified columns (_id, date, min, and max) of the rows that match the query.

    SELECT _id,date,min,max FROM weather WHERE date > 20140625 AND date < 20140628;

3. This query returns rows where the minimum temperature is greater than or equal to 18. Based on those matching rows, we order them based on increasing (also known as ascending or “ASC” for short) max temperature. The first row of the result that is printed out to the command line will be the row (with min temperature >= 18) with max temperature that is lowest out of all rows, so that subsequent rows will have higher max temperature.

    SELECT * FROM weather WHERE min >= 18 ORDER BY max ASC;

#### Update rows ####

1. You can also update existing rows in the database with an [UPDATE statement](http://www.tutorialspoint.com/sqlite/sqlite_update_query.htm). This statement updates the weather table by setting the minimum temperature to be 0 and maximum temperature to be 100 for rows where the date is greater than 20140626 but less than 20140627.

    UPDATE weather SET min = 0, max = 100 where date >= 20140626 AND date <= 20140627;

When you print out the whole weather table again, you can see that 2 rows were changed.

    SELECT * FROM weather;

#### Delete rows ####

1. Use a [DELETE statement](http://www.tutorialspoint.com/sqlite/sqlite_delete_query.htm) to delete rows from a database table that match the given selection clause. In this case, we delete any rows from the weather table where humidity is not equal to 0.

    DELETE FROM weather WHERE humidity != 0;

#### Add columns ####

1. If you have released a version of your app to users, and then decide you need to change the database schema, such as adding columns, then you’ll need to upgrade your database. You can alter existing tables, by using the [ALTER TABLE command](http://www.tutorialspoint.com/sqlite/sqlite_alter_command.htm).

Note: In general, you shouldn’t alter a table to remove a column because you’re deleting data and other tables could depend on that column. Instead you can just null out all values in that column.

This statement alters the weather table by adding another column to the table called description, which will always be non-null and contain text. It will also default to the value ‘Sunny’ if no value is provided. In reality, you would choose a more reasonable default, but this is just for example purposes.

    ALTER TABLE weather ADD COLUMN description TEXT NOT NULL DEFAULT 'Sunny';

Verify that the new description column exists when you query all rows and all columns.

    SELECT * FROM weather;

#### Delete table ####

Delete the weather table by using the [DROP TABLE command](http://www.tutorialspoint.com/sqlite/sqlite_drop_table.htm). Verify there are no more tables in the database.

    DROP TABLE weather;
    .tables

These are just the basics. Feel free to play around with SQLite some more. See this link: [http://www.sqlite.org/cli.html](http://www.sqlite.org/cli.html)

When you’re done, enter .quit to exit.

### 14. Storing Data In Android: Conclusion ###

[Data storage guide on the developer.android.com](http://developer.android.com/guide/topics/data/index.html)


### 17. Intro To WeatherContract ###

[Contacts Contract](http://developer.android.com/reference/android/provider/ContactsContract.html)

### 20. Two Tables ###

[Foreign Keys ](http://www.w3schools.com/sql/sql_foreignkey.asp)
[Inner Join](http://www.tutorialspoint.com/sqlite/sqlite_using_joins.htm)

Hint: _id is the primary key of the table and should be set to [autoincrement](http://www.tutorialspoint.com/sqlite/sqlite_using_autoincrement.htm)

### 22. Define Constants In Contract ###

Some background on [BaseColumns](http://developer.android.com/reference/android/provider/BaseColumns.html).

Inner joins are well documented [here](http://en.wikipedia.org/wiki/Join_(SQL)#Inner_join).

We're going to cover [Content Providers](http://developer.android.com/guide/topics/providers/content-providers.html) thoroughly later in Lesson 4. We're going to cover [Content Providers](http://developer.android.com/guide/topics/providers/content-providers.html) thoroughly later in Lesson 4.

### 23. SQLiteOpenHelper And Sunshine Database ###

[SQLiteOpenHelper](http://developer.android.com/reference/android/database/sqlite/SQLiteOpenHelper.html)
[JUnit testing](http://www.tutorialspoint.com/junit/junit_quick_guide.htm)
[Android testing](http://developer.android.com/tools/testing/testing_android.html)

### 25. Create Sunshine Location Database ###

See [this page](http://developer.android.com/sdk/installing/studio-tips.html) for more keyboard shortcuts.

[ON CONFLICT clause](https://www.sqlite.org/lang_conflict.html)

### 26. SQLiteOpenHelper OnUpgrade() ###

[ALTER TABLE](https://www.sqlite.org/lang_altertable.html)

### 27. Read/Write From A Database ###

[SQLite Database documentation](http://developer.android.com/reference/android/database/sqlite/SQLiteDatabase.html)

### 28. Test Read/Write From Location Table ###

[cursor.getColumnIndex()](http://developer.android.com/reference/android/database/Cursor.html#getColumnIndex(java.lang.String))

## Lesson 6 ##

### 2. Create A Content Provider ###

If you're new to ContentProviders, check out our [gnarlicious background lesson](https://www.udacity.com/course/ud258).

### 3. Get the Content Provider Code ###

#### What is a Content Provider? ####

Dan just mentioned the [Content Provider mini lesson](https://classroom.udacity.com/courses/ud258/lessons/3372188753/concepts/34096686680923). If you're not sure what a content provider is or why you would use one, please take this short mini lesson and exercise before continuing in the course. The exercise will take you through an example of grabbing data from the [UserDictionary](http://developer.android.com/reference/android/provider/UserDictionary.html) content provider and displaying it in a list.

### 5. Add A Weather W/Location UriBuilder ###

[Documentation on UriBuilder](http://developer.android.com/reference/android/net/Uri.Builder.html)

### 7. Write The UriMatcher ###

[Documentation on UriMatcher](http://developer.android.com/reference/android/content/UriMatcher.html)

### 8. Register The Content Provider ###

[Documentation on provider](http://developer.android.com/guide/topics/manifest/provider-element.html)
[ContentProvider basics](http://developer.android.com/guide/topics/providers/content-provider-basics.html#ClientProvider)

### 12. Implement Weather And Location Queries ###

[Documentation on parseId](http://developer.android.com/reference/android/content/ContentUris.html#parseId(android.net.Uri))

## Lesson 7 ##

### 1. Loaders Are Awesome ###

[AsyncTaskLoader](http://developer.android.com/reference/android/content/AsyncTaskLoader.html) is a **Loader** that uses an **AsyncTask** behind the scenes to do its work.

### 7. Leveraging Loaders ###

[Documentation on loaders](http://developer.android.com/guide/components/loaders.html)
[Documentation on CursorLoader](http://developer.android.com/reference/android/content/CursorLoader.html)

### 14. 3rd Party Content Providers ###

Android provides a number of [ContentProviders](http://developer.android.com/reference/android/provider/package-summary.html) natively to interact with common types of data such as the photos or audio media. For your project, if you choose to use any of the native content provides, you'll likely use at most the [Calendar Provider](http://developer.android.com/guide/topics/providers/calendar-provider.html) and the [Contacts Provider](http://developer.android.com/guide/topics/providers/contacts-provider.html).

## Lesson 8 ##

### 2. Android Design Principles ###

For some guidance on how to make slick and beautiful apps, check out [Material Design](https://developer.android.com/design/material/index.html). Material Design is a design language incorporated in the Android Lollipop release. The [Material Design specifications](http://www.google.com/design/spec/material-design/introduction.html#) is a great place to start.

### 3. Enjoyable Apps ###

If you are enrolled in the Android Nanodegree, you can post your responses in the Android Cafe [here](https://discussions.udacity.com/t/inspiring-android-apps/19666). If you are taking the paid version of this course, please post your response in the coaches lounge [here](https://discussions.udacity.com/t/what-makes-your-favorite-app-s-enjoyable-to-use/26445). If you are taking the free version of the course, feel free to post in the student forum [here](https://discussions.udacity.com/t/what-makes-your-favorite-apps-enjoyable-to-use/31726).

### 4. Recap On Views And ViewGroups ###

[Link to Android Design Building Blocks](http://developer.android.com/design/building-blocks/index.html)

### 5. Building List Item ###

You should use Layout Weight and can read about it [here](http://developer.android.com/guide/topics/ui/layout/linear.html#Weight).

### 9. Using The ViewHolder Pattern ###

Learn more about View Holder pattern [here](http://developer.android.com/training/improving-layouts/smooth-scrolling.html).

I found [this link](http://developer.android.com/training/contacts-provider/display-contact-badge.html#ListView) (under “Define the custom list adapter”) to be helpful.

### 10. Formatting Strings ###

Remember to import the xliff namespace in the strings.xml file as well.

[xliff tags](https://developer.android.com/distribute/tools/localization-checklist.html)
[Formatting strings](http://developer.android.com/guide/topics/resources/string-resource.html#FormattingAndStyling)
[context.getString() method](http://developer.android.com/reference/android/content/Context.html#getString)

### 12. Optimizing Layouts ###

1. Keep your layout shallow and wide, rather than deep and narrow.

I.e.

    * item1
        * item2
        * item3
        * item4

is better than

    * item1
        * item2
          * item3
          * item4

2. Your activities' full hierarchy should never have more than 10 nested Views or 80 Views in total.

### 13. Hierarchy Viewer ###

[Optimizing your UI](http://developer.android.com/tools/debugging/debugging-ui.html)

[Hierarchy Viewer](http://developer.android.com/tools/help/hierarchy-viewer.html)

[Lint](http://developer.android.com/tools/help/lint.html)

Note: Hierarchy Viewer is in **sdk/tools/hierarchyviewer**. Alternativly you can open it by going to the Android Device Monitor and then clicking the Hierarchy Viewer button.

Hierarchy Viewer only works by default with phones running a developer version of the Android OS. If your phone is not a developer phone, you have a few options:

1. If you have a phone running Jellybean or higher, you can simply add the environment variable ANDROID_HVPROTO with the value ddm:

    ANDROID_HVPROTO=ddm

2. You can run Hierarchy Viewer on an emulated phone.
3. Or you can use use the [ViewServer](https://github.com/romainguy/ViewServer) library to get Hierarchy Viewer working on a non-developer, pre Jellybean phone.

### 14. Responsive Design ###

Resources:

* [Tablet App Quality](http://developer.android.com/distribute/essentials/quality/tablets.html)
* Android Design Guide: [Multi-Pane Layouts](https://developer.android.com/design/patterns/multi-pane-layouts.html)
* Android Design in Action: [Responsive Design (video)](https://www.youtube.com/watch?v=zHirwKGEfoE)

### 15. Splitting Devices Into Buckets ###

[Configuration Examples](http://developer.android.com/guide/practices/screens_support.html#ConfigurationExamples)

[Convert dips to pixels](http://developer.android.com/guide/practices/screens_support.html#dips-pels)

| By Size     |          |
| ----------- | -------- |
| Phones      | < 600 dp |
| 7" tablets  | > 600 dp |
| 10" tablets | > 720 dp |

| By density |       |
| ---------- | ----- |
| LDPI       | ~ 120 |
| MDPI       | ~ 160 |
| HDPI       | ~ 240 |
| XHDPI      | ~ 320 |
| XXHDPI     | ~ 480 |
| XXXHDPI    | ~ 640 |

* Use density-independent pixels (dip or dp)

### 16. Resource Folder Qualifiers ###

[Supporting Multiple Screens](http://developer.android.com/guide/practices/screens_support.html)

### 17. Screen Density Size ###

[Supporting Multiple Screens](http://developer.android.com/guide/practices/screens_support.html)
[Metrics and Grids](http://developer.android.com/design/style/metrics-grids.html)

### 18. Images For Different Densities ###

[Devices and Displays](https://developer.android.com/design/style/devices-displays.html)

[Converting dp to pixel](http://developer.android.com/guide/practices/screens_support.html#dips-pels)

### 19. Adding Images To The App ###

[Application element in AndroidManifest.xml](http://developer.android.com/guide/topics/manifest/application-element.html)

### 20. Tablet UX Mocks ###

[Building a Flexible UI](http://developer.android.com/training/basics/fragments/fragment-ui.html)

### 24. Try The Fragment Manager ###

Check out the [documentation](http://developer.android.com/guide/components/fragments.html) on Fragments.

### 30. Activated List Item Style ###

[Read about ListView choice mode](http://developer.android.com/reference/android/widget/AbsListView.html#attr_android:choiceMode)
[Read about styles](http://developer.android.com/guide/topics/ui/themes.html)
[State list drawable](http://developer.android.com/guide/topics/resources/drawable-resource.html#StateList)

### 33. Wide Detail Fragment ###

[Layout aliasing](http://developer.android.com/training/multiscreen/screensizes.html#TaskUseAliasFilters)

### 35. Visual Mocks ###

[Link to Visual Mocks with Redlines for Sunshine](https://www.udacity.com/wiki/ud853/design_assets) (PDF and individual PNGs)

[Android Design Guide: Metrics and Grids](https://developer.android.com/design/style/metrics-grids.html)

### 36. Action Bar ###

Guide on [Styling the Action Bar](https://developer.android.com/training/basics/actionbar/styling.html)
Documentation for [displayOptions](http://developer.android.com/reference/android/R.attr.html#displayOptions) attribute

General resources on the Action Bar:
[Android Design Guide: Action Bar](http://developer.android.com/design/patterns/actionbar.html)
[Developer Guide on Action Bar](http://developer.android.com/guide/topics/ui/actionbar.html)
[Using a Logo Instead of an Icon](http://developer.android.com/guide/topics/ui/actionbar.html#Logo)

### 37. Settings Bar ###

#### Adding the Settings Bar ####

One more quick tweak. We are going to add an update to make the action bar appear in settings. The three themes are **AppTheme**, **ForecastTheme** and **SettingsTheme** and we will have a v21 and v14 version.

#### If you're wondering why no Action Bar... ####

The reason the action bar doesn't appear is that the current version of [appcompat](https://developer.android.com/tools/support-library/features.html#v7) - which is a library that provides backwards compatibility - styles our application. Appcompat only adds an action bar to activities that derive from [ActionBarActivity](https://developer.android.com/reference/android/support/v7/app/ActionBarActivity.html) and SettingsActivity does not subclass ActionBarActivity. SettingsActivity is a subclass of [PreferenceActivity](https://developer.android.com/reference/android/preference/PreferenceActivity.html).

So why are we using PreferenceActivity? It’s an easy way to get the preference UI working on Gingerbread devices.

By explicitly themeing SettingActivity with a theme derived from DarkActionBar, we are able to add back the Action Bar.

### 39. Implementing Redlines On Your Own ###

Helpful Resources:

[Typography](http://developer.android.com/design/style/typography.html)
[Text appearance](https://plus.google.com/108967384991768947849/posts/gQuBtnuk6iG)
[Color](http://developer.android.com/guide/topics/resources/more-resources.html#Color)
[Layout gravity](http://stackoverflow.com/questions/3482742/android-gravity-and-layout-gravity)

### 41. Coding Task On Accessibility ###

[Documentation on Accessibility](http://developer.android.com/guide/topics/ui/accessibility/index.html)
[Accessibility Developer Checklist](http://developer.android.com/guide/topics/ui/accessibility/checklist.html)
Android Design Guide: [Accessibility](http://developer.android.com/design/patterns/accessibility.html)
[Accessibility Testing Checklist](http://developer.android.com/tools/testing/testing_accessibility.html)

### 44. Create Your Own View ###

Check out the [Canvas and Drawables](http://developer.android.com/guide/topics/graphics/2d-graphics.html) guide and the [Custom Drawing](http://developer.android.com/training/custom-views/custom-drawing.html) guide.

### 45. Custom View Accessiblity ###

If you want to develop a Custom View you can reference the documentation on [Creating Custom Views](https://developer.android.com/training/custom-views/index.html) and, more specifically, the documentation on [Designing For Accessibility](https://developer.android.com/training/custom-views/create-view.html#accessibility).

### 46. Input Events In Custom Views ###

[Motion Event Docs](http://developer.android.com/reference/android/view/MotionEvent.html)
[Custom Views](http://developer.android.com/training/custom-views/index.html)

## Lesson 9 ##

### 5. Using Services ###

[IntentService](http://developer.android.com/reference/android/app/IntentService.html)
[Guide on Services](http://developer.android.com/guide/components/services.html)

### 6. Using Alarms ###

[Set a Repeating Alarm](https://developer.android.com/training/scheduling/alarms.html#set)
[PendingIntent](http://developer.android.com/reference/android/app/PendingIntent.html)
[BroadcastReceiver](http://developer.android.com/reference/android/content/BroadcastReceiver.html)

### 10. Data Transfer Best Practices ###

[Transferring Data Without Draining the Battery](http://developer.android.com/training/efficient-downloads/index.html)
[DevBytes: Efficient Data Transfers](https://www.youtube.com/watch?v=cSIB2pDvH3E&list=PLWz5rJ2EKKc-VJS9WQlj9xM_ygPopZ-Qd)

### 11. Introducing SyncAdapters ###

Read more about [Sync Adapters](http://developer.android.com/training/sync-adapters/index.html).

### 15. Google Cloud Messaging ###

[Developer guide for Google Cloud Messaging](http://developer.android.com/google/gcm/index.html)

### 16. Notifications ###

Check out the [Notifications](http://developer.android.com/guide/topics/ui/notifiers/notifications.html) tutorial for a helpful example.

Related classes:

[NotificationCompat.Builder](http://developer.android.com/reference/android/support/v4/app/NotificationCompat.Builder.html)
[NotificationManager](http://developer.android.com/reference/android/app/NotificationManager.html)
[PendingIntent](http://developer.android.com/reference/android/app/PendingIntent.html)
[TaskStackBuilder](http://developer.android.com/reference/android/support/v4/app/TaskStackBuilder.html)
