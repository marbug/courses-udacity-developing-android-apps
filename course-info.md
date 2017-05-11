# Course Info #

## The Directory Structure of Android Studio ##

There are multiple ways to view your project in Android Studio 1.0. We’ll work with the **Project** view, but the default **Android** view is also useful.

More in-depth information can be found [here](https://developer.android.com/tools/projects/index.html).

## Specific changes ##

* In your starting code (which you just downloaded) the **fragment** is an inner class of **MainActivity**. In the new template it is divided into two separate classes, in two separate files.

* In the starting code the **fragment** class is named **PlaceholderFragment**. In the new template it is called **MainActivityFragment**.

* In the starting code **PlaceholderFragment** is added programmatically to the **MainActivity**. The following code in MainActivity's **onCreate** method adds the fragment programmatically:

        if (savedInstanceState == null) {
            getSupportFragmentManager().beginTransaction()
                    .add(R.id.container, new PlaceholderFragment())
                    .commit();
        }

    Then in the XML, a **FrameLayout** is used for the **MainActivity.java** layout (defined in **activity_main.xml**).

* In the new template, the fragment is added using the XML layout code for MainActivity. In the **activity_main.xml** the code is:

        <fragment xmlns:android="http://schemas.android.com/apk/res/android"
         xmlns:tools="http://schemas.android.com/tools" android:id="@+id/fragment"
         android:name="com.example.android.sunshine.MainActivityFragment"
         tools:layout="@layout/fragment_main" android:layout_width="match_parent"
         android:layout_height="match_parent" />

## Android Software Stack and Gradle ##

The flow is:

* Android Project
* Gradle (Build)
* Gradle (APK)

    * Byte Code
    * Resources
    * Manifest

* JarSigner (Sign)
* ADB (Install on Device)

## Layouts ##

There are:

* LinearLayout
* RelativeLayout
* GridLayout

and:

* Frame Layout
* Linear Layout
* Relative Layout

| Prev page | Next page |
| --------- | --------: |
| [README](README.md) |  |
